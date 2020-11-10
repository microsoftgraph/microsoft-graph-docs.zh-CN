---
title: 删除 openShift
description: 删除 openShift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70fd651899010c827a2fbfed70776c5a1fe07a6b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962821"
---
# <a name="delete-openshift"></a><span data-ttu-id="cf0cf-103">删除 openShift</span><span class="sxs-lookup"><span data-stu-id="cf0cf-103">Delete openShift</span></span>

<span data-ttu-id="cf0cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf0cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf0cf-105">删除 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf0cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf0cf-106">Permissions</span></span>

<span data-ttu-id="cf0cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf0cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf0cf-109">Permission type</span></span>                        | <span data-ttu-id="cf0cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf0cf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf0cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf0cf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf0cf-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf0cf-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cf0cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf0cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf0cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-114">Not supported.</span></span> |
| <span data-ttu-id="cf0cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf0cf-115">Application</span></span>                            | <span data-ttu-id="cf0cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf0cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf0cf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="cf0cf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf0cf-118">Request headers</span></span>

| <span data-ttu-id="cf0cf-119">名称</span><span class="sxs-lookup"><span data-stu-id="cf0cf-119">Name</span></span>          | <span data-ttu-id="cf0cf-120">说明</span><span class="sxs-lookup"><span data-stu-id="cf0cf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cf0cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf0cf-121">Authorization</span></span> | <span data-ttu-id="cf0cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf0cf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf0cf-124">Request body</span></span>

<span data-ttu-id="cf0cf-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf0cf-126">响应</span><span class="sxs-lookup"><span data-stu-id="cf0cf-126">Response</span></span>

<span data-ttu-id="cf0cf-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf0cf-129">示例</span><span class="sxs-lookup"><span data-stu-id="cf0cf-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf0cf-130">请求</span><span class="sxs-lookup"><span data-stu-id="cf0cf-130">Request</span></span>

<span data-ttu-id="cf0cf-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf0cf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf0cf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="cf0cf-133">C#</span><span class="sxs-lookup"><span data-stu-id="cf0cf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf0cf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf0cf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf0cf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf0cf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf0cf-136">Java</span><span class="sxs-lookup"><span data-stu-id="cf0cf-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf0cf-137">响应</span><span class="sxs-lookup"><span data-stu-id="cf0cf-137">Response</span></span>

<span data-ttu-id="cf0cf-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf0cf-138">The following is an example of the response.</span></span>

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
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


