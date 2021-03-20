---
title: 删除 featureRolloutPolicy
description: 删除 featureRolloutPolicy 对象。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ac2d8f8acba29db911030718fbb37e4ddfe53093
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955929"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="deb2b-103">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="deb2b-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="deb2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb2b-105">删除 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deb2b-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="deb2b-106">权限</span><span class="sxs-lookup"><span data-stu-id="deb2b-106">Permissions</span></span>

<span data-ttu-id="deb2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deb2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deb2b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="deb2b-109">Permission type</span></span>                        | <span data-ttu-id="deb2b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deb2b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="deb2b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deb2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="deb2b-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb2b-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="deb2b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deb2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deb2b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb2b-114">Not supported.</span></span> |
| <span data-ttu-id="deb2b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="deb2b-115">Application</span></span>                            | <span data-ttu-id="deb2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb2b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="deb2b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deb2b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="deb2b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="deb2b-118">Request headers</span></span>

| <span data-ttu-id="deb2b-119">名称</span><span class="sxs-lookup"><span data-stu-id="deb2b-119">Name</span></span>          | <span data-ttu-id="deb2b-120">说明</span><span class="sxs-lookup"><span data-stu-id="deb2b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="deb2b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb2b-121">Authorization</span></span> | <span data-ttu-id="deb2b-122">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="deb2b-122">Bearer {token}.</span></span> <span data-ttu-id="deb2b-123">必需</span><span class="sxs-lookup"><span data-stu-id="deb2b-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="deb2b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="deb2b-124">Request body</span></span>

<span data-ttu-id="deb2b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="deb2b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deb2b-126">响应</span><span class="sxs-lookup"><span data-stu-id="deb2b-126">Response</span></span>

<span data-ttu-id="deb2b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="deb2b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deb2b-129">示例</span><span class="sxs-lookup"><span data-stu-id="deb2b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deb2b-130">请求</span><span class="sxs-lookup"><span data-stu-id="deb2b-130">Request</span></span>

<span data-ttu-id="deb2b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="deb2b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="deb2b-132">响应</span><span class="sxs-lookup"><span data-stu-id="deb2b-132">Response</span></span>

<span data-ttu-id="deb2b-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="deb2b-133">The following is an example of the response.</span></span>

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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


