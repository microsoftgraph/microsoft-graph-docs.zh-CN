---
title: 列出结果
description: 检索 educationoutcome 对象的列表。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 72f4d034b9afa7639b8cc671aff01489c5a334db
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900238"
---
# <a name="list-outcomes"></a>列出结果

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [educationOutcome](../resources/educationoutcome.md) 对象的列表。  有四种类型的结果： **educationPointsOutcome**、 **educationFeedbackOutcome**、 **educationRubricOutcome** 和 **educationFeedbackResourceOutcome**。

信用分配的提交 (没有点值且没有) 将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 的提交。  (它也可能返回 [educationPointsOutcome](../resources/educationpointsoutcome.md)，但该结果将被忽略。) 

 (分配了点值的分数分配的提交) 将同时具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 和 [educationPointsOutcome](../resources/educationpointsoutcome.md)。

如果使用附加的 rubric 进行作业的提交（如果 rubric 是信用标准 (没有积分) ，则将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 和 [educationRubricOutcome](../resources/educationrubricoutcome.md)。  (它也可能返回 [educationPointsOutcome](../resources/educationpointsoutcome.md)，但该结果将被忽略。) 

如果使用附加的 rubric 的作业提交，如果 rubric 是磅，则将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)（一个 [educationPointsOutcome] (.）。/resources/educationpointsoutcome.md 和 [educationRubricOutcome](../resources/educationrubricoutcome.md)。

反馈资源的提交将具有 [educationFeedbackResourceOutcome](../resources/educationfeedbackresourceoutcome.md)。

所有结果类型都有一个适合该结果类型的常规属性和已发布属性;例如， **点** 和 **已发布的Points**、 **反馈** 和 **已发布的Feedback**。  常规属性是教师更新的最新值：已发布的属性是返回给学生的最新值。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EduAssignments.ReadBasic.All、EduAssignments.ReadWriteBasic.All、EduAssignments.Read.All、EduAssignments.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [educationOutcome](../resources/educationoutcome.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-get-all-outcomes"></a>示例 1：获取所有结果

以下示例演示如何检索所有结果。

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outcomes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-outcomes-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-outcomes-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationOutcome",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "feedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedFeedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "points": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedPoints": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "rubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ]
        }
    ]
}
```

### <a name="example-2-get-outcomes-filtered-by-outcome-type"></a>示例 2：获取按结果类型筛选的结果

以下示例演示如何检索按结果类型筛选的结果。

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "get_outcomes_by_type"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/assignments/a3cce0ba-2008-4c4d-bf62-079408562d96/submissions/2185e6d7-2924-4ed1-dde1-269f89e29184/outcomes?$filter=isof('microsoft.graph.educationFeedbackResourceOutcome')
```

#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationOutcome",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('37d99af7-cfc5-4e3b-8566-f7d40e4a2070')/assignments('a3cce0ba-2008-4c4d-bf62-079408562d96')/submissions('2185e6d7-2924-4ed1-dde1-269f89e29184')/outcomes",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackResourceOutcome",
            "lastModifiedDateTime": "2022-05-06T00:52:12.8318457Z",
            "id": "8fb409c5-570b-4fe5-8473-d3666e61f3a0",
            "resourceStatus": "notPublished",
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                    "displayName": null
                }
            },
            "feedbackResource": {
                "@odata.type": "#microsoft.graph.educationWordResource",
                "displayName": "Document2.docx",
                "createdDateTime": "2022-05-06T00:52:12.8318064Z",
                "lastModifiedDateTime": "2022-05-06T00:52:12.8318457Z",
                "fileUrl": "https://graph.microsoft.com/beta/drives/b!-Ik2sRPLDEWy_bR8l75jfeDcpXQcRKVOmcml10NQLQ1F8CNZWU38SarWxPyWM7jx/items/01VANVJQ26WF6K2W2IOFAKDITG4F5GWRH5",
                "createdBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                        "displayName": null
                    }
                },
                "lastModifiedBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                        "displayName": null
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationFeedbackResourceOutcome",
            "lastModifiedDateTime": "2022-05-06T00:52:17.3180275Z",
            "id": "0710aeea-590d-46b4-9eb8-1c08b6549677",
            "resourceStatus": "notPublished",
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                    "displayName": null
                }
            },
            "feedbackResource": {
                "@odata.type": "#microsoft.graph.educationWordResource",
                "displayName": "Document3.docx",
                "createdDateTime": "2022-05-06T00:52:17.3180176Z",
                "lastModifiedDateTime": "2022-05-06T00:52:17.3180275Z",
                "fileUrl": "https://graph.microsoft.com/beta/drives/b!-Ik2sRPLDEWy_bR8l75jfeDcpXQcRKVOmcml10NQLQ1F8CNZWU38SarWxPyWM7jx/items/01VANVJQ563EMEMHRTBBH2SOZ4GDSNEUZK",
                "createdBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                        "displayName": null
                    }
                },
                "lastModifiedBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                        "displayName": null
                    }
                }
            }
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List outcomes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
