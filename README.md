### Assessment Task

DevOps Engineer

**TASK GIVEN: System Provisioning**

1\. Create a small web application to display “Hello GUVI GEEK”.

2\. Push this application to a specific folder of the given GitHub repository.

3\. Create a job in Jenkins and make a build this application.

4\. On Every Commit, It has to Build a pipeline of the Application.

5\. If needed Use Pipeline as a Code, for Building the entire pipeline.

6\. Using Jenkins and Docker Plugin, create an Image of the developed web

application.

7\. Push the Image Finally to the Docker Hub and send the URL image of the

Docker.

Tools Needed : GIT,Jenkins,Docker Hub,AWS EC2 instance(ubuntu)


### Solution

:1.Created java code for the **web application.**

.

![](https://lh3.googleusercontent.com/nIkCO653ej94Fbt_cFRKTGq0qHzTbaEcwTsWwrFnr9r2yOX7h3Q6UZ52I8h-qFCqJhA0dVwNwth3tqeY40yyLego0ViyfXNONp_yWvaMKy5aj23a7ecXyJsiHk7uuwLEPW5JgOthJkoUl6TnKoulN8ev94NkWzKRwJhk5H-1CKwC7ceM1E96iJUErtHvGg)

2.Created **index.html**

**![](https://lh4.googleusercontent.com/-sW-rLt8fyulslQ16Ex8IYmwwpZ92Lt9zWNdmsE9hBau619obeWF0Uy4TfUjRdLbUnUmO6y3Q66Wku-f7YM9on5sqO81AOGT1BKFxeNeFgnwF3p5Haw0vGs2swsei_gpIH8qlu6M8cKXhbsOrbEXTmYMELjrH2pPqxsqHpJnDSiTTQ07X7H4jlYdBID_PA)**

3.Created** Dockerfile**

**![](https://lh4.googleusercontent.com/N4Jzoufg9rkCZOW0MzmW3dODbvZpzdW16tbkMR3jPnOAbLfOGiQmpP0DlSFKAuPzYHkRjooHRVrcySwkn8bOi9jIXTuHPX6THv5emb3Pi7A4WOHzZD0tbqmDQGDRyobnPrDzD-s90GW4IFRVQtTsDMaUAKYpy0cL4dISfbw7hXWaNnO0Y1M1Yp7DE8Bo4g)**

4.Created** jenkins file, **we are using groovy script for executing the commands.

![](https://lh4.googleusercontent.com/zXQzfhmdx_3S2ep_oSFPxttXuifLHUB5lkTkd-Dq7bQxcBy9asQ6prNcpeuBT6xBiUwrbHMM21-uZYM_6XrUbP_YUW0BjPbc66Ws3d0BvKn9CPNVrxiLfbJj2ww_w3O1tLOhGeyKSk2mcLJMi75UvMDWKNpmgm-S5r65LTzS0V-crD37fuwOBosu-NDCRQ)

5.Created **script.groovy**

  


**![](https://lh4.googleusercontent.com/ux5QipXLoM6FEr_PdhBZIvTzAGTq9Q9Py3uknYsLjBRWGS2sNhbTpqI5_2esx__QUtFu9Nj1HMlnpHqtCLDasmaPEs0GsaZJAPEHs71uAdqO6ev3YlpSFRw9RWcS0Bc4xoSL8q1FOsYXRnp1Dd_58CAQBFoZFdc87dDsFCESzZDxXhA83_zBO0uVEHNj-Q)**

  


- In this script three stages there,
- Build jar is to package the maven application
- Build image is to build the docker image and by using the above command. We pushed the code into Docker Hub
- Added docker credentials in the jenkins

  
  
  


**GitHub Repository**

By using git init,git add . ,git commit, git push. We pushed our code to the repository.

![](https://lh5.googleusercontent.com/2Iv-Lv5Wk8HL6ggbc3zwT2_kLYFG5nynu4-8sE2jQQkyFHACSGjlpMpEl4iXQ7hZlI9KS6vPgVRDimLk4gFuiaQrGJRDndupHD9UxMs_KEdUa8OqfLa8FebHnO4l0r1DU-cXLPDpz49KIOdGl7ei-OB2zfWGbYccQQUROY4UjAVnnEQ-uwheLkiM_UOo5Q)

  
  


**Ubuntu instance**

  


1.Created **Ubuntu ec2 instance** with name** kaderguvi.**

  


![](https://lh4.googleusercontent.com/PsXlVIFO1i_-Qov807aVYyXdPknL2C5YTxkhZw_wHuWgCe_BKFGr9v82VxsdqFjMpNN-w87H4dyA63emnbVZ_ZAqJFrpDUyavqQqdvPDoNbA8qZNLdVmN5LKqy3yEHz_OsObp6v096FrQ2LGQlQ9Kx7NhKyJPSdsG5IbMYs8XMYJje5b-4F83PT-W5L8XA)

 

2.choosing **OS image**

 

**![](https://lh5.googleusercontent.com/Gy3DWVBl_8x3LAYWj0Nw9zH5PrevbfctCIzNWwxjRzntNeOxyaAJBaTvjOvupwkiU_2HOxVBFRgHWH3a5GIsxT4Ke9rLkFzGXzYBN1Zc2p38mL2paBIN7uu4_s48uO8FxfxgQv3k9qdaV9-O1lcIqvaG-Ot7KKH3yuectUydXMt8YOXdyhwgYgqzr6G4Fg)**

 

 

As per the task given we selected the os image ubuntu.

Instance name - kaderguvi

 

 

2\. **Instance type** & **key pair**

 

![](https://lh4.googleusercontent.com/rbV5pHws7Xdn7q5b4ymyGNnKHUXWQ5DgeoU2WWZsOZygKLlc8G7kygigdeop8P7XAys3mlg097mBeeL54eoybT6zTLrGt5hxM-Dlg96SgquPpUR0DjCK7sFVsz29BHw9z7z5Zsxg8qayBKyEIiwHHBXV1iTIh2SQhWpmpjeZsPATG1BruoHjkFPnpfmevQ)

- We choose instance type based upon our needs.
- Keypair is used to connect the instance through ssh from out local system.

3\.**Instance** is running

 

![](https://lh4.googleusercontent.com/fApa_yv0Dcmd2irf109RmhCXIfReZBsp6iP1EVxedfA-Clx9_9jv8lDhQlqW_Lk4jDHRa_TfO9s8Tgm6aIJcwU_xL_njaFijnFBIHz4W0e0UwSYq-P_h3UdPwPu5vn6nOMd7wXvjOYD1PTZ3nPrGsW68eC9iDIDzqX3UeoBPFu6cP13Zd2G8X5hgp-wbmg)

 

3.connected instance through the **aws instance connect**

On another way we can connect our instance through ssh in our local system by using the created key pair. 

cmd - **Ssh -i /kader.pem ubuntu@instance public ip**

 

**![](https://lh5.googleusercontent.com/QMyaXEL4d7c01zpZRdnTPIpX6hkAM5lgWQRgPsbbHvThxG60PMMhyoWh8PQraRbxJlEVJTabr4QcYKiQz2xZOe1ledaiDHvxR8JqgHzC4bAFAmo_Sg1yXJfkLQzk4akqD2_l6XVUHNS5mciqAaGSqQ7s_-2XI37n-g5aStrTxecwuoKq6KYbQQ9zD4QbOg)**

 

**Installing jenkins in ubuntu ec2**

1\. First, open a terminal window and update the system package repository by running:

**           sudo apt update**

**![](https://lh5.googleusercontent.com/AUsKHjsJva0Nd1voAW5BA2qTjIJXETrEERRwcetn7OV4n5BF7DYqph1-936vVpl7gWLIJ5fizBF8Oj_r2waTYk7UmNG7WkV_1MPwOe3DMdpzClUbTt8a73cOpmx88G5VIfruvuvOfiY36lkGOQm7n4t8xQCbheEblzcnFfxwH7jCZibpAIk2VdUmYrJKoQ)**

2\. To install OpenJDK 11, run:

         **sudo apt install openjdk-11-jdk -y**

3\. Start by importing the GPG key. The GPG key verifies package integrity but there is no output. Run:

**curl -fsSL https&#x3A;//pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc &amp;gt; /dev/null**

4\. Add the Jenkins software repository to the source list and provide the authentication key

**echo deb \[signed-by=/usr/share/keyrings/jenkins-keyring.asc] https&#x3A;//pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list &amp;gt; /dev/null**

5.Update the system repository one more time. Updating refreshes the cache and makes the system aware of the new Jenkins repository.  

           **sudo apt update**

6.Install Jenkins by running:

**             sudo apt install jenkins -y**

 

 

7.To check if Jenkins is installed and** running**

![](https://lh6.googleusercontent.com/-VoGmR_4SzzS39eucFO4iJqq2aSk7KbbIES1ks1H_HkJjz7KXwqlLObENyOqmkZfHyrVY9efvj4kWBll7r2SmfhUvOCpYxsCav3b0MkMvfM87cmoa_ISWX6AwvVKLNSfU5_MYnJ55TN_tMpKPnxIXCOz8nshofznXlXKCxKD41Ik7gsqAqBc109FUMxUKQ)

**sudo systemctl status jenkins**

Above used to check the status of the jenkins.

8.Install **Docker**,**maven **in EC2 for Docker build.

 **Sudo apt install docker.io**

** Sudo apt install maven**

9\. Opened jenkins port in the **security group**

 

![](https://lh6.googleusercontent.com/te-rcHjCsV8NSykVCw61haKQrkvcqGutLHB_JBomj1sP7rHxBvjwi5bHO-NQyR7F-eb7UJAZ47pB0hMtzEdfJTCEswTq0dS08A5gchwiiNDVNU8-3pEHT2gW3ETjMyQ6qEIpJYxwaxvreFnFFsSGc51dACRvdcnk-0xzzt6Vp_hdqs9KteCEhzVVnPNmeQ)

 

 

It will open the **port 8080**.

And finally we opened **jenkins url page**

 

**![](https://lh6.googleusercontent.com/EKU6FVYo8RHT3S5sdcFLat7cy8dEhjr7TRpPpxVPZR-_0oYZENwqJfx9dLVu09DHLYZdh1v22QESyJTPVs8JTG-4ZRejCmCTtOmehY1rEcaZSL7UtIapWahYwcZZ3md4vi4h75jRvnMx15Iw5MCAX-0Ev3RSLQa59TS--95afeR5BAE98U4OKqHD79xu6A)**

 

 

**Pipeline**

 

1.Created piplelne job **abdulguvi**

 

![](https://lh6.googleusercontent.com/EDsJocLdJ-6iANPjvXb1kWVUHuQVNOR06HJ9OZQGl5p0FyXpnL1EhXwdubpWt3aktxMSJ1VTm4DwTAM9nq4wG0x5oQXr_JQ8iedftpBAZSEH2vVkdrTOgxMDBB1hmsUDcRHel4om7oXMXbyXzh-BgY5Zd0Bk7x4qAkh5KX0g6oSpJsGcXIcnjavPjOhlAQ)

 

2.added **GitHub url** link in the pipeline configuration.

 

![](https://lh5.googleusercontent.com/2D1PdCwY-9wZ-I4eWhemjOHaI5nEJBb68xkEpdzPoBWZJLAIK3m7Q66mFm-Ln3NBoJQoYd_89FAUoNkblG42weDNapu3WmYWhElleIzf-dm3_-MLonbuPWCBxNtnAg8gE7OX1T5VAWpU5qRJD4v45929Ybhs3IQ7ytAE7qJe4u_149mOHPt8kAkhqzPN8w)

 

 

3.To execute jenkins file we have to select **pipeline script from scm**

 

**![](https://lh5.googleusercontent.com/0DpC8GCvPXndDzOJw2wqYlCuVrdc-0umt7CYwK7pAmzMGS73Jcjb0N2O2TAScW9SdaNN6XdHUaJBeijhaLYGmD_vlkIZGDbS0vJBQPxQNM5IWGZkQZ20LfpVmdkHOHhrJfMNIf56OEN6bvKZYYFQ4a2uRneB9SVr23e3AbSe3qn0PyU4GvEeQ5IRPsVGnQ)**

 

 

- Added GitHub url
- Type jenkins in file name
- Renamed the master branch into main

 

4.added **Dcoker hub credentials** in the jenkins 

![](https://lh6.googleusercontent.com/lYPssCKQ271FeZM3KEWKQpJ7tiB1bNEFHTFqXzYU_Y0K6KY-DhP0BWUmiidPQ-bIAWRJ3vrxFjngZg14seSLDJboB9aE54QwvH2NVuv2c_awT6FqoqBZJN5nb8gUNICIenSqX0pmjZUYB2nBKMgu2XNcUGWqS-iFloBfwl-QHTZ338Ral_FdyJQ_SQQOjw)

 

5.run the pipeline by buildnow and **build successfully**.

 

![](https://lh3.googleusercontent.com/Jn9rA8_Fgp9kx0g5blNL1j2FSblvV6fhbLc4Q5T_cXIUevRcnJAew62idaaTJoexVvZF1qSe4dBioHyFOy4wmVFuD0pOvwAXIsVYK_rIx_PM2wr1UxoWDNXvOheMgtG_O29I1-jX9alAYLGJLZogp8qAYv2hu1S5YCjYKMFXgnMkRd50qi-O2VvM6d2i9Q)

 

 

**Docker Hub**

 

![](https://lh5.googleusercontent.com/E-hU2qlZo8FS__wySu4-qexkABUrr0G9XuO3Idr0HDTJkIwxJm8aj3AaLXfUj0hxnUdHaSvfzPMBqlwfOibrsLBs43YRbb2mTu6krXSQJsyLqO8ryr7C_2-v74gTJq9cIy0dt3F8YZvPClRu7Upn05mMYQAvwAB1zrt0cur9TNRhmKum-dJ8jVOFJHkXjg)

 

The above image showing that **new image** is pushed into the Docker Hub

 

And finally we saw the result by running docker image locally

 

![](https://lh5.googleusercontent.com/rkJxnNxSjVvw1TN4bGugBCZXfMvAliB7J61Ad_vIVXi-wGMzcHsnJxJ_B_CgtJaalnZ6qd3KIXGxJoURH7yY3GlErbzJdoPXKjkpFxpxkIajdpatoJIaUpQhrJvpMB4mBmAjoqpNiJZUi-c4gi2SLS2Ii4kxGYZLag6FBszJ1Taf0TupX5uuNK4rdvzrfg)

**Command used : docker run -p 8080:8080 -it abdulkader4513/guvi:latest**

 

 

Checking in the **chrome browser** to see the web page and finally result came as per task given

 

![](https://lh5.googleusercontent.com/P1Z1IfDHfDOOwaA5uhu2q6JgFVxMWmCqDji8Sgzgd_BD7eBb1Ct8eBOqbnDFg5Khnvmx5xbyn7MCAU6NKDmkSVST0Lwe8fz3KXmRuc2RHOs90g37fLdIqGvJvXZoWSBznxmD3UUGLYf8HtTCmlTEtsKfxCZvHhz0XRC-kq08iDT6Hmda_b9bWCaSHuTRFg)

 

 

**Trigger build** automatically in** jenkins** when we make make changes in **GitHub Repo**

1.copy Hook url from the jenkins

2.paste it to the GitHub WebHook payload url

3.it will trigger the pipeline when code changes in GitHub

 

![](https://lh3.googleusercontent.com/4ajNQl2V1hpWTpxZXD_nWUc_yPgEICdj-Ig6JpIehnfJZdta9gDZigQFmgZHMSgMdvQFuOJCe3klajDVKhCDTB4agp-HcWj7AJEx8_lsGuKRMerA1TR4eCoZ2Lj65ELx2O6CnZ6l7gM7l_uCC8OgyMvL_Hxo4svoNtMgm9oWSJeud4dmib0c9g6H6s-qYA)

 Docker Hub url : https://hub.docker.com/repository/docker/abdulkader4513/guvi
 

 
