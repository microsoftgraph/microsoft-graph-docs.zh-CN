---
title: accessReviewnotificationrecipientqueryscope 资源类型
description: 指定将接收访问评审通知的用户列表。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82d1cbffd3e51ee8aff5dee3bdefd3196d004243
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562116"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>accessReviewnotificationrecipientqueryscope 资源类型

命名空间：microsoft.graph

指定用于接收访问评审 (特定用户、组所有者或) 的静态收件人列表。

继承自 [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | String | 表示收件人是谁的查询。 例如， `/groups/{group id}/members` 对于组的成员和 `/users/{user id}` 特定用户。 |
| queryType | String | 指示查询的类型。 允许的值为 `MicrosoftGraph` 。 |
| queryRoot | String | 在需要动态指定审阅者的情况下，指示查询的相对源。 此属性仅在指定相对查询 (，即) `./manager` 时是必需的。 |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
