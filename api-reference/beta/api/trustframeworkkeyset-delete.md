---
title: 删除 trustFrameworkKeySet
description: 删除**trustFrameworkKeySet**对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad73363f568c97be720cdcab3711e762b8dcde1a
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734549"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="cd154-103">删除 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="cd154-103">Delete trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd154-104">删除[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="cd154-104">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd154-105">权限</span><span class="sxs-lookup"><span data-stu-id="cd154-105">Permissions</span></span>

<span data-ttu-id="cd154-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd154-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd154-108">Permission type</span></span>                        | <span data-ttu-id="cd154-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd154-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cd154-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd154-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd154-111">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="cd154-111">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="cd154-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd154-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd154-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd154-113">Not supported.</span></span> |
| <span data-ttu-id="cd154-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd154-114">Application</span></span>                            | <span data-ttu-id="cd154-115">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="cd154-115">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd154-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd154-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cd154-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd154-117">Request headers</span></span>

| <span data-ttu-id="cd154-118">名称</span><span class="sxs-lookup"><span data-stu-id="cd154-118">Name</span></span>          | <span data-ttu-id="cd154-119">说明</span><span class="sxs-lookup"><span data-stu-id="cd154-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cd154-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd154-120">Authorization</span></span> | <span data-ttu-id="cd154-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd154-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd154-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd154-123">Request body</span></span>

<span data-ttu-id="cd154-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd154-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd154-125">响应</span><span class="sxs-lookup"><span data-stu-id="cd154-125">Response</span></span>

<span data-ttu-id="cd154-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cd154-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd154-128">示例</span><span class="sxs-lookup"><span data-stu-id="cd154-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd154-129">请求</span><span class="sxs-lookup"><span data-stu-id="cd154-129">Request</span></span>

<span data-ttu-id="cd154-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cd154-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```

### <a name="response"></a><span data-ttu-id="cd154-131">响应</span><span class="sxs-lookup"><span data-stu-id="cd154-131">Response</span></span>

<span data-ttu-id="cd154-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cd154-132">The following is an example of the response.</span></span>

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
  "description": "Delete trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
