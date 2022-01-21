---
title: 更新 plannerTask
description: 更新 **plannertask** 对象的属性。
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 935de70d80b26a6a9dd48cd9e46e62c707f7fe16
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132270"
---
# <a name="update-plannertask"></a>更新 plannerTask

命名空间：microsoft.graph

更新 **plannertask** 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Tasks.ReadWrite，Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {token}。必需。 |
| If-Match  | 要更新的 **plannerTask** 的上次已知 ETag 值。必需。|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|appliedCategories|[plannerAppliedCategories](../resources/plannerappliedcategories.md)|此任务已应用的类别。有关可能的值，请参阅[已应用的类别](../resources/plannerappliedcategories.md)。|
|assigneePriority|String|用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](../resources/planner-order-hint-format.md)定义中。|
|assignments|[plannerAssignments](../resources/plannerassignments.md)|分配到任务的用户集合。|
|bucketId|String|任务所属的存储桶 ID。 存储桶需要位于任务所在的计划中。 长度为 28 个字符，区分大小写。 [格式验证](../resources/planner-identifiers-disclaimer.md)在服务上完成。 |
|conversationThreadId|字符串|任务对话的线程 id。这是在组中创建的对话线程对象的 id。|
|dueDateTime|DateTimeOffset|任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`|
|orderHint|String|用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](../resources/planner-order-hint-format.md)定义中。|
|percentComplete|Int32|任务完成的百分比。当设置为 `100` 时，任务被视为完成。 |
|startDateTime|DateTimeOffset|任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`|
|title|String|任务的标题。|

## <a name="response"></a>响应

如果成功，此方法将返回 `204 No Content` 响应和空内容。 如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerTask](../resources/plannertask.md) 对象。

此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}
Content-type: application/json
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": "N9917 U2883!"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category4": false
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-plannertask-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-plannertask-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-24T18:36:49.2407981Z",
  "assignments": {
    "6463a5ce-2119-4198-9f2a-628761df4a62": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "N9917"
    },
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2017-04-24T22:40:44.5665917",
      "orderHint": "RWk1"
    },
    "aaa27244-1db4-476a-a5cb-004607466324": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "U2883"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category5": true,
    "category6": true,
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

