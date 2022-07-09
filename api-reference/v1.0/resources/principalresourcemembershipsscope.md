---
title: principalResourceMembershipsScope 资源类型
description: 允许选择访问评审范围，以评审所选主体对所选资源的访问权限。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2f9c2982dd8b73969d9b51b2242ad2c33367031e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698070"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>principalResourceMembershipsScope 资源类型

命名空间：microsoft.graph

principalResourceMembershipsScope 是一种 [accessReviewScope](accessreviewscope.md) 类型，可用于选择主体范围的集合和资源范围的集合，并查看所选主体对所选资源的访问权限。 它用于配置 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) **的范围** 属性。

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|principalScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义访问评审中评审其对资源的访问权限的主体的范围。|
|resourceScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义要审查其访问权限的资源的范围。|

还必须指定具有该值`#microsoft.graph.principalResourceMembershipsScope`**的 @odata.type** 属性。 有关使用 **principalResourceMembershipsScope** 的作用 **域** 的配置选项的详细信息，请参阅 [使用 Microsoft 图形 API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
