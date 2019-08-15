---
title: 删除 educationCategory
description: 删除现有类别。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8443ab8de0afda3eb7c014946973f180b94d14eb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416469"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="7bcaf-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="7bcaf-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bcaf-104">删除现有类别。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bcaf-105">权限</span><span class="sxs-lookup"><span data-stu-id="7bcaf-105">Permissions</span></span>

<span data-ttu-id="7bcaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bcaf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bcaf-108">Permission type</span></span>                        | <span data-ttu-id="7bcaf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7bcaf-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="7bcaf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bcaf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bcaf-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="7bcaf-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7bcaf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bcaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bcaf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-113">Not Supported.</span></span>                                          |
| <span data-ttu-id="7bcaf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bcaf-114">Application</span></span>                            | <span data-ttu-id="7bcaf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-115">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="7bcaf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bcaf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7bcaf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bcaf-117">Request headers</span></span>

| <span data-ttu-id="7bcaf-118">标头</span><span class="sxs-lookup"><span data-stu-id="7bcaf-118">Header</span></span>        | <span data-ttu-id="7bcaf-119">值</span><span class="sxs-lookup"><span data-stu-id="7bcaf-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7bcaf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bcaf-120">Authorization</span></span> | <span data-ttu-id="7bcaf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bcaf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bcaf-123">Request body</span></span>

<span data-ttu-id="7bcaf-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bcaf-125">响应</span><span class="sxs-lookup"><span data-stu-id="7bcaf-125">Response</span></span>

<span data-ttu-id="7bcaf-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bcaf-128">示例</span><span class="sxs-lookup"><span data-stu-id="7bcaf-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bcaf-129">请求</span><span class="sxs-lookup"><span data-stu-id="7bcaf-129">Request</span></span>

<span data-ttu-id="7bcaf-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7bcaf-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7bcaf-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bcaf-132">C#</span><span class="sxs-lookup"><span data-stu-id="7bcaf-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bcaf-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bcaf-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bcaf-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="7bcaf-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bcaf-135">响应</span><span class="sxs-lookup"><span data-stu-id="7bcaf-135">Response</span></span>

<span data-ttu-id="7bcaf-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7bcaf-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
