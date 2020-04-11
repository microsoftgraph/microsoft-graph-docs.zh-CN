---
title: 删除 tokenLifetimePolicy
description: 删除 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06b6994af764462d91cd9ee818d5b590c0bc620d
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229652"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="a811b-103">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a811b-103">Delete tokenLifetimePolicy</span></span>

<span data-ttu-id="a811b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a811b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a811b-105">删除[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a811b-105">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a811b-106">权限</span><span class="sxs-lookup"><span data-stu-id="a811b-106">Permissions</span></span>

<span data-ttu-id="a811b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a811b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a811b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a811b-109">Permission type</span></span>                        | <span data-ttu-id="a811b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a811b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a811b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a811b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a811b-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a811b-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a811b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a811b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a811b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a811b-114">Not supported.</span></span> |
| <span data-ttu-id="a811b-115">Application</span><span class="sxs-lookup"><span data-stu-id="a811b-115">Application</span></span>                            | <span data-ttu-id="a811b-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a811b-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a811b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a811b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a811b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a811b-118">Request headers</span></span>

| <span data-ttu-id="a811b-119">名称</span><span class="sxs-lookup"><span data-stu-id="a811b-119">Name</span></span>          | <span data-ttu-id="a811b-120">说明</span><span class="sxs-lookup"><span data-stu-id="a811b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a811b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a811b-121">Authorization</span></span> | <span data-ttu-id="a811b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a811b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a811b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a811b-124">Request body</span></span>

<span data-ttu-id="a811b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a811b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a811b-126">响应</span><span class="sxs-lookup"><span data-stu-id="a811b-126">Response</span></span>

<span data-ttu-id="a811b-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a811b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a811b-128">示例</span><span class="sxs-lookup"><span data-stu-id="a811b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a811b-129">请求</span><span class="sxs-lookup"><span data-stu-id="a811b-129">Request</span></span>

<span data-ttu-id="a811b-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a811b-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="a811b-131">响应</span><span class="sxs-lookup"><span data-stu-id="a811b-131">Response</span></span>

<span data-ttu-id="a811b-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a811b-132">The following is an example of the response.</span></span>

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
