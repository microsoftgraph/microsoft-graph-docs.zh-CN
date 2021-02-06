---
title: accessReviewScope 资源类型
description: '在 Azure AD 访问评审功能中，表示将在访问 `accessReviewScope` 评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8739ff822ffc6b0f2989b80a150c7d968880f532
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133439"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**accessReviewScope** 定义在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中将检查哪些实体。 这表示为 odata 查询。 还必须表示查询类型，以便支持方案来查看 MicrosoftGraph 外部的实体，如ARM。

## <a name="properties"></a>属性
| 属性   | 类型  | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 |字符串  | 指定将审阅哪些项的查询。 有关示例，请参阅表。 |
|queryType  |字符串 | 查询的类型。 示例包括 MicrosoftGraph 和 ARM。 |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a>支持将 accessReviewScope 作为范围的查询
以下是在 `scope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中作为属性支持的查询

|应用场景| 查询 | 其他注释 |
|--|--|-- |
| 审阅分配给组的所有用户 | /groups/{group id}/transitiveMembers ||
| 查看分配给组的来宾用户 | /groups/{group id}/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest')  ||
| 查看分配给所有组的来宾用户 | ./members/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest')  | 请注意，相应的 instanceEnumerationScope 还应传递到 accessReviewScheduleDefinition。 有关 instanceEnumerationScope 查询，请参阅下表。 |
| 权利管理访问包审查 | /identityGovernance/entitlementManagement/accessPackageAssignments？$filter= (accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}') | 请注意，访问包分配评审仅支持 READ|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a>支持将 accessReviewScope 作为 instanceEnumerationScope 的查询
以下是在 `instanceEnumerationScope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中作为属性支持的查询

|应用场景| 查询 | 其他注释 |
|--|--|--|
| 查看分配给所有组的来宾用户（不包括指定的组） | /groups？$filter= (groupTypes/any (c：c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}') &$count=true | 请注意，相应的作用域还应传递到 accessReviewScheduleDefinition。 有关范围查询，请参阅上述范围属性表中的"查看分配给所有组的来宾用户"。 |

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
