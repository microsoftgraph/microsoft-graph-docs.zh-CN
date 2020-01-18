---
title: 删除 tokenLifetimePolicy
description: 删除 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb4944beb5057bec0098556f81292f4ed9202910
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234173"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="26322-103">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="26322-103">Delete tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26322-104">删除[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26322-104">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26322-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="26322-105">Permissions</span></span>

<span data-ttu-id="26322-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26322-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="26322-108">Permission type</span></span>                        | <span data-ttu-id="26322-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26322-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26322-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26322-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="26322-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="26322-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="26322-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26322-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26322-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="26322-113">Not supported.</span></span> |
| <span data-ttu-id="26322-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="26322-114">Application</span></span>                            | <span data-ttu-id="26322-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="26322-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="26322-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26322-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26322-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="26322-117">Request headers</span></span>

| <span data-ttu-id="26322-118">名称</span><span class="sxs-lookup"><span data-stu-id="26322-118">Name</span></span>          | <span data-ttu-id="26322-119">说明</span><span class="sxs-lookup"><span data-stu-id="26322-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26322-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="26322-120">Authorization</span></span> | <span data-ttu-id="26322-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="26322-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26322-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="26322-122">Request body</span></span>

<span data-ttu-id="26322-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26322-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26322-124">响应</span><span class="sxs-lookup"><span data-stu-id="26322-124">Response</span></span>

<span data-ttu-id="26322-125">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="26322-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26322-126">示例</span><span class="sxs-lookup"><span data-stu-id="26322-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26322-127">请求</span><span class="sxs-lookup"><span data-stu-id="26322-127">Request</span></span>

<span data-ttu-id="26322-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26322-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="26322-129">响应</span><span class="sxs-lookup"><span data-stu-id="26322-129">Response</span></span>

<span data-ttu-id="26322-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26322-130">The following is an example of the response.</span></span>

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
  "description": "Delete tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->