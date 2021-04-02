---
title: Remove appliesTo
description: 从功能推出中删除 directoryObject。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7952b8cc3360c8332c4e5ed6a7a5635d5d7e0e2c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508701"
---
# <a name="remove-appliesto"></a><span data-ttu-id="a0ef1-103">Remove appliesTo</span><span class="sxs-lookup"><span data-stu-id="a0ef1-103">Remove appliesTo</span></span>

<span data-ttu-id="a0ef1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0ef1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ef1-105">删除[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的 appliesTo 以从功能推出中删除[directoryObject。](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a0ef1-105">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0ef1-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0ef1-106">Permissions</span></span>

<span data-ttu-id="a0ef1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0ef1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0ef1-109">Permission type</span></span>                        | <span data-ttu-id="a0ef1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0ef1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0ef1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0ef1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0ef1-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ef1-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="a0ef1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0ef1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ef1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-114">Not supported.</span></span> |
| <span data-ttu-id="a0ef1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0ef1-115">Application</span></span>                            | <span data-ttu-id="a0ef1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0ef1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0ef1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{policyId}/appliesTo/{directoryObjectId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a0ef1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0ef1-118">Request headers</span></span>

| <span data-ttu-id="a0ef1-119">名称</span><span class="sxs-lookup"><span data-stu-id="a0ef1-119">Name</span></span>          | <span data-ttu-id="a0ef1-120">说明</span><span class="sxs-lookup"><span data-stu-id="a0ef1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a0ef1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0ef1-121">Authorization</span></span> | <span data-ttu-id="a0ef1-122">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-122">Bearer {token}.</span></span> <span data-ttu-id="a0ef1-123">必需</span><span class="sxs-lookup"><span data-stu-id="a0ef1-123">Required</span></span> |

## <a name="response"></a><span data-ttu-id="a0ef1-124">响应</span><span class="sxs-lookup"><span data-stu-id="a0ef1-124">Response</span></span>

<span data-ttu-id="a0ef1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0ef1-127">示例</span><span class="sxs-lookup"><span data-stu-id="a0ef1-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0ef1-128">请求</span><span class="sxs-lookup"><span data-stu-id="a0ef1-128">Request</span></span>

<span data-ttu-id="a0ef1-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a0ef1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0ef1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="c"></a>[<span data-ttu-id="a0ef1-131">C#</span><span class="sxs-lookup"><span data-stu-id="a0ef1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0ef1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0ef1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0ef1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0ef1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0ef1-134">Java</span><span class="sxs-lookup"><span data-stu-id="a0ef1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0ef1-135">响应</span><span class="sxs-lookup"><span data-stu-id="a0ef1-135">Response</span></span>

<span data-ttu-id="a0ef1-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0ef1-136">The following is an example of the response.</span></span>

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


