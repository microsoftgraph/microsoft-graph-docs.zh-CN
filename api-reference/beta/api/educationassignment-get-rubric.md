---
title: 获取附加到 educationAssignment 的 educationRubric
description: 获取附加到 educationAssignment 的 educationRubric（如果存在）。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b233b0a0ef3f51d5ee208b6b79a3c87584d69bc3
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118982"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="6a4bc-103">获取附加到 educationAssignment 的 educationRubric</span><span class="sxs-lookup"><span data-stu-id="6a4bc-103">Get educationRubric attached to educationAssignment</span></span>

<span data-ttu-id="6a4bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a4bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a4bc-105">获取附加到[educationAssignment](../resources/educationassignment.md)的[educationRubric](../resources/educationrubric.md)对象（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-105">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a4bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="6a4bc-106">Permissions</span></span>

<span data-ttu-id="6a4bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a4bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a4bc-109">Permission type</span></span>                        | <span data-ttu-id="6a4bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a4bc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a4bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a4bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a4bc-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a4bc-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="6a4bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a4bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a4bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-114">Not supported.</span></span> |
| <span data-ttu-id="6a4bc-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="6a4bc-115">Application\*</span></span>                           | <span data-ttu-id="6a4bc-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a4bc-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="6a4bc-117">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a4bc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a4bc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="6a4bc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a4bc-119">Request headers</span></span>

| <span data-ttu-id="6a4bc-120">名称</span><span class="sxs-lookup"><span data-stu-id="6a4bc-120">Name</span></span>      |<span data-ttu-id="6a4bc-121">说明</span><span class="sxs-lookup"><span data-stu-id="6a4bc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a4bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a4bc-122">Authorization</span></span> | <span data-ttu-id="6a4bc-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6a4bc-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a4bc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a4bc-124">Request body</span></span>

<span data-ttu-id="6a4bc-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a4bc-126">响应</span><span class="sxs-lookup"><span data-stu-id="6a4bc-126">Response</span></span>

<span data-ttu-id="6a4bc-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-127">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a4bc-128">示例</span><span class="sxs-lookup"><span data-stu-id="6a4bc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a4bc-129">请求</span><span class="sxs-lookup"><span data-stu-id="6a4bc-129">Request</span></span>

<span data-ttu-id="6a4bc-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a4bc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a4bc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric
```
# <a name="c"></a>[<span data-ttu-id="6a4bc-132">C#</span><span class="sxs-lookup"><span data-stu-id="6a4bc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a4bc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a4bc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a4bc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a4bc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a4bc-135">Java</span><span class="sxs-lookup"><span data-stu-id="6a4bc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a4bc-136">响应</span><span class="sxs-lookup"><span data-stu-id="6a4bc-136">Response</span></span>

<span data-ttu-id="6a4bc-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6a4bc-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a4bc-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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


