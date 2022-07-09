---
title: accessReviewQueryScope 资源类型
description: 定义将在访问评审中查看的内容。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6fb31d3b040177e1065355bab7756b5bdf20ae02
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697867"
---
# <a name="accessreviewqueryscope-resource-type"></a>accessReviewQueryScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

accessReviewQueryScope 对象定义将在 [访问评审](../resources/accessreviewsv2-overview.md)中审查的内容。 若要将访问评审范围限定到非活动用户，请参阅 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)。 

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|查询|String|表示将在访问评审中查看的内容的查询。|
|queryRoot|字符串|在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 仅当指定了相对查询时，才需要此属性。 例如，`./manager`。|
|queryType|String|指示查询的类型。 类型包括 `MicrosoftGraph` 和 `ARM`.|

强烈建议使用该值`#microsoft.graph.accessReviewQueryScope`指定 **@odata.type** 属性。 有关使用 **accessReviewQueryScope** 的作用 **域** 的配置选项的详细信息，请参阅 [使用 Microsoft 图形 API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
