---
title: accessReviewScope 资源类型
description: '在 "Azure AD 访问评论" 功能中， `accessReviewScope` 表示将在访问评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af5a9bde0763f8aea9e28dc74832586c9e0d2e82
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000831"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AccessReviewScope** 定义将在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中审阅的实体。 这表示为 odata 查询。 此外，还必须表示查询类型，以便可以支持在 MicrosoftGraph 之外查看实体（如 ARM）的方案。

## <a name="properties"></a>属性
| 属性   | 类型  | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 |字符串  | 指定将评审的内容的查询。 有关示例，请参阅 table。 |
|queryType  |字符串 | 查询的类型。 示例包括 MicrosoftGraph 和 ARM。 |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a>支持的 accessReviewScope 作为范围的查询
以下是支持作为 `scope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中的属性的查询。

|应用场景| 查询 | 其他注释 |
|--|--|-- |
| 查看分配给组的所有用户 | /groups/{group id}/transitiveMembers ||
| 审阅分配给组的来宾用户 | /groups/{group id}/microsoft.graph.user/？ $count = true&$filter = (userType eq ' Guest ' )  ||
| 查看分配给所有组的来宾用户 | ./members/microsoft.graph.user/？ $count = true&$filter = (userType eq ' Guest ' )  | 请注意，相应的 instanceEnumerationScope 也应传递给 accessReviewScheduleDefinition。 有关 instanceEnumerationScope 查询，请参阅下表。 |
| 权利管理访问包 Assigment 评论 | $filter/identityGovernance/entitlementManagement/accessPackageAssignments = (accessPackageId eq ' {package id} ' 和 assignmentPolicyId eq ' {id} ' ) | 请注意，访问包分配审查仅支持读取|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a>支持的 accessReviewScope 查询为 instanceEnumerationScope
以下是支持作为 `instanceEnumerationScope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中的属性的查询。

|应用场景| 查询 | 其他注释 |
|--|--|--|
| 查看分配给所有组的来宾用户，但不包括指定的组 | $filter/groups = (groupTypes/any (c:c + eq + ' 统一 ' ) and id ne ' {group id} ' and id ne ' {group id} ' 和 id ne ' {group id} ' ) # B0 $count = true | 请注意，相应的作用域也应传递给 accessReviewScheduleDefinition。 有关范围查询，请参阅上面的作用域属性表中的 "复查分配给所有组的来宾用户"。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
