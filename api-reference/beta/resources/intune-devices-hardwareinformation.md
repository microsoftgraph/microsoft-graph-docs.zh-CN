---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2875ea3a4f8ba7bd00b2a1095ecaf496c36e5ef6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081389"
---
# <a name="hardwareinformation-resource-type"></a>hardwareInformation 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的硬件信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|serialNumber|String|序列号。|
|totalStorageSpace|Int64|设备的总存储空间。|
|freeStorageSpace|Int64|设备的可用存储空间。|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|设备的制造商|
|model|String|设备的型号|
|phoneNumber|String|设备的电话号码|
|subscriberCarrier|String|设备的订阅者运营商|
|cellularTechnology|字符串|设备的手机网络技术|
|wifiMac|字符串|设备的 WiFi MAC 地址|
|operatingSystemLanguage|字符串|设备的操作系统语言|
|isSupervised|Boolean|受监督的设备模式|
|isEncrypted|Boolean|设备的加密状态|
|batterySerialNumber|字符串|设备的当前电池的序列号|
|batteryHealthPercentage|Int32|设备的当前电池的运行状况百分比。 有效值为 0 至 100|
|batteryChargeCycles|Int32|设备的当前电池已过期的充电周期数。 有效值为0至2147483647|
|isSharedDevice|布尔|共享 iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合|共享 Apple 设备上的所有用户|
|tpmSpecificationVersion|字符串|指定规范版本的字符串。|
|operatingSystemEdition|字符串|指定 OS 版本的字符串。|
|deviceFullQualifiedDomainName|字符串|如果任何) ，则返回设备 (的完全限定域名。 如果设备未加入域，则返回一个空字符串。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|基于虚拟化的安全硬件要求状态。 可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|基于虚拟化的安全状态。 . 可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|本地系统颁发机构 (LSA) credential guard 状态。 . 可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。|
|osBuildNumber|字符串|Android 设备上的操作系统内部版本号|
|operatingSystemProductType|Int32|指定 Windows 操作系统 ProductType 的 Int。 此处提供了更多详细信息 https://go.microsoft.com/fwlink/?linkid=2126950 。 有效值为0至2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "batterySerialNumber": "String",
  "batteryHealthPercentage": 1024,
  "batteryChargeCycles": 1024,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String",
  "operatingSystemProductType": 1024
}
```






