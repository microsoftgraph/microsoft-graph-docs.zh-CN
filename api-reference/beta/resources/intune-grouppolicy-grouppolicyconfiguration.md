---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置的的值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431395"
---
# <a name="grouppolicyconfiguration-resource-type"></a>groupPolicyConfiguration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置实体包含一个或多个组策略定义的配置的的值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)集合|列出属性和[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象之间的关系。|
|[获取 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|读取属性和[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的关系。|
|[创建 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。|
|[删除 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|无|删除[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。|
|[更新 groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。|
|[assign 操作](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|日期和时间创建对象。|
|displayName|String|用户提供的资源对象的名称。|
|说明|String|用户提供的资源对象的说明。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|日期和实体上次修改的时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValues|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合|列表中的启用或禁用配置组策略定义值。|
|assignments|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合|为配置的组分配列表。|

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




