---
title: 列出 rubrics
description: 检索 educationrubric 对象的列表。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 316c49a9e0b6591ad64bd30e4ce80809eb8f0ac6
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461316"
---
# <a name="list-rubrics"></a><span data-ttu-id="0699b-103">列出 rubrics</span><span class="sxs-lookup"><span data-stu-id="0699b-103">List rubrics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0699b-104">检索[educationRubric](../resources/educationrubric.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0699b-104">Retrieve a list of [educationRubric](../resources/educationrubric.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0699b-105">权限</span><span class="sxs-lookup"><span data-stu-id="0699b-105">Permissions</span></span>

<span data-ttu-id="0699b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0699b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0699b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0699b-108">Permission type</span></span>                        | <span data-ttu-id="0699b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0699b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0699b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0699b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0699b-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0699b-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="0699b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0699b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0699b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0699b-113">Not supported.</span></span> |
| <span data-ttu-id="0699b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0699b-114">Application</span></span>                            | <span data-ttu-id="0699b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0699b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0699b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0699b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="0699b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0699b-117">Request headers</span></span>

| <span data-ttu-id="0699b-118">名称</span><span class="sxs-lookup"><span data-stu-id="0699b-118">Name</span></span>      |<span data-ttu-id="0699b-119">说明</span><span class="sxs-lookup"><span data-stu-id="0699b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0699b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0699b-120">Authorization</span></span> | <span data-ttu-id="0699b-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0699b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0699b-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="0699b-122">Request body</span></span>

<span data-ttu-id="0699b-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0699b-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0699b-124">响应</span><span class="sxs-lookup"><span data-stu-id="0699b-124">Response</span></span>

<span data-ttu-id="0699b-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationRubric](../resources/educationrubric.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0699b-125">If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0699b-126">示例</span><span class="sxs-lookup"><span data-stu-id="0699b-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0699b-127">请求</span><span class="sxs-lookup"><span data-stu-id="0699b-127">Request</span></span>

<span data-ttu-id="0699b-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0699b-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0699b-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0699b-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubrics"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/rubrics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0699b-130">C#</span><span class="sxs-lookup"><span data-stu-id="0699b-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubrics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0699b-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0699b-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubrics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0699b-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="0699b-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubrics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0699b-133">响应</span><span class="sxs-lookup"><span data-stu-id="0699b-133">Response</span></span>

<span data-ttu-id="0699b-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0699b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0699b-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0699b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "displayName":"Example Credit Rubric",
            "id":"c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
            "description":{
                "content":"This is an example of a credit rubric (no points)",
                "contentType":"text"
            },
            "levels":[
                {
                    "levelId":"dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
                    "displayName":"Good",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                },
                {
                    "levelId":"3f2e4b0f-508e-4005-984b-17e061bc5377",
                    "displayName":"Poor",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                }
            ],
            "qualities":[
                {
                    "qualityId":"dc79dcbf-b536-4797-9c5b-902f28129fd0",
                    "description":{
                        "content":"Argument",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                            "description":{
                                "content":"The essay's argument is persuasive.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                            "description":{
                                "content":"The essay's argument does not make sense.",
                                "contentType":"text"
                            }
                        }
                    ]
                },
                {
                    "qualityId":"7e087062-ac25-4629-8386-a946350936db",
                    "description":{
                        "content":"Spelling and Grammar",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"12276eb2-122c-4ad2-ba92-335ea798c88e",
                            "description":{
                                "content":"The essay uses proper spelling and grammar with few or no errors.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                            "description":{
                                "content":"The essay has numerous errors in spelling and/or grammar.",
                                "contentType":"text"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rubrics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
