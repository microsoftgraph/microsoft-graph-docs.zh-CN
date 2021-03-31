---
title: accessReviewQueryScope 资源类型
description: 定义在访问评审中将审阅哪些项。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 976a856755b6bb638719bec6006c3d8d0587c42a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469747"
---
# <a name="accessreviewqueryscope-resource-type"></a>accessReviewQueryScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

accessReviewQueryScope 对象定义将在 [accessReview 中查看哪些项](../resources/accessreviewsv2-root.md)。 请参阅支持的查询以查看选择选项。 若要将访问评审的范围确定为非活动用户，请参阅 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)。 

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|查询|String|表示将在访问评审中审阅哪些内容的查询。 例如 ，/groups/{id}/members？$filter=...|
|queryRoot|String|在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定了相对查询时是必需的。 例如，`./manager`。|
|queryType|String|指示查询的类型。 类型包括 MicrosoftGraph 和 ARM。|

### <a name="supported-queries-for-accessreviewqueryscope-as-scope"></a>accessReviewQueryScope 作为范围的受支持的查询
这些查询作为 `scope` [accessReviewScheduleDefinition 中的 属性受到支持](accessreviewscheduledefinition.md)

|方案| 查询 | 其他注释 |
|--|--|-- |
| 查看分配给组的所有用户 | /groups/{group id}/transitiveMembers ||
| 查看分配给组的来宾用户 | /groups/{group id}/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest')  ||
| 查看分配给所有 Microsoft 365 组的来宾用户 | ./members/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest')  | 请注意，相应的 instanceEnumerationScope 还应传递到 accessReviewScheduleDefinition。 有关 instanceEnumerationScope 查询，请参阅下表。 |
| 权利管理访问包分配评审 | /identityGovernance/entitlementManagement/accessPackageAssignments？$filter= (accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}') | 请注意，Access Package Assignment Reviews 仅支持 READ|
| 查看分配给特权角色的服务主体 | /beta/roleManagement/directory/roleAssignmentScheduleInstances？$expand=principal&$filter= (isof (principal，'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')  | |

### <a name="supported-queries-for-instanceenumerationscope"></a>instanceEnumerationScope 支持的查询 
这些查询作为 `instanceEnumerationScope` [accessReviewScheduleDefinition 中的 属性受到支持](accessreviewscheduledefinition.md)

|方案| 查询 | 其他注释 |
|--|--|--|
|  查看分配给所有 Microsoft 365 组的来宾用户| /v1.0/groups？ \$filter= (groupTypes/any (c：c+eq+'Unified') ) &$count=true | 请注意，相应的作用域也应随以下项一起传入|
| 查看分配给所有团队的来宾用户 | /v1.0/groups？ \$filter= (groupTypes/any (c：c+eq+'Unified') and resourceProvisioningOptions/Any (x：x eq 'Team') ) &$count=true | 请注意，相应的作用域也应随以下项一起传入|

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
