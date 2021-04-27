---
title: 创建 tokenLifetimePolicy
description: 创建新的 tokenLifetimePolicy。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d14b289f640c7ab2ca0b7e335d6f7b87c22eb536
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051758"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="e931d-103">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e931d-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="e931d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e931d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e931d-105">创建新的 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e931d-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e931d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e931d-106">Permissions</span></span>

<span data-ttu-id="e931d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e931d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e931d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e931d-109">Permission type</span></span>                        | <span data-ttu-id="e931d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e931d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e931d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e931d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e931d-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e931d-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="e931d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e931d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e931d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e931d-114">Not supported.</span></span> |
| <span data-ttu-id="e931d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e931d-115">Application</span></span>                            | <span data-ttu-id="e931d-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e931d-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="e931d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e931d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e931d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e931d-118">Request headers</span></span>

| <span data-ttu-id="e931d-119">名称</span><span class="sxs-lookup"><span data-stu-id="e931d-119">Name</span></span>          | <span data-ttu-id="e931d-120">说明</span><span class="sxs-lookup"><span data-stu-id="e931d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e931d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e931d-121">Authorization</span></span> | <span data-ttu-id="e931d-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e931d-122">Bearer {token}</span></span> |
| <span data-ttu-id="e931d-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="e931d-123">Content-type</span></span> | <span data-ttu-id="e931d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e931d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e931d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e931d-125">Request body</span></span>

<span data-ttu-id="e931d-126">在请求正文中，提供 [tokenLifetimePolicy 对象的](../resources/tokenlifetimepolicy.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e931d-126">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e931d-127">响应</span><span class="sxs-lookup"><span data-stu-id="e931d-127">Response</span></span>

<span data-ttu-id="e931d-128">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e931d-128">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e931d-129">示例</span><span class="sxs-lookup"><span data-stu-id="e931d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e931d-130">请求</span><span class="sxs-lookup"><span data-stu-id="e931d-130">Request</span></span>

<span data-ttu-id="e931d-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e931d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e931d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e931d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="e931d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e931d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e931d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e931d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e931d-135">C#</span><span class="sxs-lookup"><span data-stu-id="e931d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e931d-136">Java</span><span class="sxs-lookup"><span data-stu-id="e931d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e931d-137">响应</span><span class="sxs-lookup"><span data-stu-id="e931d-137">Response</span></span>

<span data-ttu-id="e931d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e931d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="e931d-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e931d-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


