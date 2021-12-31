---
title: accessReviewQueryScope 资源类型
description: 定义在访问评审中将审阅哪些项。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f1435e235baec8657f9f78c9bf842aa5ee6b61cf
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650480"
---
# <a name="accessreviewqueryscope-resource-type"></a>accessReviewQueryScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

accessReviewQueryScope 对象定义将在访问评审中 [审阅哪些项](../resources/accessreviewsv2-overview.md)。 若要将访问评审的范围确定为非活动用户，请参阅 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)。 

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|查询|String|表示将在访问评审中审阅哪些内容的查询。|
|queryRoot|String|在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定了相对查询时是必需的。 例如，`./manager`。|
|queryType|String|指示查询的类型。 类型包括 `MicrosoftGraph` `ARM` 和 。|

强烈建议@odata值指定 **@odata.type** `#microsoft.graph.accessReviewQueryScope` 属性。 有关使用 **accessReviewQueryScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph API 配置访问 [评审定义的范围](/graph/accessreviews-scope-concept)。 

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
