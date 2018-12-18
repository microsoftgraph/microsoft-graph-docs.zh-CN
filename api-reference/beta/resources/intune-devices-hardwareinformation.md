---
title: hardwareInformation 资源类型
description: 硬件的给定设备的信息。
author: tfitzmac
ms.openlocfilehash: c483aa800d920a50392d21c326cd20dea7b72e18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334522"
---
# <a name="hardwareinformation-resource-type"></a>hardwareInformation 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

硬件的给定设备的信息。
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
|subscriberCarrier|String|订阅者运营商的设备|
|cellularTechnology|字符串|移动电话的设备的技术|
|wifiMac|字符串|设备的 WiFi MAC 地址|
|operatingSystemLanguage|字符串|设备的操作系统语言|
|isSupervised|Boolean|设备监管的模式|
|isEncrypted|Boolean|设备加密状态|
|isSharedDevice|Boolean|共享的 iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合|共享的 Apple 设备上的所有用户|
|tpmSpecificationVersion|字符串|指定规范版本的字符串。|
|operatingSystemEdition|字符串|指定的操作系统版本的字符串。|
|deviceFullQualifiedDomainName|字符串|（如果有），则返回设备的完全限定的的域名。 如果设备不加入域的它将返回空字符串。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|虚拟化基于安全硬件要求状态。 可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|虚拟化基于安全状态。 . 可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other`。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|本地系统证书颁发机构 (LSA) 凭据 guard 状态。 . 可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。|

## <a name="relationships"></a>Relationships
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





