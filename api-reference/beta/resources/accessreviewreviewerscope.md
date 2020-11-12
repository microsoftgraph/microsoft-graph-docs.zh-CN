---
title: accessReviewReviewerScope 资源类型
description: 表示将查看访问评审的团队。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edc25e19a51f787dd0799fbd9e6e6c2a1b45787e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000839"
---
# <a name="accessreviewreviewerscope-resource-type"></a>accessReviewReviewerScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

AccessReviewReviewerScope 定义了将审阅 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)实例的作者。 这表示为 OData 查询，该查询允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (（即，每个用户被其经理) 审阅的情况）。 若要创建一个自我审阅 (用户在其中查看自己的访问) ，请不要在创建 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 的情况下提供审阅者。


## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | 字符串 | 指定将成为审阅者的查询。 有关示例，请参阅 table。 |
| queryType | 字符串 | 查询的类型。 示例包括 `MicrosoftGraph` 和 `ARM` 。 |
| queryRoot | 字符串 | 在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 仅当指定相对查询 (（即/manager) ）时，此属性才是必需的。 |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>AccessReviewReviewerScope 支持的查询

|应用场景| 查询 | queryType | queryRoot |
|--|--|--|--|
| 将所有者分组为审阅人 | /groups/{group id}/owners |MicrosoftGraph||
| 作为审阅者的特定用户 | /users/{user id} |MicrosoftGraph||
| 被审阅为审阅者的用户管理者 | ./manager | MicrosoftGraph |针对|

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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
