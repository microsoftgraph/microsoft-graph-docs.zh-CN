---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43f0f9970a3d94285d1abe06c86eff83f2bed818
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331530"
---
# <a name="grouppolicyconfiguration-resource-type"></a>groupPolicyConfiguration 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置实体包含一个或多个组策略定义的配置值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)集合|列出[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。|
|[获取 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|读取[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。|
|[创建 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。|
|[删除 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|无|删除[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。|
|[更新 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。|
|[分配操作](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。|
|displayName|String|用户提供的资源对象的名称。|
|说明|String|用户提供的资源对象的说明。|
|id|字符串|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValues|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合|配置的启用或禁用组策略定义值的列表。|
|assignments|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合|配置的组分配的列表。|

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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



