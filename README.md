# ecs-project-2-p0-solved
**TO GET THIS SOLUTION VISIT:** [ECS Project 2 P0 Solved](https://www.ankitcodinghub.com/product/ecs-p0-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;124842&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECS Project 2 P0 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Socket Programming:

Domain Name System (DNS)

Project 2 (100 points)

Team: The project is to be done in a team of at most 2 students. You cannot discuss your code/data with other classmates (except your project partner).

In this project you will implement Domain Name System (DNS) client and server from scratch using the socket API. Add

Domain Name System (DNS)

There are two ways to identify a host—by a hostname and by an IP address. People prefer the more mnemonic hostname identifier, while routers prefer fixed-length, hierarchically structured IP addresses. In order to reconcile these preferences, we need a directory service that translates hostnames to IP addresses. This is the main task of the Internet’s Domain Name System (DNS). The DNS is:

1. a distributed database implemented in a hierarchy of DNS servers, and

2. an application-layer protocol that allows hosts to query the distributed database.

Resolving DNS Queries

In order for a host to be able to send an HTTP request message to a Web server – say www.ucdavis.edu – it must first obtain the IP address of www.ucdavis.edu. This is usually done as follows:

1. An application layer program (such as a web browser which is the client side of the DNS server) contacts a local DNS server known as a resolver ((1) in Figure 1). The resolver maintains a cache of recently translated addresses. If the cache contains the address for the requested hostname, the resolver can return the answer immediately.

2. For hostnames that are not in the cache, the resolver would then need to traverse the distributed DNS infrastructure. The first point of contact is a root DNS server. Root servers typically have a static IP address (e.g., a.root-servers.net currently uses 198.41.0.4). These IP addresses serve as the entry point to the distributed DNS infrastructure. Local DNS resolver sends a DNS query to a root server to get the IP address of the TLD server ((2) in Figure 1).

3. After getting the IP address of the TLD server ((3) in Figure 1), the DNS resolver would then send a query to the TLD DNS server requesting the address of the authoritative DNS server ((4) in Figure 1).

4. After getting the address of the authoritative DNS server ((5) in Figure 1), the DNS resolver would then send a request to the authoritative DNS server ((6) in Figure 1) and in response it would receive the IP address of the initially requested hostname ((7) in Figure 1).

5. The application eventually receives a reply from the local DNS server, which includes the IP address for the requested hostname((8) in Figure 1).

6. Once you find the IP address, initiate a TCP connection to the IP address at port 80 at that using socket API. You need to craft and send a HTTP GET request using socket API. The standard format of the HTTP message is explained in page 101-103 of the textbook. You

can see this example of how to create an HTTP request on port 80. After getting the

response from the HTTP server, save it as an HTML file. Upload this file along with your

code.

Note: Because most of the sites these days are HTTPS only, sending an HTTP GET request to those sites will result in a 301 redirect page being shown. This is normal and expected behavior.

Understanding DNS request and response structure using Wireshark

You can use Wireshark to understand the structure of a simple DNS request and response. To see the structure of a DNS request on your local computer, open your wireshark, and start capturing network traffic.

Then, open a terminal and use dig to resolve the IP address of a web page. For example:

dig youtube.com @8.8.8.8

This command basically sends a dns query to one of the DNS resolvers with IP address 8.8.8.8. As soon as you push the enter, you will see the resolved IP address in ANSWER SECTION which is 142.250.189.174:

Add

Now, if you stop the Wireshark and filter DNS packets, you will see the list of DNS requests and responses. The size of the DNS response is usually more than the DNS request because it includes the answers to the query. You can select the DNS packets and investigate their structure as follows.

Note how this structure follows the format of a DNS message explained in Section 4 of RFC

1035, A. Implement DNS Client (30 pints)

In the first part of the project, you will implement a DNS Client ((1&amp;8) in Figure 1). The client should send a DNS request to the IP address of three different DNS resolvers provided in Table 1 to query tmz.com. After getting the IP address of the tmz.com’s web server, we ask that you initiate a TCP connection to the HTTPs server process located at port 80 at that IP address.

IP Location

91.245.229.1 Alternative:

46.224.1.42

185.161.112.34 Iran

169.237.229.88 Alternative: 168.62.214.68

104.42.159.98https:// ent Project Exam HelpUSA

136.159.85.15 Alternative:

184.94.80.170

142.103.1.1 Canada Add

Table 1: IP address of three DNS resolvers located in different regions

Workflow of your program (15 pints):

Your DNS client should follow this sequence:

1. Build a DNS query.

a. Build your DNS request, according to RFC 1035, Section 4. Pack DNS header and query in a payload buffer.

2. UDP Socket Calls

a. After your DNS request payload is built, use sendto() and recvfrom() to send and receive from the public DNS resolvers provided in Table 1. Note that DNS uses UDP port 53.

b. If you don’t get a response within 10 seconds, try another IP address from the alternative section of Table 1 in the same region.

3. Receive the response per request from the DNS server

a. When you receive your response from the call to recvfrom(), you will have to unpack the response.

Hint: Since the header is always the first 12 bytes of your response, you should unpack the header first.

4. Parse response message: Now that you have unpacked and parsed the response header, you can parse the rest of the Resource Records (RRs) in the Answer section of the response, to figure out the type of the DNS record and the IP address. Print out this IP address along with the corresponding domain name in the output.

5. Returning the resolved IP address for an A record: Once you find the IP address, initiate a TCP connection to the IP address at port 80 at that using socket API. You need to craft and send a HTTP GET request using socket API. The standard format of the HTTP message is explained in page 101-103 of the textbook. You can see this example of how to create an HTTP request on port 80. After getting the response from the HTTP server, save it as an HTML file. Upload this file along with your code.

Note: Because most of the sites these days are HTTPS only, sending an HTTP GET request to those sites will result in a 301 redirect page being shown. This is normal and expected behavior.Add

Report Details:

1. Describe in detail the DNS request and response header format in your implementation. (5 points)

2. Compute the RTT between your DNS client to each of the public DNS resolvers. Do you notice any meaningful differences across different DNS resolvers? Explain. (5 points)

3. Compute the RTT between your HTTP client to the HTTP server of the resolved hostname. (5 points) B. Implement DNS Server (40 points)

In the second part of the project, you will implement the local DNS resolver using the socket

API to find the IP address of tmz.com. You will implement the iterative strategy to resolve input DNS queries by consulting the root name server, the TLD name server, and finally the authoritative DNS server to get the IP address of the requested hostname.

Workflow of your program (30 points):

Roughly, your server should follow this sequence:

1. Build a DNS query.

a. Build your DNS request, according to RFC 1035, Section 4. Pack DNS header and query in a payload buffer.

3. UDP Socket Calls

b. After your request is built you will need to use sendto() and recvfrom() to send and receive from the server. DNS uses UDP port number 53.

c.Send that query to one of the root servers (the IP address of root servers are

provided in Table 2) and wait for a response. If you wait too long, move to the next root.

4. Receive responses per request from the DNS server hierarchy: When you receive your response from the call to recvfrom(), you will have to unpack the response.

5. Parse response messageAdd : Now that you have your response headers, you can parse the rest of the Resource Record in the response, to figure out the type of the DNS record.

6. Continue this process as you work your way down the DNS hierarchy. In the process of parsing responses from root server and TLD server, check the Resource Records (RRs) in the Additional sections of the DNS response. Print out the IP address of each of the DNS servers you are calling.

7. Returning the resolved IP address for an A record: Once your DNS server has received the IP address from the authoritative name server, return it to your DNS client.

Report Details:

1. Compute the RTT from your local DNS server to each of the DNS servers including the root name server, the TLD name server, and the authoritative DNS server of tmz.com. (10 points)

a.root-servers.net 198.41.0.4, 2001:503:ba3e::2:30

b.root-servers.net 199.9.14.201, 2001:500:200::b

c.root-servers.net 192.33.4.12, 2001:500:2::c

d.root-servers.net 199.7.91.13, 2001:500:2d::d

e.root-servers.net 192.203.230.10, 2001:500:a8::e

f.root-servers.net 192.5.5.241, 2001:500:2f::f

g.root-servers.net 192.112.36.4, 2001:500:12::d0d

h.root-servers.netAssignment Project Exam

Help198.97.190.53, 2001:500:1::53

i.root-servers.net 192.36.148.17, 2001:7fe::53

2001:503:c27::2:30

k.root-servers.net 193.0.14.129, 2001:7fd::1

l.root-servers.net 199.7.83.42, 2001:500:9f::42

2001:dc3::35

Table 2: List of Root Servers C. Implement DNS Server with Caching (30 points)

In the third part of the project, you are asked to implement a cache for your local DNS server. Before implementing the cache, use your implemented local DNS server to send DNS requests to resolve the following host names.

● youtube.com

● facebook.com

● tmz.com

● nytimes.com ● cnn.com

1. Report the time it takes to resolve each of these host names from your local DNS server. (5 points)

the transaction in progress, and should not be cached.”

2. Report the TTL value in the DNS responses to each of these host names. (5 points)

Next, implement a cache in your local DNS server. If a DNS client sends a DNS query to yourAdd local DNS server for one of the host names, the local DNS server should check its cache before sending any request to the root DNS server. If the answer is in the cache and the TTL is not expired, return the response directory from the cache. If it is expired, remove it from the cache and contact the root DNS server to start the resolution process. (15 points)

3. Report the time it takes to resolve each of these host names by your DNS client from your local DNS server when it did implement the cache (and the answers are already in the cache). (5 points) Report:

report_[name1]_[student_id1]_[name2]_[student_id2].pdf

At the beginning of the page, specify the following:

1. Full Name of student 1 (Student ID) (Discussion Group)

2. Full name of student 2 (Student ID) (Discussion Group)

3. Name of the submitted code

Uploads:

Please upload the source code for each part separately:

PartB_[name1]_[student_id1]_[name2]_[student_id2].py

PartC_[name1]_[student_id1]_[name2]_[student_id2].py

You need to upload a txt file including the HTTP response for Part A:

Partb_http_[name1]_[student_id1]_[name2]_[student_id2].txt

We should be able to run your code using the command line by providing the name of the source code file and a domain name. For example to know the IP address of facebook.com using your implemented local DNS resolver we should see the IP address in the output using this command line:

powcodere1]_[student_id1]_[name2]_[student_id2].py facebook.com

The expected output is:

Domain: facebook.com

HTTP Server IP address: X.X.X.X (depends on the response from the Authoritative DNS server)

Python3 PartB_[name1]_[student_id1]_[name2]_[student_id2].py facebook.com

The expected output is:

Domain: facebook.com

Root server IP address: 198.41.04

TLD server IP address: X.X.X.X (depends on the response from the root server) Authoritative server IP address: X.X.X.X (depends on the response from the TLD DNS server)

HTTP Server IP address: X.X.X.X (depends on the response from the Authoritative DNS server) Testing Environment:

All submissions will be tested on Python 3+.

𝑦𝑜𝑢 𝑔𝑒𝑡 = (𝐴𝑐𝑡𝑢𝑎𝑙 𝑀𝑎𝑟𝑘𝑠 𝑦𝑜𝑢 𝑤𝑜𝑢𝑙𝑑 𝑔𝑒𝑡 𝑖𝑓 𝑁𝑂𝑇 𝑙𝑎𝑡𝑒) × ⎡⎢⎣1 unless you− ℎ𝑜𝑢𝑟𝑠24 𝑙𝑎𝑡𝑒 ⎤⎥⎦

have our prior permission or documented accommodation.

Add
