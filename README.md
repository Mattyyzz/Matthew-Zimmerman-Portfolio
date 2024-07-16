# Matthew-Zimmerman-Portfolio
A portfolio featuring my knowledge of various applications. 

# Java: URL Creation Project 

I programmed in the 'Eclipse IDE for Java Developers - 2023-06' for this project.

![image](https://github.com/user-attachments/assets/71a59edb-6620-4659-b49c-796dd6144bab)

This project involved developing a Java application to dynamically generate and manage URLs for websites. I applied fundamental Java programming concepts such as object-oriented design, encapsulation (using getters and setters for attributes), and user input handling (using the Scanner class). I also utilized concepts such as attributes, methods, strings, booleans, and if-else statements to develop my code. By incorporating these Java properties, the program ensured robustness and flexibility in constructing URLs based on user-specified domain, subdomain, path, and security preferences (HTTP or HTTPS). Aditionally, users could indicate whether the website served a non-profit or for-profit purpose, influencing the URL's structure and content presentation. This project exemplifies my proficiency in Java development and my ability to create practical solutions that meet specific application requirements with clarity and precision.

# URL Class

My first class, the Url class, serves as a blueprint for representing and managing URL attributes within a Java application. It encapsulates essential components such as the complete URL, domain, optional subdomain, path, and security status (secure or not). Through its setter methods, it allows for dynamic updating of these attributes, ensuring that the complete URL is consistently updated based on any changes. The class also includes methods like printUrlInfo() to display comprehensive information about the URL, including whether the site is non-profit or for-profit, which is crucial for distinguishing between different types of organizations. 

![Screenshot (112)](https://github.com/user-attachments/assets/175b77c1-20b7-4618-b0ee-b2b87a7cd209)
![Screenshot (113)](https://github.com/user-attachments/assets/7fbc297f-5c3f-4fe5-9c40-bf09133cb8f3)

# URLCreator Class

My second class, the UrlCreator class, utilizes a Scanner object to interactively prompt users for essential details such as domain name, optional subdomain, path, and security preferences (HTTP or HTTPS). Through well-defined methods for user input handling and validation, it ensures accurate construction of URLs based on user specifications. Once all necessary details are gathered, an instance of the Url class is initialized and populated with these attributes. Finally, the UrlCreator class orchestrates the process of collecting user inputs, constructing a complete URL, and displaying comprehensive information about the generated URL through the Url class methods.

![Screenshot (114)](https://github.com/user-attachments/assets/0957355e-b38f-409e-b189-9838c85e8ea9)

# Console Example

Here is a console example of what information the user can input that results in their URL when following the prompting steps. 

![Screenshot (115)](https://github.com/user-attachments/assets/ec20b872-6280-46b0-ad5e-e2e0b8742834)

In this example, we have a domain, subdomain, path, and are asking the user questions such as if the website is a non-profit and is secure or not. 




