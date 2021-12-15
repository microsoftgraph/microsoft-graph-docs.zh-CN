---
title: 列出提交
description: 列出与工作分配关联的所有提交。
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f572caf09a4127fc24957980d7b63b763e8631e4
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525868"
---
# <a name="list-submissions"></a>列出提交

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 [与作业](../resources/educationsubmission.md) 关联的所有 [提交](../resources/educationassignment.md)。

教师或具有应用程序权限的应用程序可以获取所有提交，学生只能获取与其关联的提交。 

提供标头 `Prefer: include-unknown-enum-members` 以正确 **列出状态** 为 `reassigned` 提交的提交。 有关详细信息，请参阅示例部分。

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
GET /education/classes/{class-id}/assignments/{assignment-id}/submissions
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

以下是此方法的 `$expand` 可用选项：、、和 `outcomes` `resources` `submittedResources` `*` ，其中包括之前的所有选项。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Prefer  | `include-unknown-enum-members`. 可选。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmission](../resources/educationsubmission.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-get-submissions"></a>示例 1：获取提交
#### <a name="request"></a>请求
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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-submissions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
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

### <a name="example-2-get-submissions-with-expand-options"></a>示例 2：获取具有$expand提交
#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","efcdf80b-a5de-42ac-8579-e40b0223d48b"],
  "name": "get_submissions_expand"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/efcdf80b-a5de-42ac-8579-e40b0223d48b/submissions?$expand=outcomes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-submissions-expand-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
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
Content-length: 4492

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('efcdf80b-a5de-42ac-8579-e40b0223d48b')/submissions(outcomes())",
    "value": [
        {
            "status": "returned",
            "submittedDateTime": null,
            "unsubmittedDateTime": null,
            "returnedDateTime": "2021-10-13T15:57:00.0349869Z",
            "reassignedDateTime": null,
            "resourcesFolderUrl": null,
            "id": "9bc724ee-d314-1ec5-725d-5f81228e85a6",
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
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "reassignedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            },
            "outcomes@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('efcdf80b-a5de-42ac-8579-e40b0223d48b')/submissions('9bc724ee-d314-1ec5-725d-5f81228e85a6')/outcomes",
            "outcomes": [
                {
                    "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
                    "lastModifiedDateTime": null,
                    "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
                    "lastModifiedBy": null,
                    "feedback": null,
                    "publishedFeedback": null
                },
                {
                    "@odata.type": "#microsoft.graph.educationPointsOutcome",
                    "lastModifiedDateTime": null,
                    "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
                    "lastModifiedBy": null,
                    "points": null,
                    "publishedPoints": null
                },
                {
                    "@odata.type": "#microsoft.graph.educationRubricOutcome",
                    "lastModifiedDateTime": "2021-10-13T15:57:00.0076092Z",
                    "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
                    "lastModifiedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": null,
                            "displayName": null
                        }
                    },
                    "rubricQualityFeedback": [
                        {
                            "qualityId": "f4c7b781-4c0c-4113-a5fb-c0885b7ab510",
                            "feedback": null
                        }
                    ],
                    "rubricQualitySelectedLevels": [
                        {
                            "qualityId": "f4c7b781-4c0c-4113-a5fb-c0885b7ab510",
                            "columnId": "ef99fe68-b6f8-4f67-a13b-9a81c1724788"
                        }
                    ],
                    "publishedRubricQualityFeedback": [
                        {
                            "qualityId": "f4c7b781-4c0c-4113-a5fb-c0885b7ab510",
                            "feedback": null
                        }
                    ],
                    "publishedRubricQualitySelectedLevels": [
                        {
                            "qualityId": "f4c7b781-4c0c-4113-a5fb-c0885b7ab510",
                            "columnId": "ef99fe68-b6f8-4f67-a13b-9a81c1724788"
                        }
                    ]
                }
            ]
        }
    ]
}
```

### <a name="example-3-get-submissions---request-with-optional-prefer-header"></a>示例 3：获取提交 - 具有可选 Prefer 标头的请求
#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submissions_prefer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions
Prefer: include-unknown-enum-members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-prefer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-prefer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-prefer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-prefer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-submissions-prefer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>响应
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
Content-length: 4492

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions",
    "value": [
        {
            "status": "working",
            "submittedDateTime": null,
            "unsubmittedDateTime": null,
            "returnedDateTime": null,
            "reassignedDateTime": null,
            "resourcesFolderUrl": null,
            "id": "f51a6687-a4a3-a8d9-ac4a-6ff81c5a8da7",
            "recipient": {
                "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
                "userId": "0ca0dd79-57eb-4903-97dc-88c769dd2a3d"
            },
            "submittedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0ca0dd79-57eb-4903-97dc-88c769dd2a3d",
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
            },
            "reassignedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "status": "reassigned",
            "submittedDateTime": "2021-11-10T00:57:17.0495233Z",
            "unsubmittedDateTime": null,
            "returnedDateTime": null,
            "reassignedDateTime": "2021-11-10T01:03:25.7812455Z",
            "resourcesFolderUrl": null,
            "id": "869369de-3e5a-89eb-6f2d-83cd88f860b5",
            "recipient": {
                "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
                "userId": "723e2402-f503-4825-a4d5-5143fbe6f53d"
            },
            "submittedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "723e2402-f503-4825-a4d5-5143fbe6f53d",
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
            },
            "reassignedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "afc58f1f-7c9e-4770-a448-e53ba43463a5",
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
