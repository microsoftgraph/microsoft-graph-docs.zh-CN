---
title: 创建 educationRubric
description: 创建新的 educationRubric 对象。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a0ce2f6bc0c284ac14ac4494cfbc506986a4e7cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951050"
---
# <a name="create-educationrubric"></a><span data-ttu-id="4a67f-103">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="4a67f-103">Create educationRubric</span></span>

<span data-ttu-id="4a67f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a67f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a67f-105">创建新的 [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a67f-105">Create a new [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a67f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a67f-106">Permissions</span></span>

<span data-ttu-id="4a67f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a67f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a67f-109">Permission type</span></span>                        | <span data-ttu-id="4a67f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a67f-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="4a67f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a67f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a67f-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a67f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="4a67f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a67f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a67f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a67f-114">Not supported.</span></span>                                          |
| <span data-ttu-id="4a67f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a67f-115">Application</span></span>                            | <span data-ttu-id="4a67f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a67f-116">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="4a67f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a67f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="4a67f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a67f-118">Request headers</span></span>

| <span data-ttu-id="4a67f-119">名称</span><span class="sxs-lookup"><span data-stu-id="4a67f-119">Name</span></span>          | <span data-ttu-id="4a67f-120">说明</span><span class="sxs-lookup"><span data-stu-id="4a67f-120">Description</span></span>    |
| :------------ | :------------- |
| <span data-ttu-id="4a67f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a67f-121">Authorization</span></span> | <span data-ttu-id="4a67f-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4a67f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a67f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a67f-123">Request body</span></span>

<span data-ttu-id="4a67f-124">在请求正文中，提供 [educationRubric](../resources/educationrubric.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a67f-124">In the request body, supply a JSON representation of an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4a67f-125">响应</span><span class="sxs-lookup"><span data-stu-id="4a67f-125">Response</span></span>

<span data-ttu-id="4a67f-126">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和新 [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a67f-126">If successful, this method returns `201 Created` response code and a new [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a67f-127">示例</span><span class="sxs-lookup"><span data-stu-id="4a67f-127">Examples</span></span>

### <a name="example-1-posting-a-credit-rubric"></a><span data-ttu-id="4a67f-128">示例 1：发布信用额度</span><span class="sxs-lookup"><span data-stu-id="4a67f-128">Example 1: Posting a Credit Rubric</span></span>

#### <a name="request"></a><span data-ttu-id="4a67f-129">请求</span><span class="sxs-lookup"><span data-stu-id="4a67f-129">Request</span></span>

<span data-ttu-id="4a67f-130">下面是一个请求发布信用额度， (一个没有分数的) 。</span><span class="sxs-lookup"><span data-stu-id="4a67f-130">The following is an example of the request to post a credit rubric (a rubric with no points).</span></span>

# <a name="http"></a>[<span data-ttu-id="4a67f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a67f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser_1"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Credit Rubric",
    "description":{
        "content":"This is an example of a credit rubric (no points)",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ]
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="4a67f-132">C#</span><span class="sxs-lookup"><span data-stu-id="4a67f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a67f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a67f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a67f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a67f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a67f-135">Java</span><span class="sxs-lookup"><span data-stu-id="4a67f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a67f-136">响应</span><span class="sxs-lookup"><span data-stu-id="4a67f-136">Response</span></span>

<span data-ttu-id="4a67f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4a67f-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4a67f-138">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4a67f-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a67f-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4a67f-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Credit Rubric",
    "id": "63618139-2e8d-4f56-a762-dd734736816f",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "qualities": [
        {
            "qualityId": "461e866a-4844-4a3f-9a3c-e5464a32acf1",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ccb47c1c-1a01-4027-93d7-f14b9fe86fdd",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "levels": [
        {
            "levelId": "564e68f6-984b-4574-bea7-ffae3c92633f",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f082e35-46e3-4944-baea-ea6c7e36ef37",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ]
}
```

### <a name="example-2-posting-a-points-rubric"></a><span data-ttu-id="4a67f-140">示例 2：发布点数</span><span class="sxs-lookup"><span data-stu-id="4a67f-140">Example 2: Posting a Points Rubric</span></span>

<span data-ttu-id="4a67f-141">下面是一个请求发布带分数的分数的分数的示例。</span><span class="sxs-lookup"><span data-stu-id="4a67f-141">The following is an example of the request to post a rubric with points.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a67f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a67f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser_2"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Points Rubric",
    "description":{
        "content":"This is an example of a rubric with points",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":2
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":1
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        }
    ],
    "grading":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="4a67f-143">C#</span><span class="sxs-lookup"><span data-stu-id="4a67f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a67f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a67f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a67f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a67f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a67f-146">Java</span><span class="sxs-lookup"><span data-stu-id="4a67f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a67f-147">响应</span><span class="sxs-lookup"><span data-stu-id="4a67f-147">Response</span></span>

<span data-ttu-id="4a67f-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4a67f-148">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4a67f-149">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4a67f-149">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a67f-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4a67f-150">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Points Rubric",
    "id": "bf040af7-a5ff-4abe-a8c8-1bdc532344c2",
    "description": {
        "content": "This is an example of a rubric with points",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "519cd134-c513-40b9-aa71-fdb0d063c084",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 2
            }
        },
        {
            "levelId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 1
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
            "weight": 50.0,
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5e637d79-f26b-4ea6-acd7-73824f0c0967",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "ebdcc27f-d1ec-4aa3-9da7-bd8d7842e3d3",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
            "weight": 50.0,
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5417252a-f810-41eb-9a83-09276a258a08",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "5de220bd-74b9-41a7-85d5-9be7c6cb7933",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


