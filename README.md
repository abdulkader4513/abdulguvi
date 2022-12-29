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

1.Created java code for the **web application.**

![](https://lh3.googleusercontent.com/DYO9YQLNwWJqpz35P_uPGwPYX4HG217V540wSkWBAFs0euwejKWyKaR4Zy9RpH3Bq3YE615P8atA-gHkuv9WehLpUd2SWqzoZnmHqyRA6DPf4NE0ORnFz8yX0bRifRF53foOo-TMGjbJTnDaBUv7bXfqgbgMuoSutF1hj2smbtW9k6qbcJiFVvlmbZsWfg)

2.Created **index.html**

**![](https://lh6.googleusercontent.com/rx6tGqkDR9oLjfVh2lbQJJkTUBg9lrKyRrBI2sAPDRFQINSq4Ds_4Mm5aIWsAOpenHKfxv0VKAARSDLDGNu7oLpwrSg1_3AwjVOizufzQCS7BWtZQ3IYx6PS5zqwkyxv8pCCMrbdGjHPeGQDIexqYplfFsI710-7DdZ3Ki23Zat1Z-NoHp49Y3RZw2Esjw)**

3.Created** Dockerfile**

**![](https://lh5.googleusercontent.com/FxiVmxzrinG2FBipO04Rpg83Sz-wDfOR4L8a8iiTzOPxKlPv1pmBvUSKCuD9FGwVzilYUqvh1kwnTJav54i90a3nwM6kr1q38uO5iYStTsx6ki9EC38_R8eWHYlxuft_-WBfhpMfDg91mee93qo4Yv_KjXPRwgu7htgx_F_mUPYCsEy727f71yA53BNwJA)**

4.Created** jenkins file, **we are using groovy script for executing the commands.

![](https://lh3.googleusercontent.com/tClMRW9DQyE5viJ2j6vgL9Pc_I0RBY1BEcxl2BffLUMYM5ewPYumx5d0mgRwvWTbOc9M_KO1UEDiKQMOHp6ypb5MAhn06okQI4nY8tqVMUGQ1e4NK-FOAOUXCVYxkgnfDIdiEw9hD95CDSW4cahyMoBZogWwZDLByjQ_qFyae0r9AdriqRUvQv221PPh9w)

5.Created **script.groovy**

  


**![](https://lh4.googleusercontent.com/66TOoLvmCFyFZApEnw5kyt7JIZlYKyyTvkvrMz1AonZodc8Cxnz6REEQScl_Ip-5Fa3Ka3FZ_c7RexS59dbkkPKOLd70uz-uMOPIXV5ywnmnzNEpwYlkJizzwjWodsw-dLk_oW_qb_8VaWc8zOtjnYKjyA8M70C-E4j9vQ64O8IAF9aHwfFJKfDT1RC0vA)**

  


- In this script three stages are there,
- Build jar is to package the maven application
- Build image is to build the docker image and by using the above command. We pushed the code into Docker Hub
- Added docker credentials in the jenkins

  
  
  


**GitHub Repository**

By using git init,git add . ,git commit, git push. We pushed our code to the repository.

![](https://lh6.googleusercontent.com/IOp5bdb6g2UVEFOFdvrPszyBMCiHkIJ0h7JQpb8Vz2IJK8nB2GCjPaLfuRVCP-yJlSOlsyRYI7ygnmwBjhbSl6zYb0xuBrlZF_PHQxRg_Qosh1aIAasE0i0Ki1i6gWlFD8D6_aohQJ8kBJZ1iQJLriplJFb-6JCJEKuz_VXdQzFwRjn7Mz0su-dmVfq7Rw)

  
  


**Ubuntu instance**

  


1.Created **Ubuntu ec2 instance** with name** kaderguvi.**

  


![](https://lh3.googleusercontent.com/VJRjwQwY3T53ah_GeDEGpDqTR4oKe8kILHRzgSoz9_SI7Eugf27oDRK5FLjFIxsRBfAa8AIEwvjdGTPc3CoWUu6EreAdQ1y9qXCxzODmVChukQ-blHxBCGU70_B3_c0O6Jna3MpG2TeawtXE0ymzPmgrxittJIniqhEYE-G4AyAgTpJF61kfKScp5hqniw)

 

2.choosing **OS image**

 

**![](https://lh4.googleusercontent.com/-M5k4sC3tWUmXWvHgY2O5abzwCWlJNxxa_-8dg6A2VfyruXG6UL1iYoYBYO6_vXxPqIaUJ61iOvxY3yHeONzAsgT9JIbBUm3wL91ka2vGqoK8Qh0FNJBIHz1SbIRSEXd9YhQHZKKCA5KFK9aDRiLtcKV6fYrJ9GmBhgOAF8mE8_1_ggx1nkjni2fu2LciQ)**

 

 

As per the task given we selected the os image ubuntu.

Instance name - kaderguvi

 

 

2\. **Instance type** & **key pair**

 

![](https://lh5.googleusercontent.com/iugY5jZWJmm58pigwtRC1S1X0y8GqMfVGHvYDKLfqZ1cPrgc1J8rShEnxSeQaK4_JqP4MuqTS0-ryKmFYFNXT6JVuirZXPtuOmUgWxS52QvDyL3VDsJ2WNKJXejFCVRKSfT8wyallbjuZNkOwHQNezR8ZxvpCgkf0vExyVebWjd5rv5k0OMKwB5lw165WA)

- We choose instance type based upon our needs.
- Keypair is used to connect the instance through ssh from out local system.

3\.**Instance** is running

 

![](https://lh4.googleusercontent.com/5BtWr6QWLhHXyekGAO2jtIDn833afh4gosX6ENImOAFCckCrVSq9F12CQasY-9lOFTrG-kMHl4h-e_wGYdvR_2N_PXohliNieNjFliCZ4MjJmPjMrZJLJfpfyqBuvK0HBJ8GNbUi_IpQlXo9y8iFAV6QN952z_iTDk5uY8_RAjWSoFc7tBSsoJ5QFlQcSA)

 

4.connected instance through the **aws instance connect**

On another way we can connect our instance through ssh in our local system by using the created key pair. 

cmd - **Ssh -i /kader.pem ubuntu@instance public ip**

 

**![](https://lh3.googleusercontent.com/5kpAFvosZXjctc-BunDKsNsxmeWafHwLu2wLOApMm_eujfygTLYRckQcMg-p3FxBs1e6WXp5BaHuMJXm1O-3a4Ao_3_f2E6iT9HRXeauA5l1k8TJzOyr251pVISyGvbk-wbxupJlf4EAgyVtTgxkIUeKoMKK3mH2VM9c-MZvUSZwvRe7PFOMsQukR90Z_g)**

 

**Installing jenkins in ubuntu ec2**

1\. First, open a terminal window and update the system package repository by running:

**           sudo apt update**

**![](https://lh4.googleusercontent.com/eaOqynoHa5hyi4_YJAFYuORgAZUoKdNxU7EBXGrfVSRFXVVJO4ZWqOV9lCUvVpaaUIo-QG1BOd7P-FO9yuoR_jC9lLH1wLgh-CpSwerU9pGdYR4li0TSvIgPH8RdB5VdK31j2c9wd0QCg67n3ztouUlCNYghUPUmRe5Twd4jAwB1bY_bvml0fyWSvBT9FQ)**

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

![](https://lh6.googleusercontent.com/zDqjouxxycfKIaA5omv3am8Qh1Leym0bacDBhO26EU8Nu5_T5owfO15BBd-olX3hbt_Y9QWQkWdAQA8BUlklT8cJrvYxJUFQjWDxuubL3L6fwSlF7UWjGc-uY8hrT3wXCrxpRtLRL1Zg7FjjIjHerYKeVI1q8PffUqlOJ6ujVfa-gFWWtRkm9J3N2l-1Zw)

**sudo systemctl status jenkins**

Above used to check the status of the jenkins.

8.Install **Docker**,**maven **in EC2 for Docker build.

 **Sudo apt install docker.io**

** Sudo apt install maven**

9\. Opened jenkins port in the **security group**

 

![](https://lh6.googleusercontent.com/OTGtkcY7_fTS8y9IxT_RB36cw5ckCiXi70n4oVHMpRpL3EKvwVv183s-VA9HqwLBD32yBmZ3o6GZg4JZbOZxWuAiF5wSmer7BGRnL_NSDsmxWnGCvSTMCJwVzCNvoxfhZKw5h7R8v_klEqvzqpdGrNnKINQkZaR_LAM61xMuq78-wBRst9wk-g_b5Vc0RQ)

 

 

It will open the **port 8080**.

And finally we opened **jenkins url page**

 

**![](https://lh5.googleusercontent.com/3Vd_y8aSMR7_F27aRl7ZEDXAielFaphpBaVFrSlHr3VOFXCukFX_qaDErraaucGnd21tzyLJ3jsVVtmICv_7pwhpEzPmvyRxJXgYDiDgTiUomFTM4TjzirFb-wGu7iWpSNubX_PJIaDYSUBf5bQ8DBYTnWqU8vaAYtGKGRaxeX19kSYGmJeKLx-7fVXH5Q)**

 

 

**Pipeline**

 

1.Created piplelne job **abdulguvi**

 

![](https://lh6.googleusercontent.com/p2-Bnf83igjCJMgvPtbHHj4XpJ1eXJpiX5y6JZLP010V_bU5SoURTImcvkmbDSooZpfRlA22j11awAg6JXIRzx6K5bivUgtf9IDHbHs7DVE_NC32LO1tFupsnWiYcsROqnv6VnbgjGF56U3INh9sE6OjW_WF8lbl3P5vYzCp2Cj4OI3Ch1obBWzyx0Z61A)

 

2.added **GitHub url** link in the pipeline configuration.

 

![](https://lh6.googleusercontent.com/O4USW8EBuPmPiyK6_IEifyXkUtrzpVdeZRSq9-o5CazvhYLzrcoAQ17MQmVRJV8CaBVJ9ZSoMZmJl0iUNAcnwtm5rjId47sAJyZr79Wd-CFRQ-IzGx1cm437XEvmHz6aLmXozpclQyJoCdujmLWR8x0CcMHpNTgDKHOJF4StzmV2QqV61rO7uhTHc8G0pw)

 

 

3.To execute jenkins file we have to select **pipeline script from scm**

 

**![](https://lh5.googleusercontent.com/9KKsce0n6celwcgYZduKBAT6AT5ZNeip1Qtg05UWiaF-se3sV8fp-jvUrOZcnkZBHdlPmVRMaDXgE8lZa89z5p9jIalezlPyX1_Q3syDWDYH0qNc5ya9wr2OXfencRMNb9FPT0pc7KKL2VXGSNfm3PmnbUMFpEdEK6ae4hLPVFXsLHe6POD0nngyJycCvw)**

 

 

- Added GitHub url
- Type jenkins in file name
- Renamed the master branch into main

 

4.added **Docker hub credentials** in the jenkins 

![](https://lh3.googleusercontent.com/Kn2TcP6psZSP-Xbd8_SJSAP_-p0BgpTRZhpqHFpReqAgMOry2Q1GCaZb-dUn0wMwtYjWpTgPJ-5Jfw_ufpLWE0ktnq68jBLasiFn4sL1QjiNzFFm-pnxcRoGnNoiJoeyPsRzHk8S1jK95FVLVcZ9tRFAW8UDe-o3RpV89zsddJ_atIgM3IuCrUyAIWGppQ)

 

5.run the pipeline by buildnow and **build successfully**.

 

![](https://lh4.googleusercontent.com/R3l6LHnl6oTDgp_R_qEvnBh59mLJ7LYNRPqOouDZykYyZx7gl1wI7mbyay63nn7Ao40wKcBU0Uz0J21O2XJkHiOF8XSubJ9S91b4xgYaa-BMU6WFcLAGjzSxlxWUwV6shH17auXiubU3x9yJ0_YnviYQvyic3I5ow_r9vw_NLkPZ-CQqAuqzIFUGv64Afw)

 

 

**Docker Hub**

 

![](https://lh3.googleusercontent.com/O0PQmakLGzdLv_XRymF-TXz6dIZYuaxnM_yHS05sL5hfKsuYzQj-bOd3SIkrY_z0nE2Q7ydc1pWNHI7sKjsOtK3Bf0lXIiNhaViCR-9lT3Ya49rqwbvgn-ohyJVvnKCUtohTBoYror5j-Vm7F3YIZAqL7mlSCNOqYh1XLT4zj9jSUr-9aQ7gQa4NKk6NvQ)

 

The above image showing that **new image** is pushed into the Docker Hub

 

And finally we saw the result by running docker image locally

 

![](https://lh3.googleusercontent.com/fb3UyyyAdRM3LErth43IIYv1CYUiuk77PY7ECprSyRN0dIo1d4f7TN57BnADJxHJVhPqdFnEwBWoDAM20dObrIUOnh_pEGZ5qr3WTJTSaS4AMxR_gOwnA6LwjvMjvoBGE1grSuzOBJuEF6tT99JjfuDWwZcnicfB55KJyH9Fg8RhFEHGsioL6miFW85rug)

**Command used : docker run -p 8080:8080 -it abdulkader4513/guvi:latest**

 

 

Checking in the **chrome browser** to see the web page and finally result came as per task given

 

![](https://lh4.googleusercontent.com/psRUvWfVvt0I_0dmMPPiGwFfyjLN5qXxlfiTAta_DdnrfWFO7N9NMNIYs7wpEa-ZKYOnGCHJL6G2aR85oJQGminugof572-UHyq_bU8umnIb-t2bmc0USFT-CA8mtH4qDQc4tkzXMXEqcOskT6_QrJZfRlOLaLOduHMTlWIfXkKIVLa6N7R1mMA-dCF-XQ)

 

 

**Trigger build** automatically in** jenkins** when we make make changes in **GitHub Repo**

1.copy Hook url from the jenkins

2.paste it to the GitHub WebHook payload url

3.it will trigger the pipeline when code changes in GitHub

 

![](https://lh4.googleusercontent.com/lGP9yns0IP61AAVUKf5M-wjRR5DWPsjGVOCV5SsEUANT9HSKAZko9wKOgMBcJOPvITCu7LfIXWiZg4iJ7uea_Cda9rna1X2ZXk84OvPwiIU30WXMJHn-kwg0Lue1gHOd_-K0BaFIxmdhFC6l9M3J1sFbz8upqcg9PkShCn9otbZuKSRjU4cmWdabZyBwBw)

 
