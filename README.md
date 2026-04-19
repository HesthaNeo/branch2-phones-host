<p align="center">
<img width="671" height="210" alt="Screenshot 2026-04-18 192012" src="https://github.com/user-attachments/assets/94888021-38c6-473a-a7ec-4f0ed9bf9544" />
</p>
<h1><u>Milestone 12: Branch 2 Phones & Hosts</u></h1>
    <p>Eleventh phase, we will install Cisco CP-7960 VoIP phones and connect host computers for testing. The Branch 2 VoIP Phones will connect via the HQ Voice Router as no voice services are configured on the Branch 2 router.</p>
    <h2><strong><u>Configuration Steps</u></strong></h2>
    <p><b>Step 1: Connect Two Cisco 7960 VoIP Phones To The Branch 1 Access Switch</b></p>
    <p><b>Step 2: Access The Branch 2 Router CLI And View The DHCP Bindings For Each Phone, Obtaining The MAC-Address Of Each Phone</b></p>
    <p><b>Step 3: On The HQ Voice Router Configure The Two Ephones That Were Just Connected</b></p>
        <p>- A. x3001, x3002</p>
        <p>- B. Ephone 4, Ephone 5</p>
        <p>- C. MAC-Address</p>
        <p>- D. Phone Type</p>
        <p>- E. Button 1</p>
    <p><b>Step 4: Test Dialing By Extension Between Each Branch Phone, To The HQ Phones, And Branch 1 Phones</b></p>
    <p><b>Step 5: Test Outbound Dialing To The PSTN Test Phone 8885551111</b></p>
    <p><b>Step 6: Test Inbound Dialing To B1 External Phone Number(s) <em>(Lab Configuration Not Supported)</em></b></p>
    <p><b>Step 7: Connect Two Hosts To The Branch 2 Switch</b></p>
    <p><b>Step 8: Test Each Host By Pinging Around The Branch 2 Network From Each Host, Between Each Host And To The Headquarters Network And PCs</b></p>
    <p><b>Step 9: Test IP Connectivity To The Internet By Pinging Google Server 8.8.8.8</b></p>
    <p><b>Step 10: Test DNS And Website Connectivity By Using The Web Browser On Each Host To Access Www.Google.Com</b></p>
        <h2><strong><u>Implementation</u></strong></h2>
        <h3>Step 1: Connect Two Cisco 7960 VoIP Phones To The Branch 2 Access Switch</h3>
                <img width="1905" height="936" alt="Screenshot 2026-04-18 194259" src="https://github.com/user-attachments/assets/fa8f85cb-6986-41ea-9596-9816797793b4" />
        <h3>Step 2: Access The Branch 2 Router CLI And View The DHCP Bindings For Each Phone, Obtaining The MAC-Address Of Each Phone</h3>
                <img width="872" height="239" alt="Screenshot 2026-04-18 194451" src="https://github.com/user-attachments/assets/cdcd9c09-d9e0-4b49-96df-d74bc12396c2" />
        <h3>Step 3: On The HQ Voice Router Configure Two Branch 2 Ephone-DNS And The Two Ephones That Were Just Connected</h3>
                <img width="871" height="664" alt="Screenshot 2026-04-18 194816" src="https://github.com/user-attachments/assets/a86302fe-65dd-4504-8457-a5ce21a251db" />
                <img width="868" height="1066" alt="Screenshot 2026-04-18 200412" src="https://github.com/user-attachments/assets/6a014fd5-610d-455f-990c-7a11d60d1534" />
        <h3>Step 4: Test Dialing By Extension Between Each Branch Phone And To The HQ Phones, And Branch 1 Phones</h3>
                <img width="1754" height="883" alt="Screenshot 2026-04-18 200747" src="https://github.com/user-attachments/assets/b37c688a-8713-442b-8c2b-8200d13122c2" />
                <p><em>- We are able to successfully place calls between the branch 2 phones.</em></p>
                <img width="1754" height="869" alt="Screenshot 2026-04-18 200942" src="https://github.com/user-attachments/assets/59f125f9-02fb-475e-a9f4-b9bbdc90aca0" />
                <p><em>- We are able to successfully place calls to the HQ from branch 2.</em></p>
                <img width="1753" height="882" alt="Screenshot 2026-04-18 201105" src="https://github.com/user-attachments/assets/7999069a-e4d2-4005-b6b9-07e9f54e56f9" />
                <p><em>- We are able to successfully place calls to branch 1 from branch 2.</em></p>
        <h3>Step 5: Test Outbound Dialing To The PSTN Test Phone 8885551111</h3>
                <img width="1748" height="882" alt="Screenshot 2026-04-18 201235" src="https://github.com/user-attachments/assets/ab49ccfe-8224-49ff-ac27-e3c47ec81d5d" />
                <p><em>- We are able to successfully place calls to the PSTN.</em></p>
        <h3>Step 6: Test Inbound Dialing To B1 External Phone Number(s) <em>(Lab Configuration Not Supported)</em></h3>
        <h3>Step 7: Connect Two Hosts To The Branch 2 Switch</h3>
                <img width="1875" height="884" alt="Screenshot 2026-04-18 201524" src="https://github.com/user-attachments/assets/2ce3996d-a444-47a4-9564-01933b251538" />
        <h3>Step 8: Test Each Host By Pinging Around The Branch 2 Network From Each Host, Between Each Host And To The Headquarters Network And PCs</h3>
                <img width="866" height="1586" alt="Screenshot 2026-04-18 201911" src="https://github.com/user-attachments/assets/4dd69934-396f-4032-8eda-2cebe052663b" />
                <img width="873" height="1597" alt="Screenshot 2026-04-18 202112" src="https://github.com/user-attachments/assets/e2da0a87-a3a3-45a5-aed8-0f73be34da8a" />
                <p><em>- On both hosts we are able to successfully ping 192.168.30.1 (default gateway), 192.168.10.100 (the HQ-Core Switch Data network gateway at HQ. Also The ping to HQ should initiate the IPSec VPN automatically. This can be confirmed by successful ping replies and also by connecting to the CLI on B2-RTR and running the command “show crypto isakmp sa”.), 192.168.10.50 (the HQ-Server), and both google's DNS server by IP and hostname.</em></p>
        <h3>Step 10: Test DNS And Website Connectivity By Using The Web Browser On Each Host To Access Www.Google.Com</h3>
                <img width="538" height="647" alt="Screenshot 2026-04-18 203041" src="https://github.com/user-attachments/assets/75390712-aff3-489d-8474-7f5906ed3247" />
                <img width="563" height="671" alt="Screenshot 2026-04-18 203118" src="https://github.com/user-attachments/assets/4a01a1d0-6fb8-4ecd-ae0a-5cfecaf5c98d" />
                <p><em>- Successful.</em></p>







 





