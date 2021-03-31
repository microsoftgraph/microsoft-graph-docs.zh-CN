---
title: accessReviewReviewerScope 资源类型
description: 表示将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 55f881ff1bcb1b08cc66938fd8a7b4d28f540687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469544"
---
# <a name="accessreviewreviewerscope-resource-type"></a>accessReviewReviewerScope 资源类型

命名空间：microsoft.graph

accessReviewReviewerScope 定义在 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 中指定的审阅 [appConsentRequests](../resources/appconsentrequest.md) 和 [userConsentRequests 的用户](../resources/appconsentrequest.md)。 这表示为 OData 查询，它允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (，即每个用户都由其经理) 审阅的情况。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|查询|String|用于指定审阅者的查询。 有关示例，请参阅表。 |
|queryRoot|String|查询的类型。 示例包括 `MicrosoftGraph` `ARM` 和 。|
|queryType|String|在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定了相对查询 (，即) `./manager` 时是必需的。|

### <a name="supported-queries-for-accessreviewreviewerscope"></a>accessReviewReviewerScope 支持的查询

|方案| 查询 | queryType | queryRoot |
|--|--|--|--|
| 作为审阅者的组所有者 | /groups/{group id}/owners |MicrosoftGraph||
| 作为审阅者的特定用户 | /users/{user id} |MicrosoftGraph||
| 被审阅为审阅者的用户的经理 | ./manager | MicrosoftGraph |决策|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
