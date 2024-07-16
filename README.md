# Matthew-Zimmerman-Portfolio
A portfolio featuring my knowledge of various applications. 

public class Url {
	private String completeUrl;
	private String domain;
	private String subdomain;
	private String path;
	private boolean isNonProfit;
	private boolean isSecure;

	// Getters and setters
	public String getCompleteUrl() {
		return completeUrl;
	}

	public void setCompleteUrl(String completeUrl) {
		this.completeUrl = completeUrl;
	}

	public String getDomain() {
		return domain;
	}

	public void setDomain(String domain) {
		this.domain = domain;
		updateCompleteUrl();
	}

	public String getSubdomain() {
		return subdomain;
	}

	public void setSubdomain(String subdomain) {
		this.subdomain = subdomain;
		updateCompleteUrl();
	}

	public String getPath() {
		return path;
	}

	public void setPath(String path) {
		this.path = path;
		updateCompleteUrl();
	}

	public boolean isNonProfit() {
		return isNonProfit;
	}

	public void setNonProfit(boolean isNonProfit) {
		this.isNonProfit = isNonProfit;
		updateCompleteUrl();
	}

	public boolean isSecure() {
		return isSecure;
	}

	public void setSecure(boolean isSecure) {
		this.isSecure = isSecure;
		updateCompleteUrl();
	}

	// Update the complete URL based on domain, subdomain, path, and security status
	private void updateCompleteUrl() {
		String protocol = isSecure ? "https://" : "http://";
		String subdomainPart = subdomain != null && !subdomain.isEmpty() ? subdomain + "." : "";
		String pathPart = path != null && !path.isEmpty() ? "/" + path : "";
		this.completeUrl = protocol + subdomainPart + domain + pathPart;
	}

	// Method to print URL information
	public void printUrlInfo() {
		System.out.println("Complete URL: " + completeUrl);
		System.out.println("Website Domain: " + domain);
		System.out.println("Subdomain: " + subdomain);
		System.out.println("Path: " + path);
		System.out.println("The website is " + (isSecure ? "secure" : "not secure"));
		System.out.println(
				"This site is used for a " + (isNonProfit ? "non-profit organization" : "for-profit business"));
	}
}

