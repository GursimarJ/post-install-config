<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Installation Configuration</h1>
This walkthrough involves some configuration of the open-source help desk ticketing system osTicket. This builds upon the previous project: osTicket - Prerequisites and Installation.<br />


<h2>Environments Used</h2>

- Microsoft Azure 
- Windows 10
- Windows App (Remote Desktop)

<h2>Technology/Applications/Services </h2>

- osTicket
- Azure Virtual Machines




<h2>Walkthrough</h2>

</br>
<h3 align="center">
  First of all there are 2 important links:
</h3>
</br>

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php
  
![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic1.png)
</p>
<br />
<p>
End Users osTicket URL:
http://localhost/osTicket
  

![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic2.png)
</p>
<br />
<p>
Configure Roles (for grouping permissions)<br />
Admin Panel -> Agents -> Roles<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Supreme Admin

</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic3.png)

<br />



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic4.png)
</p>
<br />
<p>
*Check all in Tickets, Tasks, and Knowledgebase
</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic5.png)

<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic6.png)
</p>
<br />
<p>
Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)<br />
Admin Panel -> Agents -> Departments<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- SysAdmins
</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic7.png)

<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic8.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic9.png)
</p>
<br />
<p>
Configure Teams<br />
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Online Banking

  
</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic10.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic11.png)
</p>
<br />
<p>
Allow anyone to create tickets<br />
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Registration Required: Require registration and login to create tickets 
</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic12.png)
</p>
<br />
<p>
Configure Agents (workers)<br />
Admin Panel -> Agents -> Add New<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- Jane (Dept: SysAdmins)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- John (Dept: Support)

</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic13.png)

<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic14.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic15.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic16.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic17.png)
</p>
<br />



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic18.png)
</p>
<br />
<p>
Configure Users (customers)<br />
Agent Panel -> Users -> Add New<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Karen
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Ken

</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic19.png)
</p>
<br />
<p>
Configure SLA<br />
Admin Panel -> Manage -> SLA<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Sev-A (Grace Period: 1 hour, Schedule: 24/7)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Sev-B (Grace Period: 4 hours, Schedule: 24/7)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Sev-C (Grace Period: 8 hours, Business Hours)

</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic20.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic21.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic22.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic23.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic24.png)
</p>
<br />
<p>
Configure Help Topics (For when users create a ticket)<br />
Admin Panel -> Manage -> Help Topics<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Business Critical Outage<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Personal Computer Issues<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Equipment Request<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Password Reset<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Other
</p>



![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic25.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic26.png)
</p>
<br />




![image alt](https://github.com/GursimarJ/post-install-config/blob/1da6c0122c789f5a1058b0c02fb343b5a0377398/assets/Part2Pic27.png)
</p>
<br />
<br />
<p>
<h3 align="center">
  After this walkthrough, we now have a configuration that allows us to get started in handling user tickets.
  </h3>
</p>

