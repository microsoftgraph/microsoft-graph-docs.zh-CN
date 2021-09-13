---
title: groupLifecyclePolicy 资源类型
description: 表示组策略的Microsoft 365策略。
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 2a927f172074e8a889589c9c0b475be78868ca62
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062675"
---
# <a name="grouplifecyclepolicy-resource-type"></a>groupLifecyclePolicy 资源类型

命名空间：microsoft.graph

表示组策略的Microsoft 365策略。 使用组生命周期策略，管理员可以为组设置到期期限。 例如，组在 180 天后到期。 如果组到期，组的所有者必须在管理员定义的时间段内续订组。 续订后，组的有效期就会延长策略中定义的天数。 例如，续订后，组的新到期时间是在 180 天后。 如果不续订组，组就会到期并被删除。 可以在删除后的 30 天内还原组。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取 groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |读取 groupLifecyclePolicy 对象的属性和关系。|
|[列出 groupLifecyclePolicy](../api/grouplifecyclepolicy-list.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) 集合 | 列出所有 groupLifecyclePolicy。 |
|[更新 groupLifecyclePolicy](../api/grouplifecyclepolicy-update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) | 更新 groupLifecyclePolicy 对象。 |
|[删除 groupLifecyclePolicy](../api/grouplifecyclepolicy-delete.md) | 无 | 删除 groupLifecyclePolicy 对象。 |
|[向 groupLifecyclePolicy 添加组](../api/grouplifecyclepolicy-addgroup.md)|无| 向生命周期策略添加组 |
|[从 groupLifecyclePolicy 中删除组](../api/grouplifecyclepolicy-removegroup.md)|无| 从生命周期策略中删除组 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|alternateNotificationEmails|String| 针对没有所有者的组向其发送通知的电子邮件地址列表。 可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。 |
|groupLifetimeInDays|Int32| 还剩多少天组就到期且需要续订。 续订后，组的有效期就会延长定义的天数。 |
|id|String| 策略的唯一标识符。 只读。|
|managedGroupTypes|String| 到期策略适用的组类型。 可取值为 **All**、**Selected** 或 **None**。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

