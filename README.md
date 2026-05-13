# DemoExam26
# Instructions for the stand
# Virtual machines
  ```DC1 - DC2 (Windows Server 2019) (NAT,DNS,AD DS)```
  ```Client (Windows 10-11) (client of our "company")```
  ```Ubuntu (Ubuntu Server or Ubuntu Desktop) (Apache/DVWA)```
# Network Settings
  <table>
  <tr>
    <td width="50%" valign="top">
      <strong>DC1</strong><br>
      1Adapter - NAT<br>
      2Adapter - internal network (kit.local)<br>
      ipaddress - 192.168.10.1<br>
      mask - 255.255.255.0<br>
      dns - 127.0.0.1
    </td>
    <td width="50%" valign="top">
      <strong>DC2</strong><br>
      1Adapter - NAT<br>
      2Adapter - internal network (kit.local)<br>
      ipaddress - 192.168.10.2<br>
      mask - 255.255.255.0<br>
      dns - 192.168.10.1
    </td>
  </tr>
  <tr>
    <td valign="top">
      <strong>Client1</strong><br>
      1Adapter - internal network (kit.local)<br>
      ipaddress - auto (DHCP)
    </td>
    <td valign="top">
      <strong>Ubuntu</strong><br>
      1Adapter - internal network (kit.local)<br>
      ipaddress - auto (DHCP)
    </td>
  </tr>
</table>


# Setting up Windows Server (DC1 and DC2) 
First, you need to change the name of the server itself. 

<img width="521" height="100" alt="image" src="https://github.com/user-attachments/assets/ab616365-5165-4bd5-83f7-c7e1485bb9cd" />

  
