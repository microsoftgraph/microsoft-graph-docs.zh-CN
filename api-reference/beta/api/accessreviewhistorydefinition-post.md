---
title: 创建 accessReviewHistoryDefinition
description: 创建新的 accessReviewHistoryDefinition 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1ecb35c0c56d0db937aca60fa00d3559f0a063c4
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232904"
---
# <a name="create-accessreviewhistorydefinition"></a>创建 accessReviewHistoryDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.ReadWrite.All|

登录用户还必须是允许其读取访问评审以检索任何数据的目录角色。  有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象的 JSON 表示形式。

下表显示用于创建 [accessReviewHistoryDefinition 所需的属性](../resources/accessreviewhistorydefinition.md)。

|属性|类型|说明|
|:---|:---|:---|
|displayName | String  | 访问评审历史记录数据收集的名称。 必需。 |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | 时间戳、在此日期当天或之后开始审阅将包含在提取的历史记录数据中。 必需。  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | 时间戳、在此日期或之前开始审阅将包含在提取的历史记录数据中。 必需。  |
|scopes|microsoft.graph.accessReviewQueryScope 集合| 用于筛选包含在提取的历史记录数据中的审阅。 获取其范围与提供的范围匹配的审阅。 必需。  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>accessReviewHistoryDefinition 支持的范围查询

以下是基于[accessreviewqueryscope](../resources/accessreviewqueryscope.md)的[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)上支持的查询。 这些作用域规定创建定义时生成的可下载 CSV 文件中包含哪种类型的审阅历史记录数据。

|应用场景| 查询 |
|--|--|
| 包括单个组上的每个审阅结果 (不包括作用域为具有来宾用户的所有Microsoft 365 `accessReviewScheduleDefinition` 组)  | /identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups') " |
| 包括特定组上的每个审阅结果 (不包括作用域为具有来宾用户的所有Microsoft 365 `accessReviewScheduleDefinition` 组)  | /identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups/{group id}')  |
| 包含范围 `accessReviewScheduleDefinition` 为包含来宾用户的所有Microsoft 365组的所有审阅结果 | /identityGovernance/accessReviews/definitions？$filter=contains (scope/query， './members')  |
| 包含 `accessReviewScheduleDefinition` 访问包上的每个审阅结果 | /identityGovernance/accessReviews/definitions？$filter=contains (scope/query， 'accessPackageAssignments')  |
| 包括 `accessReviewScheduleDefinition` 分配给特权角色的服务主体的每次审阅结果 | /identityGovernance/accessReviews/definitions？$filter=contains (scope/query， 'roleAssignmentScheduleInstances')  |
| 包含 `accessReviewScheduleDefinition` 特定组的每次审阅结果 | /identityGovernance/accessReviews/definitions？$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members' |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。

## <a name="examples"></a>示例

以下示例演示如何创建访问评审历史记录定义，该定义范围为从 01/01/2021 的开始日期到 04/05/2021 的结束日期，以访问访问包和组上的审阅。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
