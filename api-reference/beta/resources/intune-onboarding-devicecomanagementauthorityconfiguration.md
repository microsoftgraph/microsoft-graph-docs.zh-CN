---
title: deviceComanagementAuthorityConfiguration 资源类型
description: Windows 10 Co-Management颁发机构页面配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3314c33a80aaf4c922e22a88b3536f0012cfe95
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793794"
---
# <a name="devicecomanagementauthorityconfiguration-resource-type"></a>deviceComanagementAuthorityConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10 Co-Management颁发机构页面配置


继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComanagementAuthorityConfigurations](../api/intune-onboarding-devicecomanagementauthorityconfiguration-list.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 集合|列出 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性和关系。|
|[获取 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-get.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|读取 [deviceComanagementAuthorityConfiguration 对象的属性和](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 关系。|
|[创建 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-create.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|创建新的 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象。|
|[删除 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-delete.md)|无|删除 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)。|
|[更新 deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-update.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|更新 [deviceComanagementAuthorityConfiguration 对象](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|字符串|设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|字符串|设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|如果用户位于分配了注册配置的多个组中，则使用优先级。 用户仅受优先级值最低的配置使用。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|字符串集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|managedDeviceAuthority|Int32|CoManagement Authority 配置 ManagedDeviceAuthority|
|installConfigurationManagerAgent|布尔值|CoManagement Authority 配置 InstallConfigurationManagerAgent|
|configurationManagerAgentCommandLineArgument|String|CoManagement Authority 配置配置ManagerAgentCommandLineArgument|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|设备配置文件的组分配列表 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

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
  "managedDeviceAuthority": 1024,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "String"
}
```



