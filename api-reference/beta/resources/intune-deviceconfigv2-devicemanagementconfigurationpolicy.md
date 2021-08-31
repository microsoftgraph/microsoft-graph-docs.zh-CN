---
title: deviceManagementConfigurationPolicy 资源类型
description: 设备管理配置策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 26cd4f91cfaa0a28c3d13f26fd5764d571c47ce4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792587"
---
# <a name="devicemanagementconfigurationpolicy-resource-type"></a>deviceManagementConfigurationPolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备管理配置策略

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationPolicies](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-list.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 集合|列出 [deviceManagementConfigurationPolicy 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 关系。|
|[获取 deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-get.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|读取 [deviceManagementConfigurationPolicy 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 关系。|
|[创建 deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-create.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|创建新的 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。|
|[删除 deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-delete.md)|无|删除 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)。|
|[更新 deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-update.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|更新 [deviceManagementConfigurationPolicy 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 的属性。|
|[分配操作](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-assign.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合|尚未记录|
|[createCopy 操作](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-createcopy.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略文档的键。 自动生成。|
|name|String|策略名称|
|description|字符串|策略说明|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|此策略的平台。 可能的值是：`none`、`macOS`、`windows10X`、`windows10`。|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|此策略的技术。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`、`exchangeOnline`。|
|createdDateTime|DateTimeOffset|策略创建日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|策略上次修改日期和时间。 此属性是只读的。|
|settingCount|Int32|设置数。 此属性是只读的。|
|creationSource|String|策略创建源|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|
|isAssigned|Boolean|策略分配状态。 此属性是只读的。|
|templateReference|[deviceManagementConfigurationPolicyTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplatereference.md)|模板参考信息|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settings|[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 集合|策略设置|
|assignments|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合|策略分配|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "platforms": "String",
  "technologies": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "settingCount": 1024,
  "creationSource": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "String",
    "templateFamily": "String",
    "templateDisplayName": "String",
    "templateDisplayVersion": "String"
  }
}
```



