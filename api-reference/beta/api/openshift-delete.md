---
title: 删除 openShift
description: 删除 openShift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a65239af849e8cb54102760c077f9fa525516c1
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153511"
---
# <a name="delete-openshift"></a><span data-ttu-id="b6f3e-103">删除 openShift</span><span class="sxs-lookup"><span data-stu-id="b6f3e-103">Delete openShift</span></span>

<span data-ttu-id="b6f3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6f3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6f3e-105">删除[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6f3e-106">权限</span><span class="sxs-lookup"><span data-stu-id="b6f3e-106">Permissions</span></span>

<span data-ttu-id="b6f3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6f3e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6f3e-109">Permission type</span></span>                        | <span data-ttu-id="b6f3e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6f3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b6f3e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6f3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6f3e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f3e-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b6f3e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6f3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-114">Not supported.</span></span> |
| <span data-ttu-id="b6f3e-115">Application</span><span class="sxs-lookup"><span data-stu-id="b6f3e-115">Application</span></span>                            | <span data-ttu-id="b6f3e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6f3e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6f3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b6f3e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6f3e-118">Request headers</span></span>

| <span data-ttu-id="b6f3e-119">名称</span><span class="sxs-lookup"><span data-stu-id="b6f3e-119">Name</span></span>          | <span data-ttu-id="b6f3e-120">说明</span><span class="sxs-lookup"><span data-stu-id="b6f3e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b6f3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6f3e-121">Authorization</span></span> | <span data-ttu-id="b6f3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6f3e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6f3e-124">Request body</span></span>

<span data-ttu-id="b6f3e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f3e-126">响应</span><span class="sxs-lookup"><span data-stu-id="b6f3e-126">Response</span></span>

<span data-ttu-id="b6f3e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6f3e-129">示例</span><span class="sxs-lookup"><span data-stu-id="b6f3e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6f3e-130">请求</span><span class="sxs-lookup"><span data-stu-id="b6f3e-130">Request</span></span>

<span data-ttu-id="b6f3e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6f3e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f3e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="b6f3e-133">C#</span><span class="sxs-lookup"><span data-stu-id="b6f3e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6f3e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6f3e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6f3e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6f3e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6f3e-136">响应</span><span class="sxs-lookup"><span data-stu-id="b6f3e-136">Response</span></span>

<span data-ttu-id="b6f3e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b6f3e-137">The following is an example of the response.</span></span>

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
