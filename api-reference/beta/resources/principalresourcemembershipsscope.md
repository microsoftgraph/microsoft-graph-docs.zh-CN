---
title: principalResourceMembershipsScope 资源类型
description: 允许选择范围查看所选主体对选定资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2ac3dd53223b9260c3f51c3c872d36b044e698d5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469742"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>principalResourceMembershipsScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

principalResourceMembershipsScope 是 [accessReviewScope](accessreviewscope.md) 的一种类型，它允许您选择主体作用域的集合和资源作用域的集合，并查看所选主体对选定资源的访问权限。 请参阅受支持的查询以查看可以选择哪些查询。 它用作 `scope` [accessReviewScheduleDefinition 的属性](accessreviewscheduledefinition.md)。

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|principalScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义要包含在访问评审中的主体范围。|
|resourceScopes|[accessReviewScope](../resources/accessreviewscope.md) 集合|定义将检查其访问权限的资源的范围。|

## <a name="relationships"></a>关系
无。

### <a name="supported-queries-for-resourcescope"></a>resourceScope 支持的查询
支持将查询作为 `resourceScope` 属性。 它们确定要检查的资源访问权限集。 

|方案| resourceScope 查询 | 
|--|--|
| 查看对服务主体的 principalScopes 的访问 | /servicePrincipals/{service principal ID} |
| 查看对 Azure AD 目录角色的 principalScopes 的访问权限 | /roleManagement/directory/roleDefinitions/{role ID} |
| 查看所有 Azure AD 目录角色对 principalScopes 的访问权限 | /roleManagement/directory/roleDefinitions |

### <a name="supported-queries-for-principalscope"></a>principalScope 支持的查询
支持将查询作为 `principalScope` 属性。 它们确定将检查其对关联 resourceScope 的访问权的主体集。 关联的 principalScope 类型列出了接受为 principalScope 的 odata 查询类型。

|方案| principalScope 查询 | OData 查询类型 | 其他注释 |
|--|--|-- | --|
| 查看所有用户对 resourceScope 的访问权限 | /users |[accessReviewQueryScope](accessreviewqueryscope.md)||
| 查看来宾用户对 resourceScope 的访问权限 | /users？$filter= (userType eq 'Guest')  |[accessReviewQueryScope](accessreviewqueryscope.md)||
| 查看所有非活动用户对 resourceScope 的访问权限 | /users |[accessReviewInactiveUsersQueryScope](accessreviewinactiveusersqueryscope.md)| 必须包含 `instanceDuration` 属性|
| 查看对 resourceScope 的来宾非活动用户的访问权限 | /users？$filter= (userType eq 'Guest')  |[accessReviewInactiveUsersQueryScope](accessreviewinactiveusersqueryscope.md)| 必须包含 `instanceDuration` 属性|




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
