---
title: outlookCategory 资源类型
description: 表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。 用户在主列表中定义类别，并可以应用这些用户定义的一个或多个
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 30bed7723cc25b668029bae494a24cbc6c4278fc4caeb6d55f039e65c68e63f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182376"
---
# <a name="outlookcategory-resource-type"></a>outlookCategory 资源类型

命名空间：microsoft.graph


表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。 用户在主列表中定义类别，并且可以将这些用户定义的一个或多个类别应用到项目中。 

使用 REST API，可以在用户类别的主列表中[创建](../api/outlookuser-post-mastercategories.md)和定义类别。 还可以[获取主类别列表](../api/outlookuser-list-mastercategories.md)、[获取特定类别](../api/outlookcategory-get.md)、[更新](../api/outlookcategory-update.md)与类别相关联的颜色，或[删除](../api/outlookcategory-delete.md)类别。 可以通过将类别的 **displayName** 属性分配给项目的 **categories** 集合，将类别应用到项目。
可以为资源分配以下类别：[联系人](contact.md)、[事件](event.md)、[邮件](message.md)和[帖子](post.md)。   

每个类别都有 2 个属性：**displayName** 和 **color**。 **displayName** 值在用户的主列表中必须是唯一的。 然而，**color** 不一定是唯一的；主列表中的多个类别可以映射到相同颜色。 可以在用户的主列表中将多达 25 种不同的颜色映射到类别。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|标识用户邮箱中的类别的唯一名称。 在创建类别后，名称将无法更改。 只读。|
|color|categoryColor|预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。 请参阅下面的备注。 |

> **注意**：**color** 的可能值为预设的常数，如 `None`、`preset0` 和 `preset1`。 每个预设定的常数会被进一步映射到一种颜色；实际颜色取决于显示类别的 Outlook 客户端。 下表显示了 Outlook（桌面客户端）中映射到每个预设常数的颜色。 

| 预设常数  | Outlook 中映射的颜色 |
|:---------------|:--------|
| None | 没有映射的颜色 |
| Preset0 | 红色 |
| Preset1 | 橙色 |
| Preset2 | 褐色 |
| Preset3 | 黄色 |
| Preset4 | 绿色 |
| Preset5 | 青色 |
| Preset6 | 橄榄绿 |
| Preset7 | 蓝色 |
| Preset8 | 紫色 |
| Preset9 | 蔓越橘色 |
| Preset10 | 青灰色 |
| Preset11 | 深青灰 |
| Preset12 | 灰色 |
| Preset13 | 深灰 |
| Preset14 | 黑色 |
| Preset15 | 深红 |
| Preset16 | 暗橙 |
| Preset17 | 深褐 |
| Preset18 | 深黄 |
| Preset19 | 深绿 |
| Preset20 | 深青 |
| Preset21 | 深橄榄色 |
| Preset22 | 深蓝 |
| Preset23 | 深紫 |
| Preset24 | 深蔓越橘色 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List categories](../api/outlookuser-list-mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) 集合 |获取为用户定义的所有类别。|
|[Get category](../api/outlookcategory-get.md) | [outlookCategory](../resources/outlookcategory.md) |获取指定的 **outlookCategory** 对象的属性和关系。|
|[Create](../api/outlookuser-post-mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) |在用户主类别列表中创建 **outlookCategory** 对象。|
|[Update](../api/outlookcategory-update.md) | [outlookCategory](../resources/outlookcategory.md) |更新指定 **outlookCategory** 对象的可写属性 **color**。 |
|[删除](../api/outlookcategory-delete.md) | 无 |删除指定的 **outlookCategory** 对象。 |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->
 

