---
title: aospDeviceOwnerPkcsCertificateProfile 资源类型
description: AOSP 设备所有者 PKCS 证书配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f994f864e4c3a0fa37e81b361587d7474ac1357c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63378758"
---
# <a name="aospdeviceownerpkcscertificateprofile-resource-type"></a>aospDeviceOwnerPkcsCertificateProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AOSP 设备所有者 PKCS 证书配置文件


继承自 [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 aospDeviceOwnerPkcsCertificateProfiles](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-list.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) 集合|列出 [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) 对象的属性和关系。|
|[获取 aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-get.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|读取 [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) 对象的属性和关系。|
|[创建 aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-create.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|创建新的 [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) 对象。|
|[删除 aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-delete.md)|无|删除 [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)。|
|[更新 aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-update.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|更新 [aospDeviceOwnerPkcsCertificateProfile 对象](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|certificationAuthority|String|PKCS 证书颁发机构|
|certificationAuthorityName|String|PKCS 证书颁发机构名称|
|certificationAuthorityType|[deviceManagementCertificationAuthority](../resources/intune-deviceconfig-devicemanagementcertificationauthority.md)|证书颁发机构类型。 可取值为：`notConfigured`、`microsoft`、`digiCert`。|
|certificateTemplateName|字符串|PKCS 证书模板名称|
|subjectAlternativeNameFormatString|String|定义属性的自定义AAD字符串。|
|subjectNameFormatString|String|要与 SubjectNameFormat 一同使用的自定义格式 = Custom。 示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|目标存储证书。 可取值为：`user`、`machine`。|
|customSubjectAlternativeNames|[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合|自定义主题备用名称设置。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 集合|设备的证书状态。 此集合最多可包含 2147483647 元素。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aospDeviceOwnerPkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerPkcsCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificationAuthorityType": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String",
  "subjectNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ]
}
```




