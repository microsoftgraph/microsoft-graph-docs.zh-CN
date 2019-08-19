---
title: 删除 educationRubric
description: 删除 educationRubric 对象。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d9d3b67ec4ef0ef8bdd6684489630228355e3d1
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461055"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="9d9f0-103">删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="9d9f0-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d9f0-104">删除[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d9f0-105">权限</span><span class="sxs-lookup"><span data-stu-id="9d9f0-105">Permissions</span></span>

<span data-ttu-id="9d9f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d9f0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d9f0-108">Permission type</span></span>                        | <span data-ttu-id="9d9f0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d9f0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d9f0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d9f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d9f0-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="9d9f0-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9d9f0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d9f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d9f0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-113">Not supported.</span></span> |
| <span data-ttu-id="9d9f0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d9f0-114">Application</span></span>                            | <span data-ttu-id="9d9f0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d9f0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d9f0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d9f0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d9f0-117">Request headers</span></span>

| <span data-ttu-id="9d9f0-118">名称</span><span class="sxs-lookup"><span data-stu-id="9d9f0-118">Name</span></span>          | <span data-ttu-id="9d9f0-119">说明</span><span class="sxs-lookup"><span data-stu-id="9d9f0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9d9f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d9f0-120">Authorization</span></span> | <span data-ttu-id="9d9f0-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9d9f0-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d9f0-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d9f0-122">Request body</span></span>

<span data-ttu-id="9d9f0-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d9f0-124">响应</span><span class="sxs-lookup"><span data-stu-id="9d9f0-124">Response</span></span>

<span data-ttu-id="9d9f0-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d9f0-127">示例</span><span class="sxs-lookup"><span data-stu-id="9d9f0-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d9f0-128">请求</span><span class="sxs-lookup"><span data-stu-id="9d9f0-128">Request</span></span>

<span data-ttu-id="9d9f0-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d9f0-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9d9f0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d9f0-131">C#</span><span class="sxs-lookup"><span data-stu-id="9d9f0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d9f0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d9f0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d9f0-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="9d9f0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d9f0-134">响应</span><span class="sxs-lookup"><span data-stu-id="9d9f0-134">Response</span></span>

<span data-ttu-id="9d9f0-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d9f0-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
