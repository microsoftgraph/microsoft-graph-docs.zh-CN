---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aba75cb97b15253932eda90dbd252fde640f8461
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697656"
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
|cellularTechnology|String|设备的手机网络技术|
|wifiMac|String|设备的 WiFi MAC 地址|
|operatingSystemLanguage|String|设备的操作系统语言|
|isSupervised|Boolean|受监督的设备模式|
|isEncrypted|Boolean|设备的加密状态|
|batterySerialNumber|String|设备的当前电池的序列号|
|batteryHealthPercentage|Int32|设备的当前电池的运行状况百分比。 有效值为 0 至 100|
|batteryChargeCycles|Int32|设备的当前电池已过期的充电周期数。 有效值为0至2147483647|
|isSharedDevice|布尔|共享 iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合|共享 Apple 设备上的所有用户|
|tpmSpecificationVersion|String|指定规范版本的字符串。|
|operatingSystemEdition|String|指定 OS 版本的字符串。|
|deviceFullQualifiedDomainName|String|如果任何) ，则返回设备 (的完全限定域名。 如果设备未加入域，则返回一个空字符串。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|基于虚拟化的安全硬件要求状态。 可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|基于虚拟化的安全状态。 . 可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|本地系统颁发机构 (LSA) credential guard 状态。 . 可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。|
|osBuildNumber|String|Android 设备上的操作系统内部版本号|
|operatingSystemProductType|Int32|指定 Windows 操作系统 ProductType 的 Int。 此处提供了更多详细信息 https://go.microsoft.com/fwlink/?linkid=2126950 。 有效值为0至2147483647|
|ipAddressV4|String|IPAddressV4|
|subnetAddress|String|SubnetAddress|

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
  "operatingSystemProductType": 1024,
  "ipAddressV4": "String",
  "subnetAddress": "String"
}
```





