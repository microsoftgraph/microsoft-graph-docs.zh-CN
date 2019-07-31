---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 874cee0b2b09b3d106d771f2c176ceed3d4d04e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999785"
---
# <a name="hardwareinformation-resource-type"></a>hardwareInformation 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的硬件信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|serialNumber|字符串|序列号。|
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
|isSharedDevice|Boolean|共享 iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合|共享 Apple 设备上的所有用户|
|tpmSpecificationVersion|String|指定规范版本的字符串。|
|operatingSystemEdition|String|指定 OS 版本的字符串。|
|deviceFullQualifiedDomainName|String|返回设备的完全限定的域名 (如果有)。 如果设备未加入域, 则返回一个空字符串。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|基于虚拟化的安全硬件要求状态。 可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|基于虚拟化的安全状态。 . 可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|本地系统颁发机构 (LSA) credential guard 状态。 . 可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。|

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
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





