---
title: 创建 educationRubric
description: 创建新的 educationRubric 对象。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5e31839a9eb1c0e80e23e909a1d87f6c2b84428d
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439762"
---
# <a name="create-educationrubric"></a><span data-ttu-id="dd824-103">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="dd824-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd824-104">创建新的[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd824-104">Create a new [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd824-105">权限</span><span class="sxs-lookup"><span data-stu-id="dd824-105">Permissions</span></span>

<span data-ttu-id="dd824-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd824-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd824-108">Permission type</span></span>                        | <span data-ttu-id="dd824-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd824-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="dd824-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd824-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd824-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="dd824-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="dd824-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd824-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd824-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd824-113">Not supported.</span></span>                                          |
| <span data-ttu-id="dd824-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd824-114">Application</span></span>                            | <span data-ttu-id="dd824-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd824-115">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="dd824-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd824-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="dd824-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd824-117">Request headers</span></span>

| <span data-ttu-id="dd824-118">名称</span><span class="sxs-lookup"><span data-stu-id="dd824-118">Name</span></span>          | <span data-ttu-id="dd824-119">说明</span><span class="sxs-lookup"><span data-stu-id="dd824-119">Description</span></span>    |
| :------------ | :------------- |
| <span data-ttu-id="dd824-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd824-120">Authorization</span></span> | <span data-ttu-id="dd824-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dd824-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd824-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd824-122">Request body</span></span>

<span data-ttu-id="dd824-123">在请求正文中，提供[educationRubric](../resources/educationrubric.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd824-123">In the request body, supply a JSON representation of an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd824-124">响应</span><span class="sxs-lookup"><span data-stu-id="dd824-124">Response</span></span>

<span data-ttu-id="dd824-125">如果成功，此方法在`201 Created`响应正文中返回响应代码和新的[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd824-125">If successful, this method returns `201 Created` response code and a new [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd824-126">示例</span><span class="sxs-lookup"><span data-stu-id="dd824-126">Examples</span></span>

### <a name="example-1-posting-a-credit-rubric"></a><span data-ttu-id="dd824-127">示例1：过帐信用卡 Rubric</span><span class="sxs-lookup"><span data-stu-id="dd824-127">Example 1: Posting a Credit Rubric</span></span>

#### <a name="request"></a><span data-ttu-id="dd824-128">请求</span><span class="sxs-lookup"><span data-stu-id="dd824-128">Request</span></span>

<span data-ttu-id="dd824-129">下面的示例演示了如何将信用卡 rubric （没有点的 rubric）发布的请求。</span><span class="sxs-lookup"><span data-stu-id="dd824-129">The following is an example of the request to post a credit rubric (a rubric with no points).</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd824-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd824-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd824-131">C#</span><span class="sxs-lookup"><span data-stu-id="dd824-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd824-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd824-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd824-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd824-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dd824-134">响应</span><span class="sxs-lookup"><span data-stu-id="dd824-134">Response</span></span>

<span data-ttu-id="dd824-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dd824-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="dd824-136">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dd824-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd824-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dd824-137">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-posting-a-points-rubric"></a><span data-ttu-id="dd824-138">示例2：发布点 Rubric</span><span class="sxs-lookup"><span data-stu-id="dd824-138">Example 2: Posting a Points Rubric</span></span>

<span data-ttu-id="dd824-139">下面的示例演示了使用点发布 rubric 的请求。</span><span class="sxs-lookup"><span data-stu-id="dd824-139">The following is an example of the request to post a rubric with points.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
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

#### <a name="response"></a><span data-ttu-id="dd824-140">响应</span><span class="sxs-lookup"><span data-stu-id="dd824-140">Response</span></span>

<span data-ttu-id="dd824-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dd824-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="dd824-142">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dd824-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd824-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dd824-143">All the properties will be returned from an actual call.</span></span>

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
