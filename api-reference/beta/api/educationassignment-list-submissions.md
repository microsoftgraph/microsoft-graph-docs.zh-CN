---
title: 列出提交
description: 列出与工作分配关联的所有提交。
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0f28375a67b7db090fa1a3dda5f7bb91ddc900cd
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763188"
---
# <a name="list-submissions"></a>列出提交

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出与作业关联的所有 [提交](../resources/educationassignment.md)。

教师或具有应用程序权限的应用程序可以获取所有提交，而学生只能获取与其关联的提交。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | EduAssignments.ReadBasic.All、EduAssignments.ReadWriteBasic.All、EduAssignments.Read.All、EduAssignments.ReadWrite.All | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmission](../resources/educationsubmission.md) 对象集合。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["f4a941ff-9da6-4707-ba5b-0eae93cad0b4","3c77de7f-539b-49e1-9c96-1274f2f0ee3b"],
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/3c77de7f-539b-49e1-9c96-1274f2f0ee3b/submissions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [
        {
            "status": "working",
            "submittedDateTime": null,
            "unsubmittedDateTime": null,
            "returnedDateTime": null,
            "resourcesFolderUrl": "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEDJCE5LX4OXABF37QSORAK5WKQD",
            "id": "4af73d2b-6b9c-493f-0688-979087bed39b",
            "recipient": {
                "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
                "userId": "80cefd93-8d88-40e2-b5d3-67898383e226"
            },
            "submittedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                    "displayName": null
                }
            },
            "unsubmittedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            },
            "returnedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
