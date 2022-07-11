---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09dde616eee8d4740f33499baebcf784967ad93d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670314"
---
# <a name="hardwareinformation-resource-type"></a>hardwareInformation 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|subscriberCarrier|String|设备的订阅服务器运营商|
|cellularTechnology|String|设备的手机网络技术|
|wifiMac|String|设备的 WiFi MAC 地址|
|operatingSystemLanguage|String|设备的操作系统语言|
|isSupervised|Boolean|设备的监督模式|
|isEncrypted|Boolean|设备的加密状态|
|batterySerialNumber|String|设备当前电池的序列号|
|batteryHealthPercentage|Int32|设备当前电池的运行状况百分比。 有效值为 0 至 100|
|batteryChargeCycles|Int32|设备当前电池的充电周期数。 有效值 0 到2147483647|
|isSharedDevice|布尔|共享 iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合|共享 Apple 设备上的所有用户|
|tpmSpecificationVersion|String|指定规范版本的字符串。|
|operatingSystemEdition|String|指定 OS 版本的字符串。|
|deviceFullQualifiedDomainName|String|如果有任何) ，则返回设备 (的完全限定域名。 如果设备未加入域，则返回空字符串。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|基于虚拟化的安全硬件要求状态。 可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|基于虚拟化的安全状态。 . 可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|本地系统颁发机构 (LSA) 凭据防护状态。 . 可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。|
|osBuildNumber|String|Android 设备上的操作系统生成编号|
|operatingSystemProductType|Int32|指定 Windows 操作系统 ProductType 的 Int。 有关详细信息，请参阅此处 https://go.microsoft.com/fwlink/?linkid=2126950。 有效值 0 到2147483647|
|ipAddressV4|String|IPAddressV4|
|subnetAddress|String|SubnetAddress|
|esimIdentifier|String|eSIM 标识符|
|systemManagementBIOSVersion|String|SMBIOS 报告的 BIOS 版本|
|tpmManufacturer|String|唯一命名 TPM 制造商的标识信息|
|tpmVersion|String|由制造商指定的 TPM 版本|
|wiredIPv4Addresses|字符串集合|有线 IPv4 地址的列表。 更新频率 (从设备同步到此属性的云存储) 的属性值更改的最大延迟为每日。 请注意，此属性目前仅在 Windows 上运行的设备上受支持。|
|batteryLevelPercentage|双精度|电池电量在 0.0 到 100 之间，如果电池电量无法确定，则为 null。 此属性的更新频率是按检查。 请注意，此属性目前仅在运行 iOS 5.0 及更高版本的设备上受支持，并且仅在获得设备信息访问权限时才可用。 有效值为 0 至 100|
|residentUsersCount|Int32|此设备上当前的用户数，如果无法确定此属性的值，则为 null (默认) 。 此属性的更新频率是按检查。 请注意，此属性目前仅在运行 iOS 13.4 和更高版本的设备上受支持，并且仅在获得设备信息访问权限时才可用。 有效值 0 到2147483647|
|productName|String|产品名称，例如 iPad8，12 等。此属性的更新频率为每周。 请注意，此属性目前仅在 iOS/MacOS 设备上受支持，并且仅在获得设备信息访问权限时才可用。|
|deviceLicensingStatus|[deviceLicensingStatus](../resources/intune-devices-devicelicensingstatus.md)|基于设备的订阅许可状态。 此属性的更新频率为每日。 请注意，此属性目前仅支持基于 Windows 的基于设备的订阅许可。 如果不支持该值，则该值将设置为未知 (-1) 。 可取值为：`licenseRefreshStarted`、`licenseRefreshPending`、`deviceIsNotAzureActiveDirectoryJoined`、`verifyingMicrosoftDeviceIdentity`、`deviceIdentityVerificationFailed`、`verifyingMirosoftAccountIdentity`、`mirosoftAccountVerificationFailed`、`acquiringDeviceLicense`、`refreshingDeviceLicense`、`deviceLicenseRefreshSucceed`、`deviceLicenseRefreshFailed`、`removingDeviceLicense`、`deviceLicenseRemoveSucceed`、`deviceLicenseRemoveFailed`、`unknownFutureValue`、`unknown`。|
|deviceLicensingLastErrorCode|Int32|指示最后一个错误的标准错误代码，或指示默认)  (没有错误的 0。 此属性的更新频率为每日。 请注意，此属性目前仅支持基于 Windows 的基于设备的订阅许可。 有效值 0 到2147483647|
|deviceLicensingLastErrorDescription|String|错误文本消息作为 deviceLicensingLastErrorCode 的取消订阅。 此属性的更新频率为每日。 请注意，此属性目前仅支持基于 Windows 的基于设备的订阅许可。|

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
  "subnetAddress": "String",
  "esimIdentifier": "String",
  "systemManagementBIOSVersion": "String",
  "tpmManufacturer": "String",
  "tpmVersion": "String",
  "wiredIPv4Addresses": [
    "String"
  ],
  "batteryLevelPercentage": "4.2",
  "residentUsersCount": 1024,
  "productName": "String",
  "deviceLicensingStatus": "String",
  "deviceLicensingLastErrorCode": 1024,
  "deviceLicensingLastErrorDescription": "String"
}
```




