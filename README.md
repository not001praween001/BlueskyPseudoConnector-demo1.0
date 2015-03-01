Blue-sky cloud connector (Demo v. 1.0)
================================
This is the compatible connecting tester of Blue-sky cloud server. You can use this one to implement your embedded devices connected the Blue-sky cloud server at your local network in another platform that accept java.

The connector uses the Blue-sky connecting wrapping protocol. It is optimized connector that adapts to least connection appoach of Blue-sky load balancer. The protocol is using the light-weight cipher and using the edAccessToken to authenticate the device with the end-user account. The edAccessToken is easily create by a command that decribes in the next section. In order to commpletly access the device, the end-user have to regist the edAccessToken to their account.

**Note:** *This is not including another feature of the Blue-sky*

Getting Start
-------------
- **Clone the git to your embedded devices(ED)**
  ```shell
  git clone https://github.com/not001praween001/BlueskyPseudoConnector-demo1.0.git
  cd BlueskyPseudoConnector-demo1.0/bin
  ```
  
- **Create the edAccessToken**
  ```shell
  # The token message will be encrypted. 
  # Do not use it same as the password of the front site account.
  java EDAccessToken [Input your token message do you want to set]
  cd ..
  ```
  
- **Test the connector**
  ```shell
  ./test.sh
  ```
  
  ***Author***: *Praween AMONTAMAVUT*
  
