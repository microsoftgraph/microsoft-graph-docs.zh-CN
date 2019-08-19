---
title: 获取 educationRubric
description: 检索 educationrubric 对象的属性和关系。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f57b3b38aeef88356dfb2502bf47f84c5e8e16c3
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460990"
---
# <a name="get-educationrubric"></a><span data-ttu-id="d99eb-103">获取 educationRubric</span><span class="sxs-lookup"><span data-stu-id="d99eb-103">Get educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d99eb-104">检索[educationRubric](../resources/educationrubric.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d99eb-104">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="d99eb-105">请注意, 在获取工作分配的 rubric (`GET /education/me/assignments/{id}/rubric`) 时, 返回的内容是存在于下`/education/users/{id}/rubrics`的原始 rubric 的不可变副本。</span><span class="sxs-lookup"><span data-stu-id="d99eb-105">Note that when getting the rubric of an assignment (`GET /education/me/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="d99eb-106">副本与该特定工作分配相关联。</span><span class="sxs-lookup"><span data-stu-id="d99eb-106">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d99eb-107">权限</span><span class="sxs-lookup"><span data-stu-id="d99eb-107">Permissions</span></span>

<span data-ttu-id="d99eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d99eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d99eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d99eb-110">Permission type</span></span>                        | <span data-ttu-id="d99eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d99eb-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d99eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d99eb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d99eb-113">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="d99eb-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d99eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d99eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d99eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d99eb-115">Not supported.</span></span> |
| <span data-ttu-id="d99eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d99eb-116">Application</span></span>                            | <span data-ttu-id="d99eb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d99eb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d99eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d99eb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d99eb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d99eb-119">Request headers</span></span>

| <span data-ttu-id="d99eb-120">名称</span><span class="sxs-lookup"><span data-stu-id="d99eb-120">Name</span></span>      |<span data-ttu-id="d99eb-121">说明</span><span class="sxs-lookup"><span data-stu-id="d99eb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d99eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d99eb-122">Authorization</span></span> | <span data-ttu-id="d99eb-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d99eb-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d99eb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d99eb-124">Request body</span></span>

<span data-ttu-id="d99eb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d99eb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d99eb-126">响应</span><span class="sxs-lookup"><span data-stu-id="d99eb-126">Response</span></span>

<span data-ttu-id="d99eb-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d99eb-127">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d99eb-128">示例</span><span class="sxs-lookup"><span data-stu-id="d99eb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d99eb-129">请求</span><span class="sxs-lookup"><span data-stu-id="d99eb-129">Request</span></span>

<span data-ttu-id="d99eb-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d99eb-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d99eb-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d99eb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d99eb-132">C#</span><span class="sxs-lookup"><span data-stu-id="d99eb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d99eb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d99eb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d99eb-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="d99eb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d99eb-135">响应</span><span class="sxs-lookup"><span data-stu-id="d99eb-135">Response</span></span>

<span data-ttu-id="d99eb-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d99eb-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d99eb-137">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d99eb-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d99eb-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d99eb-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
