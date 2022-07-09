---
title: accessReviewReviewerScope 资源类型
description: 表示谁将审阅访问评审。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5374d68318349a9ae4fa7cb36c54e0aa8efe8870
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696530"
---
# <a name="accessreviewreviewerscope-resource-type"></a>accessReviewReviewerScope 资源类型

命名空间：microsoft.graph

accessReviewReviewerScope 定义谁将查看 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。 它是一个 OData 查询，允许审阅者同时指定为用户 (的静态列表，即特定用户、组所有者和组成员) 或动态地由其经理或组所有者评审每个用户。 若要创建自审 (用户在其中查看自己的访问权限) ，请勿在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | String | 指定谁将成为审阅者的查询。 有关示例，请参阅表。 |
| queryType | 字符串 | 查询的类型。 示例包括 `MicrosoftGraph` 和 `ARM`. |
| queryRoot | String | 在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 仅当指定了相对查询时， `./manager`才需要此属性。 可能的值： `decisions`. |

有关 **审阅者** 配置选项的详细信息，请参阅 [使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-reviewers-concept)。


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
