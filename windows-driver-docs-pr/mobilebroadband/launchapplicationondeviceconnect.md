---
title: LaunchApplicationOnDeviceConnect
description: LaunchApplicationOnDeviceConnect
ms.assetid: d8a5f20a-bd88-4279-9e15-4f20287edfd4
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# LaunchApplicationOnDeviceConnect


The LaunchApplicationOnDeviceConnect element specifies an app that should appear as the recommended AutoPlay action when a user plugs in the device.

## <span id="Usage"></span><span id="usage"></span><span id="USAGE"></span>Usage


``` syntax
<LaunchApplicationOnDeviceConnect>
  child elements
</LaunchApplicationOnDeviceConnect>
```

## <span id="Attributes"></span><span id="attributes"></span><span id="ATTRIBUTES"></span>Attributes


There are no attributes.

## <span id="Child_elements"></span><span id="child_elements"></span><span id="CHILD_ELEMENTS"></span>Child elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[AutoplayHandler](autoplayhandler.md)</p></td>
<td><p>Specifies a Windows Store device app that should appear as the recommended AutoPlay action when a user plugs in a device.</p></td>
</tr>
<tr class="even">
<td><p>[DesktopAutoplayHandler](desktopautoplayhandler.md)</p></td>
<td><p>Specifies a desktop app that should appear as the recommended AutoPlay action when a user plugs in a device.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Parent_elements"></span><span id="parent_elements"></span><span id="PARENT_ELEMENTS"></span>Parent elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[WindowsInfo](windowsinfo.md)</p></td>
<td><p>The parent element of the [WindowsInfo XML schema](windowsinfo-xml-schema.md).</p></td>
</tr>
</tbody>
</table>

 

## <span id="XSD"></span><span id="xsd"></span>XSD


``` syntax
<xs:element name="LaunchApplicationOnDeviceConnect" type ="tns:LaunchApplicationOnDeviceConnectType" />

<xs:complexType name="LaunchApplicationOnDeviceConnectType">
    <xs:choice>
      <xs:element name="AutoplayHandler" type="tns:AutoplayHandlerType" />
      <xs:element name="DesktopAutoplayHandler" type="xs:string" />
      <xs:any namespace="##other" processContents="lax" />
    </xs:choice>
  </xs:complexType>
```

## <span id="Remarks"></span><span id="remarks"></span><span id="REMARKS"></span>Remarks


You must specify either a Windows Store device app or a desktop app. Use [AutoplayHandler](autoplayhandler.md) if you will specify a Windows Store device app, and use [DesktopAutoplayHandler](desktopautoplayhandler.md) if you specify a desktop application.

The LaunchApplicationOnDeviceConnect element is optional.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_mb\p_mb%5D:%20LaunchApplicationOnDeviceConnect%20%20RELEASE:%20%281/18/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




