---
title: 删除 featureRolloutPolicy
description: 删除 featureRolloutPolicy 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 305ab5e58c0f51997890e9f0387fe450189824cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421751"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="2fa0a-103">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="2fa0a-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="2fa0a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2fa0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fa0a-105">删除[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fa0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fa0a-106">Permissions</span></span>

<span data-ttu-id="2fa0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fa0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fa0a-109">Permission type</span></span>                        | <span data-ttu-id="2fa0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fa0a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2fa0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fa0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fa0a-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="2fa0a-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="2fa0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fa0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fa0a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-114">Not supported.</span></span> |
| <span data-ttu-id="2fa0a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fa0a-115">Application</span></span>                            | <span data-ttu-id="2fa0a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fa0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fa0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2fa0a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fa0a-118">Request headers</span></span>

| <span data-ttu-id="2fa0a-119">名称</span><span class="sxs-lookup"><span data-stu-id="2fa0a-119">Name</span></span>          | <span data-ttu-id="2fa0a-120">说明</span><span class="sxs-lookup"><span data-stu-id="2fa0a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2fa0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fa0a-121">Authorization</span></span> | <span data-ttu-id="2fa0a-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2fa0a-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fa0a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fa0a-123">Request body</span></span>

<span data-ttu-id="2fa0a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fa0a-125">响应</span><span class="sxs-lookup"><span data-stu-id="2fa0a-125">Response</span></span>

<span data-ttu-id="2fa0a-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2fa0a-128">示例</span><span class="sxs-lookup"><span data-stu-id="2fa0a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2fa0a-129">请求</span><span class="sxs-lookup"><span data-stu-id="2fa0a-129">Request</span></span>

<span data-ttu-id="2fa0a-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="2fa0a-131">响应</span><span class="sxs-lookup"><span data-stu-id="2fa0a-131">Response</span></span>

<span data-ttu-id="2fa0a-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2fa0a-132">The following is an example of the response.</span></span>

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
