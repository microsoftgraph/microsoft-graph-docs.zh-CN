---
title: 创建 historyDefinitions
description: 创建新的 accessReviewHistoryDefinition 对象。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7533b52e58f7229043bf9e6132ca02d36d7acc29
ms.sourcegitcommit: 1ae0079021dfcbcc910dcdc74440d367ec4af7d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63460131"
---
# <a name="create-historydefinitions"></a>创建 historyDefinitions

命名空间：microsoft.graph

创建新的 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.ReadWrite.All|

登录用户还必须是允许其读取访问评审以检索任何数据的目录角色。  有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-overview.md)。

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

下表显示用于创建 [accessReviewHistoryDefinition 的必需属性](../resources/accessreviewhistorydefinition.md)。

|属性|类型|说明|
|:---|:---|:---|
|displayName | 字符串  | 访问评审历史记录数据收集的名称。 必需。 |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | 时间戳。 在此日期或之后开始审阅将包含在提取的历史记录数据中。 仅在未定义 **scheduleSettings** 时是必需的。  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | 时间戳。 在此日期或之前开始审阅将包含在提取的历史记录数据中。 仅在未定义 **scheduleSettings** 时是必需的。  |
|scopes|[accessReviewQueryScope](../resources/accessreviewqueryscope.md) 集合| 用于筛选包含在提取的历史记录数据中的审阅。 获取其范围与提供的范围匹配的审阅。 必需。 <br> 有关详细信息，请参阅 [accessReviewHistoryDefinition 支持的作用域查询](#supported-scope-queries-for-accessreviewhistorydefinition)。 |
| scheduleSettings  |[accessReviewHistoryScheduleSettings](../resources/accessReviewHistoryScheduleSettings.md)| 定期访问评审历史记录定义系列的设置。 仅在未定义 **reviewHistoryPeriodStartDateTime** 或 **reviewHistoryPeriodEndDateTime** 时是必需的。|

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>accessReviewHistoryDefinition 支持的范围查询

[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 的 **scopes** 属性基于 **accessReviewQueryScope**，这是一种允许您在查询属性中配置不同 **资源** 的资源。 然后，这些资源表示历史记录定义的作用域，并指示在创建历史记录定义的 [accessReviewHistoryInstances](../resources/accessreviewhistoryinstance.md) 时生成的可下载 CSV 文件中包含的审阅历史记录数据的类型。

对查询 **属性使用以下格式** ：

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

的值 `{object}` 是可在 **accessReviewScheduleDefinition 中配置的资源之一**。 例如，以下内容包括单个组上的每个 accessReviewScheduleDefinition 审阅结果 (并排除作用域为具有来宾用户的所有 Microsoft 365 组) 。

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

有关更多支持的值，请参阅在 [accessReviewScheduleDefinition $filter查询参数](accessreviewset-list-definitions.md#use-the-filter-query-parameter)。

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。

## <a name="examples"></a>示例

以下示例演示如何创建访问评审历史记录定义，该定义范围为从 01/01/2021 的开始日期到 04/05/2021 的结束日期，以访问访问包和组上的审阅。

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions
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
  "scheduleSettings": {
      "reportRange": "P1M",
      "recurrence": {
          "pattern": {
              "type": "monthly",
              "interval": 1
          },
          "range": {
              "type": "noEnd",
              "startDate": "2018-08-03T21:02:30.667Z",
              "count": 0
          }
        }
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accessreviewhistorydefinition-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "scheduleSettings": {
        "reportRange": "P1M",
        "recurrence": {
            "pattern": {
                "type": "monthly",
                "interval": 1
            },
            "range": {
                "type": "noEnd",
                "startDate": "2018-08-03T21:02:30.667Z",
                "count": 0
            }
        }
    },
    "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
    ],
    "status": "requested",
    "createdDateTime": "2021-04-14T00:22:48.9392594Z",
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
