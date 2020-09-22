---
title: 获取 educationRubric
description: 检索 educationrubric 对象的属性和关系。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c5454d52d30b6174cfbb5a387fea0d115d4981a4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002401"
---
# <a name="get-educationrubric"></a><span data-ttu-id="77e88-103">获取 educationRubric</span><span class="sxs-lookup"><span data-stu-id="77e88-103">Get educationRubric</span></span>

<span data-ttu-id="77e88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77e88-105">检索 [educationRubric](../resources/educationrubric.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77e88-105">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="77e88-106">请注意，在 () 中获取工作分配的 rubric 时 `GET /education/me/assignments/{id}/rubric` ，返回的内容是存在于下的原始 rubric 的不可变副本 `/education/users/{id}/rubrics` 。</span><span class="sxs-lookup"><span data-stu-id="77e88-106">Note that when getting the rubric of an assignment (`GET /education/me/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="77e88-107">副本与该特定工作分配相关联。</span><span class="sxs-lookup"><span data-stu-id="77e88-107">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="77e88-108">权限</span><span class="sxs-lookup"><span data-stu-id="77e88-108">Permissions</span></span>

<span data-ttu-id="77e88-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77e88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77e88-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77e88-111">Permission type</span></span>                        | <span data-ttu-id="77e88-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77e88-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77e88-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77e88-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="77e88-114">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="77e88-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="77e88-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77e88-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77e88-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77e88-116">Not supported.</span></span> |
| <span data-ttu-id="77e88-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77e88-117">Application</span></span>                            | <span data-ttu-id="77e88-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="77e88-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77e88-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77e88-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="77e88-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="77e88-120">Request headers</span></span>

| <span data-ttu-id="77e88-121">名称</span><span class="sxs-lookup"><span data-stu-id="77e88-121">Name</span></span>      |<span data-ttu-id="77e88-122">说明</span><span class="sxs-lookup"><span data-stu-id="77e88-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77e88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77e88-123">Authorization</span></span> | <span data-ttu-id="77e88-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="77e88-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="77e88-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="77e88-125">Request body</span></span>

<span data-ttu-id="77e88-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77e88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77e88-127">响应</span><span class="sxs-lookup"><span data-stu-id="77e88-127">Response</span></span>

<span data-ttu-id="77e88-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77e88-128">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77e88-129">示例</span><span class="sxs-lookup"><span data-stu-id="77e88-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77e88-130">请求</span><span class="sxs-lookup"><span data-stu-id="77e88-130">Request</span></span>

<span data-ttu-id="77e88-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77e88-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77e88-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="77e88-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="77e88-133">C#</span><span class="sxs-lookup"><span data-stu-id="77e88-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77e88-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77e88-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77e88-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77e88-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77e88-136">响应</span><span class="sxs-lookup"><span data-stu-id="77e88-136">Response</span></span>

<span data-ttu-id="77e88-137">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="77e88-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="77e88-138">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77e88-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77e88-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="77e88-139">All the properties will be returned from an actual call.</span></span>

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


