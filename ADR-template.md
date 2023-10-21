# Architectural Decision Record: Mobile Retail App

## 1. Native, Web, or Hybrid App

### Decision 
We have decided to develop a native mobile app for the retail company.

### Rationale 
On both iOS and Android platforms, native applications provide the finest performance and user interface with robust offline capabilities. They tend to be more performant compared to web or hybrid apps. They have direct access to device features like the camera, GPS, and sensors, which are essential for implementing push notifications. Moreover, they offer more security options, which are crucial when handling customer data and payment information.

### Status
Accepted

### Consequences
Advantages: The native app will provide superior performance, responsiveness, and offline capabilities, enhancing user experience and ensuring data security.  
Challenges: Building native apps may require more effort and may take slightly longer development time compared to web or hybrid applications.

## 2. UI Framework

## Decision 
We have decided to use React Native as the UI framework for the development of the application.

## Rationale 
With React Native, we can create a single codebase that can be used for both iOS and Android platforms, ensuring a consistent experience for users. It actively supports the latest platform-specific features and design patterns like gesture controls, animations, and UI interactions. The advantages in terms of development effectiveness, performance, and user experience exceed the little overhead, even though some platform-specific code may still be required.

## Status
Accepted

## Consequences
Advantages: Choosing React Native as the UI framework ensures a UI that aligns with the conventions of iOS and Android, providing a familiar and consistent UX. It improves responsiveness and performance, which are essential for a retail app with a large volume of data and graphics. It also speeds up development by allowing code to be shared between platforms.  
Challenges: While React Native provides exceptional development efficiency, certain features or optimizations may require platform-specific development effort. However, the advantages in terms of performance and user experience usually outweigh the work and expenditure.

## 3. Backend Language

### Decision 
We have decided to use Node.js as the backend language for the development of the application.

### Rationale 
Node.js has a non-blocking, event-driven design which promotes real-time data synchronization. It is well-known for its capacity to manage a large number of concurrent connections, making it suitable for supporting large customer basewhile also satisfying the scalability needs of the retail app. Since React Native uses JavaScript, using Node.js for the backend can streamline the development process and enable code sharing between the frontend and backend. Moreover, it has robust ecosystem of libraries and modules making it easier to integrate with wide range of services and APIs.

### Status
Accepted

### Consequences
Advantages: It enables efficient real-time data synchronization, scalability, and seamless integration with third-party services. It leverages the expertise of JavaScript developers.  
Challenges: Node.js is renowned for its scalability, although for high loads, careful architecture and optimization may still be needed. Some team members may need to learn more about Node.js or broaden their understanding of it.

## 4. Permissions

### Decision 
We have decided to implement a granular permissions system to control access to application features and data.

### Rationale 
Granular permissions system ensures that sensitive user data, such as payment information, is only accessible by authorized users which helps in maintaining data security and protecting user privacy. Different user roles or privileges have varying access needs, this system allows us to customize the app’s functionality based on these roles.

### Status
Accepted

### Consequences
Advantages: By regulating access to critical information, a granular permissions system improves data security. It enables a personalized user experience based on roles and rights, which improves user happiness and app usability.  
Challenges: A granular permissions system can be difficult to design and deploy,necessitating considerable planning and development work. It will be a continuous responsibility to maintain and update the permissions system as user roles and access needs change.

## 5. Data Storage

### Decision 
We have decided to use a combination of local storage on the mobile device and a server-side database for data storage.

### Rationale 
Local storage on the mobile device will enable offline data access, allowing customers to use certain features without an internet connection. A server-side database, such as MongoDB, can handle the storage and retrieval of a large volume of data efficiently. This server-side database will ensure data consistency and reduce the risk of data loss in case of device failure, ensuring that customer data is reliable and up to date.

### Status
Accepted

### Consequences
Advantages: The method of choice gives a complete solution, allowing for scalability and data integrity through a server-side database and offline support through local storage. It guarantees that users can access data even when they are not online.  
Challenges: It might be challenging to create and maintain synchronization techniques between local storage and the server-side database. It may need continual work to resolve disputes and guarantee that data is consistent across all platforms and devices.

## 6. Analytics Tool 

### Decision 
We have decided to implement Google Analytics as the analytics tool for the application.

### Rationale 
The Google Analytics platform provides a consistent set of features and functionality, across both iOS and Android, such as event tracking, e-commerce tracking, and user segmentation. It can be easily integrated into the app using SDKs and APIs which simplifies the implementation process and ensures that data is collected effectively. Moreover, it provides user demographics and interests data, helping us understand the app’s audience and tailor content accordingly.

### Status
Accepted

### Consequences
Advantages: Integrating Google Analytics delivers a comprehensive set of analytics capabilities, facilitates integration, provides insights into user activity, and provides data visualization tools. This allows for data-driven decision-making and contributes to the app's performance and user experience.  
Challenges: The analytics tool must be managed and configured on an ongoing basis to ensure that data gathering corresponds with the app's developing goals and key performance metrics.

## 7. Image Storing and Optimization

### Decision 
We have decided to use a combination of server-side caching, lazy loading, and 
image compression techniques for image storage and optimization. 

### Rationale 
Caching images on the server-side helps reduce the load on the server and improves the delivery of images to the app.  
Implementing lazy loading ensures that images are loaded only when they are visible in the user’s viewport, reducing the load time and conserving bandwidth.  
Images may be made smaller without sacrificing much of their quality by using compression techniques like lossless and lossy compression. Users have quicker picture loading times and utilize less data as a result

### Status
Accepted

### Consequences
Advantages: The selected strategy of lazy loading, server-side caching, and picture compression results in quicker image loading, less data use, and increased performance across the board for the app. The software will be more responsive, and users will notice faster image loading times.  
Challenges: Server-side caching, lazy loading, and image compression methods need careful configuration and continual optimization to be implemented and maintained. Furthermore, it is crucial to guarantee that image quality after compression is still acceptable.
