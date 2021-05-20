---
title: principalResourceMembershipsScope 资源类型
description: 允许选择范围查看所选主体对选定资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b22c52c0bf71f1a1169d51e2e6fd3e8ac10e99d9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579891"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>principalResourceMembershipsScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

principalResourceMembershipsScope 是 [accessReviewScope](accessreviewscope.md) 的一种类型，它允许您选择主体作用域的集合和资源作用域的集合，并查看所选主体对选定资源的访问权限。 它用于配置[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 scope 属性。 

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|principalScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义要包含在访问评审中的主体范围。|
|resourceScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义将检查其访问权限的资源的范围。|

还必须使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.principalResourceMembershipsScope` 。 有关使用 **principalResourceMembershipsScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph API 配置访问 [评审定义的范围](/graph/accessreviews-scope-concept)。 

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
