---
author: joshbax-msft
title: TargetFamily.IsValidTarget Method (TargetData, StringBuilder)
description: TargetFamily.IsValidTarget Method (TargetData, StringBuilder)
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: d4278518-d643-4ccc-942e-dcfbea550f59
---

# TargetFamily.IsValidTarget Method (TargetData, StringBuilder)


This method determines whether the specified TargetData can be a member of this TargetFamily.

**Namespace:** Microsoft.Windows.Kits.Hardware.ObjectModel **Assembly:** Microsoft.Windows.Kits.Hardware.ObjectModel (in Microsoft.Windows.Kits.Hardware.ObjectModel)

## Syntax


**Visual Basic**`Public Function IsValidTarget ( _`           `target As TargetData, _`          `stringBuilder As StringBuilder _``) As Boolean`

**C#**`public bool IsValidTarget (`           `TargetData target,`           `StringBuilder stringBuilder``)`

## Parameters


*target*      Target data to examine.

*stringBuilder*      String builder that contains information on any checks that fail.

## Return Value


Returns **true** if the target can be a member of the target family; otherwise, **false**.

## Remarks


The following conditions determine validity.

1.  The Machine of the target is in the same machine pool as the ProductInstance.

2.  The Machine of the target has the same OS Platform as the ProductInstance (parent) object.

3.  All targets having common manufacturer/VID/Ven.

4.  All targets having common driver hash (of all drivers associated with this device, including any upper and lower filters).

5.  All targets having a common INF hash.

6.  All targets having the same bus/enumerator type.

7.  All targets having the same class/subclass.

8.  If DX capable, same DX major version.

9.  All targets are on unique machines not already part of the TargetFamily. Note that different targets under a product instance are supported on one machine.

10. All targets must be in the running state.

11. Each machine associated with the Target family is running the same version of the OSPlatform as the product instance.

If any of the checks fail, the method returns false.

This specifically allows different Device ID, PID (Product Id) or “Dev” and different sub vendor or implementer Ids.

If the comparison fails, this method populates the event log with additional data.

## Thread Safety


Any public static (**Shared** in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hck\p_hck%5D:%20TargetFamily.IsValidTarget%20Method%20%28TargetData,%20StringBuilder%29%20%20RELEASE:%20%284/27/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")



