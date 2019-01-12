---
title: messageRule 资源类型
description: 适用于用户收件箱邮件的规则。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86fa0edd5bf24be6e8b18fe648b6cffa505d0a7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931072"
---
# <a name="messagerule-resource-type"></a>messageRule 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

适用于用户收件箱邮件的规则。

在 Outlook 中，可以为收件箱中的传入邮件设置规则，以便在特定条件下执行具体操作。 

可以按编程方式通过收件箱[文件夹](mailfolder.md)的 **messageRules** 导航属性来访问规则。 每个规则都由此 **messageRule** 资源表示，可用的规则操作由 [messageRuleActions](messageruleactions.md) 复杂类型表示，而可用的规则条件和例外则通过 [messageRulePredicates](messagerulepredicates.md) 复杂类型表示。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| actions | [messageRuleActions](messageruleactions.md) | 满足相应条件时对邮件执行的操作。 |
| conditions | [messageRulePredicates](messagerulepredicates.md) | 满足条件时，将触发该规则的相应操作。 |
| displayName | String | 规则的显示名称。 |
| exceptions | [messageRulePredicates](messagerulepredicates.md) | 规则的例外情况。 |
| hasError | Boolean | 指示规则是否处于错误状态。 只读。 |
| id |String|规则的唯一标识符。 只读。|
| isEnabled | Boolean | 指示是否启用规则以应用到邮件。 |
| isReadOnly | Boolean | 表示规则是否为只读且无法由规则 REST API 修改或删除。 |
| Sequence | Int32 | 表示在其他规则中执行规则的顺序。 |


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List rules](../api/mailfolder-list-messagerules.md) | [messageRule](messagerule.md) 集合 |获取为用户收件箱定义的所有 **messageRule** 对象。|
|[Get rule](../api/messagerule-get.md) | [messageRule](messagerule.md) |读取 **messageRule** 对象的属性和关系。|
|[Create](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) |通过指定一组条件和操作来创建 **messageRule** 对象。|
|[Update](../api/messagerule-update.md) | [messageRule](messagerule.md) |为 **messageRule** 对象更改可写属性并保存更改。 |
|[Delete](../api/messagerule-delete.md) | 无 |删除指定的 **messageRule** 对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
