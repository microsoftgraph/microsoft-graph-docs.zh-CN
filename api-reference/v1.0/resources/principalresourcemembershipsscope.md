---
title: principalResourceMembershipsScope 资源类型
description: 允许选择访问评审作用域，以检查所选主体对选定资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 494e4c24f0fa912190e60b74fdc1c39e09bb3dc32f8590b30e7391e770eb0d0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196556"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>principalResourceMembershipsScope 资源类型

命名空间：microsoft.graph

principalResourceMembershipsScope 是 [accessReviewScope](accessreviewscope.md) 的一种类型，它允许您选择主体作用域的集合和资源作用域的集合，并查看所选主体对选定资源的访问权限。 它用于配置[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 scope 属性。 

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|principalScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义访问评审中审查其资源访问权限的主体的范围。|
|resourceScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义审查其访问权限的资源的范围。|

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
