# DNS-spoofing-URL-spoofing
# Details of Steps taken 

•	Samples problematic MSISDNS were requested from performance and business continuity teams and high level UGW configuration audit was performed for any possible overlooked scenario. 

•	Few sample numbers were provided by performance team and live tracing was enabled on all of these numbers to capture any possible spoofing case.

•	Traces captured didn't highlight any concrete case of Spoofing.

# Captured Scenario 
•	For ZERO Balance Subscriber, OCS Send Redirection to Landing Page URL

•	User Tries to browse any HTTP URL, and makes a DNS Query, which is allowed to Pass by UGW for the purpose of recharge   

![image](https://github.com/user-attachments/assets/dd7a684b-0cda-4006-a5d4-8039bf3a4763)


![image](https://github.com/user-attachments/assets/88194461-2bb8-4023-9fa7-473ecdf857ad)

•	After Successful DNS, User Initiates HTTP Request that gets redirected to Landing Page URL

![image](https://github.com/user-attachments/assets/fc3bd329-36ca-4dab-9ba3-43eaacfcc45f)

•	User was able to spoof Fraudulent Traffic as DNS Traffic that UGW allowed to Pass through in Redirection  Scenario

![image](https://github.com/user-attachments/assets/1cc27946-b1fe-4a5b-98b9-98085742a89c)

# Solution Implementation
•	Two parameters were identified to stop the ongoing spoofing of DNS and to mitigate the risk of URL spoofing.

![image](https://github.com/user-attachments/assets/1c8c08d1-2248-499c-a612-325faa6df602)


Results of Solution Implementation

•	Significant decrease was observed in L7 DNS Parsing UL/DL Traffic after the SoftPara Change 





