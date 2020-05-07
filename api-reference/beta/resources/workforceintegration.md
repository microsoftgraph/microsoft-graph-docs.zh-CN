---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d32d3f665a8ea22ac4374df794031caaa9fa1964
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154071"
---
# <a name="workforceintegration-resource-type"></a>workforceIntegration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

员工的一个实例与倒班的集成。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/workforceintegration-list.md) | [workforceIntegration](workforceintegration.md)集合 | 获取与此计划关联的**workforceIntegration**对象的列表。|
| [创建](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | 创建新的**workforceIntegration**对象。|
| [获取](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | 读取**workforceIntegration**对象的属性和关系。 |
| [更新](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | 更新**workforceIntegration**对象。 |
| [删除](../api/workforceintegration-delete.md) | None | 删除**workforceIntegration**对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|apiVersion|Int32|回调 URL 的 API 版本。 从1开始。|
|displayName|String|劳动力集成的名称。|
|技术|[workforceIntegrationEncryption](workforceintegrationencryption.md)|劳动力集成加密资源。|
|isActive|布尔值|指示此劳动力集成当前是否处于活动状态且可用。|
|支持|string| 移位支持同步更改通知的实体。 班次将回拨到在此处添加的这些实体上的客户端更改上提供的 url。 默认情况下，不支持更改通知的任何实体。 可能的值为`none`： `shift`、 `swapRequest`、 `openshift` `openShiftRequest`、、`userShiftPreferences`|
|supportedEntities|string| 此属性将替换1.0 版中的**支持**。 建议使用此属性，而不**支持**。 **支持**属性将在 beta 中仍受支持。 可能的值`none`为`shift`、 `swapRequest` `openshift` `openShiftRequest`、、、 `userShiftPreferences`。 如果选择多个值，则所有值必须以大写形式的第一个字母开头。|
|url|String| 来自倒班服务的回调的劳动力集成 URL。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supports": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
