---
title: System Audio - Audio Logo Test - Glitch
description: System Audio - Audio Logo Test - Glitch
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 54b23258-a8b5-4074-8a51-902e232ebca5
author: EliotSeattle
ms.author: EliotSeattle
ms.date: 10/15/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# <span id="p_hlk_test.7e0233fb-ab35-4a1b-9cce-badc6cbe9421"></span>System Audio - Audio Logo Test - Glitch

>[!IMPORTANT]
>  
This test requires supplemental content. You can find this content in the 'Windows HLK supplemental test content' section at the following location:

-   <http://go.microsoft.com/fwlink/p/?LinkId=532718>

 

Parameter: \[WDKDeviceID\] - set this parameter to device ID when scheduling from Job Explorer for private testing Please refer to WDK documentation for details about this test!

## Test details
|||
|---|---|
| **Specifications**  | <ul><li>System.Fundamentals.SystemAudio.Audio</li></ul> |  
| **Platforms**   | <ul><li>Windows 10, client editions (x86)</li><li>Windows 10, client editions (x64)</li><li>Windows Server 2016 (x64)</li><li>Windows 10, client editions (ARM64)</li></ul> |
| **Supported Releases** | <ul><li>Windows 10</li><li>Windows 10, version 1511</li><li>Windows 10, version 1607</li><li>Windows 10, version 1703</li><li>Windows 10, version 1709</li></ul> |
|**Expected run time (in minutes)**| 2 |
|**Category**| Benchmark |
|**Timeout (in minutes)**| 120 |
|**Requires reboot**| false |
|**Requires special configuration**| true |
|**Type**| automatic |

 

## <span id="Additional_documentation"></span><span id="additional_documentation"></span><span id="ADDITIONAL_DOCUMENTATION"></span>Additional documentation


Tests in this feature area might have additional documentation, including prerequisites, setup, and troubleshooting information, that can be found in the following topic(s):

-   [System.Fundamentals additional documentation](system-fundamentals-additional-documentation.md)

## <span id="More_information"></span><span id="more_information"></span><span id="MORE_INFORMATION"></span>More information


### <span id="Parameters"></span><span id="parameters"></span><span id="PARAMETERS"></span>Parameters

| Parameter name         | Parameter description                   |
|------------------------|-----------------------------------------|
| **WDKDeviceID**        | Device ID string                        |
| **LLU\_NetAccessOnly** | Name of machine's LLU for copying files |
| **TestPro**            | Test Case Profile String                |

 

## <span id="Troubleshooting"></span><span id="troubleshooting"></span><span id="TROUBLESHOOTING"></span>Troubleshooting


For generic troubleshooting of HLK test failures, see [Troubleshooting Windows HLK Test Failures](..\user\troubleshooting-windows-hlk-test-failures.md).

 

 






