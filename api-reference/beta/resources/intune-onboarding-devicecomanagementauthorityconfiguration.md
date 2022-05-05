---
title: deviceComanagementAuthorityConfiguration 资源类型
description: Windows 10 Co-Management颁发机构页面配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae2f690a1e1ee10c606eeb7c880be2152cd45951
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210232"
---
# <a name="devicecomanagementauthorityconfiguration-resource-type"></a>deviceComanagementAuthorityConfiguration 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10 Co-Management颁发机构页面配置


继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComanagementAuthorityConfigurations](../api/intune-onboarding-devicecomanagementauthorityconfiguration-list.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 集合|列出 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性和关系。|
|[获取 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-get.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|读取 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性和关系。|
|[创建 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-create.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|创建新的 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象。|
|[删除 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-delete.md)|无|删除 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)。|
|[更新 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-update.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|更新 [deviceComanagementAuthorityConfiguration 对象的](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的帐户的唯一标识符|
|displayName|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的显示名称|
|说明|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配了注册配置的多个组中时，将使用优先级。 用户仅受优先级最低的配置的约束。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|在 UTC 中创建的设备注册配置的日期时间继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的 UTC 中上次修改的日期时间|
|version|Int32|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的版本|
|roleScopeTagIds|字符串集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|支持从 [deviceEnrollmentConfiguration 继承的](../resources/intune-shared-deviceenrollmentconfiguration.md)注册配置类型。 可能的值是：`unknown`、`limit`、`platformRestrictions`、`windowsHelloForBusiness`、`defaultLimit`、`defaultPlatformRestrictions`、`defaultWindowsHelloForBusiness`、`defaultWindows10EnrollmentCompletionPageConfiguration`、`windows10EnrollmentCompletionPageConfiguration`、`deviceComanagementAuthorityConfiguration`、`singlePlatformRestriction`、`unknownFutureValue`、`enrollmentNotificationsConfiguration`。|
|managedDeviceAuthority|Int32|CoManagement Authority 配置 ManagedDeviceAuthority|
|installConfigurationManagerAgent|Boolean|CoManagement Authority 配置 InstallConfigurationManagerAgent|
|configurationManagerAgentCommandLineArgument|字符串|CoManagement Authority 配置 ConfigurationManagerAgentCommandLineArgument|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备配置文件的组分配列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComanagementAuthorityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "deviceEnrollmentConfigurationType": "String",
  "managedDeviceAuthority": 1024,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "String"
}
```




