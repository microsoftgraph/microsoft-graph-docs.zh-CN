---
title: accessReviewReviewerScope 资源类型
description: 表示将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58abda6c89e484336b34d546edc68ebbfe432162
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579252"
---
# <a name="accessreviewreviewerscope-resource-type"></a>accessReviewReviewerScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

accessReviewReviewerScope 定义谁将审阅 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。 它是一个 OData 查询，它允许将审阅者指定为用户 (（即特定用户、组所有者和组成员) ）的静态列表，或者动态地将审阅者指定为其经理或组所有者审阅每个用户。 若要创建自审阅 (用户查看自己的访问权限) ，请不要在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | String | 用于指定审阅者的查询。 有关示例，请参阅表。 |
| queryType | String | 查询的类型。 示例包括 `MicrosoftGraph` `ARM` 和 。 |
| queryRoot | String | 在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定了相对查询（例如 ） `./manager` 时是必需的。 可能的值 `decisions` ：。 |

有关审阅者的 **配置选项的详细信息**，请参阅使用 Microsoft Graph API 将审阅者 [分配给你的访问Graph定义](/graph/accessreviews-reviewers-concept)。


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
