# Building a low-cost NAS
[//]: <> (https://paperhive.org/help/markdown)
Building a DIY NAS (Network-Attached Storage) is a fantastic project for anyone looking to centralize their data storage, streamline backups, or create a personal media server. With the ability to customize the hardware and software, a DIY NAS offers flexibility and cost-effectiveness compared to pre-built systems. Combining my technical skills with my passion for DIY projects is exciting, from selecting suitable hard drives to configuring power-efficient components. Plus, with everything stored on a personal server, I can easily access data from anywhere while ensuring privacy and control over my files.

Commercial Off-The-Shelf (COTS) NAS devices can be quite expensive, especially when compared to building your DIY solution. Popular models from brands like Synology or QNAP often come with a hefty price tag, especially as you scale up in storage capacity and advanced features like hardware RAID, encryption, or multi-bay configurations. High-end COTS NAS systems can easily range from $250 to over $2,000, and that's often without the cost of hard drives, which can add hundreds more depending on the desired storage capacity. These pre-built solutions are convenient but can limit customization, meaning you often pay a premium for features you might not need or use. Building your own NAS can offer better value for those comfortable with DIY projects, allowing you to tailor the system to your specific needs at a fraction of the cost.

Considering the cost factor and data safety, I seek to have a NAS supporting 2+ disk spaces for expandability, and I would start by placing two drives, forming a RAID 5 configuration (https://www.asustor.com/en/online/College_topic?topic=352). After a brief survey, I found the 4-Bay COTS products under US$500 can be summarized below: 

## Surveying the market
###### Table 1: Surveyed Sub-USD500 COTS NAS
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#93a1a1;border-spacing:0;}
.tg td{background-color:#fdf6e3;border-color:#93a1a1;border-style:solid;border-width:1px;color:#002b36;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#657b83;border-color:#93a1a1;border-style:solid;border-width:1px;color:#fdf6e3;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-9wq8{border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-nrix{text-align:center;vertical-align:middle}
</style>
<table class="tg"><thead>
  <tr>
    <th class="tg-9wq8">Brand</th>
    <th class="tg-9wq8">Model</th>
    <th class="tg-9wq8">Disk Bays</th>
    <th class="tg-9wq8">Price (USD)</th>
    <th class="tg-nrix">Links</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-9wq8">Synology</td>
    <td class="tg-9wq8">DS-423</td>
    <td class="tg-9wq8">4</td>
    <td class="tg-9wq8">369 + Tax</td>
    <td class="tg-nrix">https://www.bhphotovideo.com/c/product/1767280-REG/synology_diskstation_ds423_4_bay_nas.html</td>
  </tr>
  <tr>
    <td class="tg-9wq8">Synology</td>
    <td class="tg-9wq8">DS-423+</td>
    <td class="tg-9wq8">4</td>
    <td class="tg-9wq8">499 + Tax</td>
    <td class="tg-nrix">https://www.bhphotovideo.com/c/product/1757288-REG/synology_diskstation_ds423_4_bay_nas.html</td>
  </tr>
  <tr>
    <td class="tg-nrix">AsusStor</td>
    <td class="tg-nrix">AS1104T</td>
    <td class="tg-nrix">4</td>
    <td class="tg-nrix">239 + Tax</td>
    <td class="tg-nrix">https://www.bhphotovideo.com/c/product/1652766-REG/asustor_as1104t_drivestor_4_4_bay_nas.html</td>
  </tr>
  <tr>
    <td class="tg-nrix">AsusStor</td>
    <td class="tg-nrix">Drivestor 4 Pro Gen2</td>
    <td class="tg-nrix">4</td>
    <td class="tg-nrix">319 + Tax</td>
    <td class="tg-nrix">https://www.bhphotovideo.com/c/product/1801856-REG/asustor_as3304t_v2_drivestor_2_pro_gen2.html</td>
  </tr>
  <tr>
    <td class="tg-nrix">QNAP</td>
    <td class="tg-nrix">TL-D400s</td>
    <td class="tg-nrix">4</td>
    <td class="tg-nrix">299 + Tax</td>
    <td class="tg-nrix">https://www.bhphotovideo.com/c/product/1556654-REG/qnap_tl_d400s_us_4_bay_desktop_sata_jbod.html</td>
  </tr>
  <tr>
    <td class="tg-nrix">QNAP</td>
    <td class="tg-nrix">TS-433</td>
    <td class="tg-nrix">4</td>
    <td class="tg-nrix">379 + Tax</td>
    <td class="tg-nrix">https://www.bhphotovideo.com/c/product/1722875-REG/qnap_ts_433_4g_us_4_bay_personal_cloud_nas_backup_data.html</td>
  </tr>
</tbody></table>

The lowest-priced NAS mentioned earlier is the AsusStor AS1104T, which costs around $260 including tax. But can I build a solution for a similar price that offers more disk bays, better computing power, and more versatile connectivity? Challenge accepted!

## Selecting the parts
### Case
Inspired by the article [DIY NAS: 2023 Edition](https://blog.briancmoses.com/2023/03/diy-nas-2023-edition.html), I chose the Jonsbo N1 case for my NAS build. It’s ideal for my needs, supporting a Mini-ITX motherboard and a dedicated power supply unit and offering space for six HDD bays—perfect for expanding storage while maintaining a compact footprint. It can be found at US$140 + tax on Amazon, or you can find it at US$85 + US$30 for shipping from JD in China. 

### Motherboard + CPU
TBD

### HDD 
TBD

### Memory 
TBD

### Power Supply Unit
SFX PSU TBD

### NAS Operating System
[TrueNAS](https://www.truenas.com/)

![placeholder picture](../pics/DSC03271.JPG)

###### Table 2: My DIY NAS Components
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-9wq8{border-color:inherit;text-align:center;vertical-align:middle}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 510px"><colgroup>
<col style="width: 90px">
<col style="width: 68px">
<col style="width: 74px">
<col style="width: 49px">
<col style="width: 229px">
</colgroup>
<thead>
  <tr>
    <th class="tg-9wq8">Component</th>
    <th class="tg-9wq8">Model</th>
    <th class="tg-9wq8">Brand</th>
    <th class="tg-9wq8">Price (USD)</th>
    <th class="tg-9wq8">Link</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-9wq8">Case</td>
    <td class="tg-9wq8">N1</td>
    <td class="tg-9wq8">Jonsbo</td>
    <td class="tg-9wq8">110</td>
    <td class="tg-9wq8">https://item.jd.com/10038246252061.html</td>
  </tr>
  <tr>
    <td class="tg-9wq8">Motherboard + CPU</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">Topton</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
  </tr>
  <tr>
    <td class="tg-9wq8">HDD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
  </tr>
  <tr>
    <td class="tg-9wq8">Memory</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
  </tr>
  <tr>
    <td class="tg-9wq8">Power Supply</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
    <td class="tg-9wq8">TBD</td>
  </tr>
</tbody></table>

[To be continued]
