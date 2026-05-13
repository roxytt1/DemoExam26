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
