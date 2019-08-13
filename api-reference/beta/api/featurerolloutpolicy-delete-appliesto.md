---
title: 删除 appliesTo
description: 从功能推出中删除 directoryObject。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9d1c6046ab108313cf040293e66209f4492f45
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325251"
---
# <a name="remove-appliesto"></a><span data-ttu-id="70aa5-103">删除 appliesTo</span><span class="sxs-lookup"><span data-stu-id="70aa5-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70aa5-104">删除[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象上的 appliesTo, 以从功能展示中删除[directoryObject](../resources/directoryobject.md) 。</span><span class="sxs-lookup"><span data-stu-id="70aa5-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="70aa5-105">权限</span><span class="sxs-lookup"><span data-stu-id="70aa5-105">Permissions</span></span>

<span data-ttu-id="70aa5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70aa5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="70aa5-108">Permission type</span></span>                        | <span data-ttu-id="70aa5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70aa5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="70aa5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70aa5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="70aa5-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="70aa5-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="70aa5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70aa5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70aa5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="70aa5-113">Not supported.</span></span> |
| <span data-ttu-id="70aa5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="70aa5-114">Application</span></span>                            | <span data-ttu-id="70aa5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70aa5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70aa5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70aa5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="70aa5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="70aa5-117">Request headers</span></span>

| <span data-ttu-id="70aa5-118">名称</span><span class="sxs-lookup"><span data-stu-id="70aa5-118">Name</span></span>          | <span data-ttu-id="70aa5-119">说明</span><span class="sxs-lookup"><span data-stu-id="70aa5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="70aa5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="70aa5-120">Authorization</span></span> | <span data-ttu-id="70aa5-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="70aa5-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="70aa5-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="70aa5-122">Request body</span></span>

<span data-ttu-id="70aa5-123">在请求正文中, 提供[directoryObject](../resources/directoryobject.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70aa5-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="70aa5-124">响应</span><span class="sxs-lookup"><span data-stu-id="70aa5-124">Response</span></span>

<span data-ttu-id="70aa5-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="70aa5-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70aa5-127">示例</span><span class="sxs-lookup"><span data-stu-id="70aa5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70aa5-128">请求</span><span class="sxs-lookup"><span data-stu-id="70aa5-128">Request</span></span>

<span data-ttu-id="70aa5-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70aa5-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="70aa5-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="70aa5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70aa5-131">C#</span><span class="sxs-lookup"><span data-stu-id="70aa5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70aa5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70aa5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70aa5-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="70aa5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70aa5-134">Java</span><span class="sxs-lookup"><span data-stu-id="70aa5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70aa5-135">响应</span><span class="sxs-lookup"><span data-stu-id="70aa5-135">Response</span></span>

<span data-ttu-id="70aa5-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70aa5-136">The following is an example of the response.</span></span>

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
