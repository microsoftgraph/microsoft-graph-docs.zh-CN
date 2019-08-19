---
title: 获取附加到 educationAssignment 的 educationRubric
description: 获取附加到 educationAssignment 的 educaitonRubric (如果存在)。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 19d2867749a0b53e6b5649610ed6626af56fce38
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461188"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="d3d2c-103">获取附加到 educationAssignment 的 educationRubric</span><span class="sxs-lookup"><span data-stu-id="d3d2c-103">Get educationRubric attached to educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d2c-104">获取附加到[educationAssignment](../resources/educationassignment.md)的[educationRubric](../resources/educationrubric.md)对象 (如果有的话)。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-104">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3d2c-105">权限</span><span class="sxs-lookup"><span data-stu-id="d3d2c-105">Permissions</span></span>

<span data-ttu-id="d3d2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3d2c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3d2c-108">Permission type</span></span>                        | <span data-ttu-id="d3d2c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3d2c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3d2c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3d2c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3d2c-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="d3d2c-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d3d2c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3d2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3d2c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-113">Not supported.</span></span> |
| <span data-ttu-id="d3d2c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3d2c-114">Application</span></span>                            | <span data-ttu-id="d3d2c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3d2c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3d2c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="d3d2c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3d2c-117">Request headers</span></span>

| <span data-ttu-id="d3d2c-118">名称</span><span class="sxs-lookup"><span data-stu-id="d3d2c-118">Name</span></span>      |<span data-ttu-id="d3d2c-119">说明</span><span class="sxs-lookup"><span data-stu-id="d3d2c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3d2c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3d2c-120">Authorization</span></span> | <span data-ttu-id="d3d2c-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d3d2c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3d2c-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3d2c-122">Request body</span></span>

<span data-ttu-id="d3d2c-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3d2c-124">响应</span><span class="sxs-lookup"><span data-stu-id="d3d2c-124">Response</span></span>

<span data-ttu-id="d3d2c-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-125">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3d2c-126">示例</span><span class="sxs-lookup"><span data-stu-id="d3d2c-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3d2c-127">请求</span><span class="sxs-lookup"><span data-stu-id="d3d2c-127">Request</span></span>

<span data-ttu-id="d3d2c-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3d2c-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d3d2c-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3d2c-130">C#</span><span class="sxs-lookup"><span data-stu-id="d3d2c-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3d2c-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3d2c-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3d2c-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="d3d2c-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3d2c-133">响应</span><span class="sxs-lookup"><span data-stu-id="d3d2c-133">Response</span></span>

<span data-ttu-id="d3d2c-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="d3d2c-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": false
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
  "description": "List rubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
