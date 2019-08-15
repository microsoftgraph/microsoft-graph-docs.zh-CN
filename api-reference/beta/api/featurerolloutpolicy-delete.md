---
title: 删除 featureRolloutPolicy
description: 删除 featureRolloutPolicy 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: defcc190f67dc7a78a0069445401e6f624a9a878
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419739"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="9f1c7-103">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="9f1c7-103">Delete featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f1c7-104">删除[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-104">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f1c7-105">权限</span><span class="sxs-lookup"><span data-stu-id="9f1c7-105">Permissions</span></span>

<span data-ttu-id="9f1c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f1c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f1c7-108">Permission type</span></span>                        | <span data-ttu-id="9f1c7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f1c7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f1c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f1c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f1c7-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="9f1c7-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="9f1c7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f1c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f1c7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-113">Not supported.</span></span> |
| <span data-ttu-id="9f1c7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f1c7-114">Application</span></span>                            | <span data-ttu-id="9f1c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f1c7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f1c7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f1c7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f1c7-117">Request headers</span></span>

| <span data-ttu-id="9f1c7-118">名称</span><span class="sxs-lookup"><span data-stu-id="9f1c7-118">Name</span></span>          | <span data-ttu-id="9f1c7-119">说明</span><span class="sxs-lookup"><span data-stu-id="9f1c7-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9f1c7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f1c7-120">Authorization</span></span> | <span data-ttu-id="9f1c7-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9f1c7-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f1c7-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f1c7-122">Request body</span></span>

<span data-ttu-id="9f1c7-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f1c7-124">响应</span><span class="sxs-lookup"><span data-stu-id="9f1c7-124">Response</span></span>

<span data-ttu-id="9f1c7-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f1c7-127">示例</span><span class="sxs-lookup"><span data-stu-id="9f1c7-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f1c7-128">请求</span><span class="sxs-lookup"><span data-stu-id="9f1c7-128">Request</span></span>

<span data-ttu-id="9f1c7-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="9f1c7-130">响应</span><span class="sxs-lookup"><span data-stu-id="9f1c7-130">Response</span></span>

<span data-ttu-id="9f1c7-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f1c7-131">The following is an example of the response.</span></span>

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
