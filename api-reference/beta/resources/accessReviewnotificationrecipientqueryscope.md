---
title: accessReviewnotificationrecipientqueryscope 资源类型
description: 表示将接收访问评审通知的用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b619b7479212e5fc055f5ab19b025d8d512dc1
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896732"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>accessReviewnotificationrecipientqueryscope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

指定收件人的静态 (例如，特定用户、组所有者或组) 接收访问评审通知。

继承自 [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | String | 这表示对收件人是谁的查询。 例如， `/groups/{group id}/members` 对于组的成员和 `/users/{user id}` 特定用户。 |
| queryType | String | 指示查询的类型。 允许的值为 `MicrosoftGraph` 。 |
| queryRoot | String | 在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定相对查询时是必需的，即) `./manager` 查询。 |


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
