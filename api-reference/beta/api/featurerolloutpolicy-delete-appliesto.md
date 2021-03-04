---
title: Remove appliesTo
description: 从功能推出中删除 directoryObject。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4bd3ce83f81a040583fdc3400e8ce808e1a3c8f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436124"
---
# <a name="remove-appliesto"></a><span data-ttu-id="ad804-103">Remove appliesTo</span><span class="sxs-lookup"><span data-stu-id="ad804-103">Remove appliesTo</span></span>

<span data-ttu-id="ad804-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad804-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad804-105">删除[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的 appliesTo，以从功能推出中删除[directoryObject。](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ad804-105">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad804-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ad804-106">Permissions</span></span>

<span data-ttu-id="ad804-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad804-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad804-109">Permission type</span></span>                        | <span data-ttu-id="ad804-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad804-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ad804-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad804-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad804-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="ad804-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="ad804-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad804-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad804-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad804-114">Not supported.</span></span> |
| <span data-ttu-id="ad804-115">Application</span><span class="sxs-lookup"><span data-stu-id="ad804-115">Application</span></span>                            | <span data-ttu-id="ad804-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad804-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad804-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad804-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ad804-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad804-118">Request headers</span></span>

| <span data-ttu-id="ad804-119">名称</span><span class="sxs-lookup"><span data-stu-id="ad804-119">Name</span></span>          | <span data-ttu-id="ad804-120">说明</span><span class="sxs-lookup"><span data-stu-id="ad804-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ad804-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad804-121">Authorization</span></span> | <span data-ttu-id="ad804-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ad804-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad804-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad804-123">Request body</span></span>

<span data-ttu-id="ad804-124">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad804-124">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad804-125">响应</span><span class="sxs-lookup"><span data-stu-id="ad804-125">Response</span></span>

<span data-ttu-id="ad804-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ad804-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad804-128">示例</span><span class="sxs-lookup"><span data-stu-id="ad804-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad804-129">请求</span><span class="sxs-lookup"><span data-stu-id="ad804-129">Request</span></span>

<span data-ttu-id="ad804-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad804-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad804-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad804-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="c"></a>[<span data-ttu-id="ad804-132">C#</span><span class="sxs-lookup"><span data-stu-id="ad804-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad804-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad804-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad804-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad804-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad804-135">Java</span><span class="sxs-lookup"><span data-stu-id="ad804-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad804-136">响应</span><span class="sxs-lookup"><span data-stu-id="ad804-136">Response</span></span>

<span data-ttu-id="ad804-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ad804-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


