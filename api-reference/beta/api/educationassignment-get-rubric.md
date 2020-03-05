---
title: 获取附加到 educationAssignment 的 educationRubric
description: 获取附加到 educationAssignment 的 educaitonRubric （如果存在）。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ad4e72c2d638e1b07aa1ef363f8d0c406ef9b4bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427653"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="11242-103">获取附加到 educationAssignment 的 educationRubric</span><span class="sxs-lookup"><span data-stu-id="11242-103">Get educationRubric attached to educationAssignment</span></span>

<span data-ttu-id="11242-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="11242-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11242-105">获取附加到[educationAssignment](../resources/educationassignment.md)的[educationRubric](../resources/educationrubric.md)对象（如果有的话）。</span><span class="sxs-lookup"><span data-stu-id="11242-105">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="11242-106">权限</span><span class="sxs-lookup"><span data-stu-id="11242-106">Permissions</span></span>

<span data-ttu-id="11242-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11242-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11242-109">Permission type</span></span>                        | <span data-ttu-id="11242-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11242-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11242-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11242-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11242-112">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="11242-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="11242-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11242-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11242-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="11242-114">Not supported.</span></span> |
| <span data-ttu-id="11242-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11242-115">Application</span></span>                            | <span data-ttu-id="11242-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11242-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11242-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11242-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="11242-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="11242-118">Request headers</span></span>

| <span data-ttu-id="11242-119">名称</span><span class="sxs-lookup"><span data-stu-id="11242-119">Name</span></span>      |<span data-ttu-id="11242-120">说明</span><span class="sxs-lookup"><span data-stu-id="11242-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11242-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11242-121">Authorization</span></span> | <span data-ttu-id="11242-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="11242-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="11242-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="11242-123">Request body</span></span>

<span data-ttu-id="11242-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11242-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11242-125">响应</span><span class="sxs-lookup"><span data-stu-id="11242-125">Response</span></span>

<span data-ttu-id="11242-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11242-126">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11242-127">示例</span><span class="sxs-lookup"><span data-stu-id="11242-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11242-128">请求</span><span class="sxs-lookup"><span data-stu-id="11242-128">Request</span></span>

<span data-ttu-id="11242-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11242-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11242-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="11242-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```
# <a name="c"></a>[<span data-ttu-id="11242-131">C#</span><span class="sxs-lookup"><span data-stu-id="11242-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11242-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11242-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11242-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11242-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11242-134">响应</span><span class="sxs-lookup"><span data-stu-id="11242-134">Response</span></span>

<span data-ttu-id="11242-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11242-135">The following is an example of the response.</span></span>

> <span data-ttu-id="11242-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="11242-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
