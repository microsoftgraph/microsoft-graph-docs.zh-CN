---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01d62b9c8b777ae4ae2d27e2977e49dd1b5bde487fdf5f3ede45661c3bf20208
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139360"
---
# <a name="grouppolicyconfiguration-resource-type"></a>groupPolicyConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置实体包含一个或多个组策略定义的配置值。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 集合|列出 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象的属性和关系。|
|[获取 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|读取 [groupPolicyConfiguration 对象的属性和](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 关系。|
|[创建 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|创建新的 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象。|
|[删除 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|无|删除 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。|
|[更新 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|更新 [groupPolicyConfiguration 对象](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 的属性。|
|[分配操作](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 集合|尚未记录|
|[updateDefinitionValues 操作](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。|
|displayName|字符串|用户为资源对象提供的名称。|
|description|String|用户提供了资源对象的说明。|
|roleScopeTagIds|String collection|配置的范围标记列表。|
|id|字符串|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValues|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 集合|配置的已启用或已禁用组策略定义值的列表。|
|assignments|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 集合|配置的组分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




