---
title: trustFrameworkKeySet： getActiveKey
description: 获取键集中的活动键。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: befdd0ba66a7650774a73b5e2b4e3e09c5859bd2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051744"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="eee07-103">trustFrameworkKeySet： getActiveKey</span><span class="sxs-lookup"><span data-stu-id="eee07-103">trustFrameworkKeySet: getActiveKey</span></span>

<span data-ttu-id="eee07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee07-105">获取[trustFrameworkKeySet](../resources/trustframeworkkey.md)中的当前活动的[trustFrameworkKey。](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="eee07-105">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="eee07-106">一次只有一个键在键集内处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="eee07-106">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="eee07-107">权限</span><span class="sxs-lookup"><span data-stu-id="eee07-107">Permissions</span></span>

<span data-ttu-id="eee07-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eee07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eee07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eee07-110">Permission type</span></span>                        | <span data-ttu-id="eee07-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eee07-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eee07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eee07-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eee07-113">TrustFrameworkKeySet.Read.All、TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eee07-113">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="eee07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eee07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eee07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eee07-115">Not supported.</span></span> |
| <span data-ttu-id="eee07-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eee07-116">Application</span></span>                            | <span data-ttu-id="eee07-117">TrustFrameworkKeySet.Read.All、TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eee07-117">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eee07-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eee07-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="eee07-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eee07-119">Request headers</span></span>

| <span data-ttu-id="eee07-120">名称</span><span class="sxs-lookup"><span data-stu-id="eee07-120">Name</span></span>          | <span data-ttu-id="eee07-121">说明</span><span class="sxs-lookup"><span data-stu-id="eee07-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eee07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eee07-122">Authorization</span></span> | <span data-ttu-id="eee07-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eee07-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eee07-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eee07-125">Request body</span></span>

<span data-ttu-id="eee07-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eee07-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eee07-127">响应</span><span class="sxs-lookup"><span data-stu-id="eee07-127">Response</span></span>

<span data-ttu-id="eee07-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eee07-128">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eee07-129">示例</span><span class="sxs-lookup"><span data-stu-id="eee07-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eee07-130">请求</span><span class="sxs-lookup"><span data-stu-id="eee07-130">Request</span></span>

<span data-ttu-id="eee07-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eee07-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eee07-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="eee07-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="c"></a>[<span data-ttu-id="eee07-133">C#</span><span class="sxs-lookup"><span data-stu-id="eee07-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eee07-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eee07-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eee07-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eee07-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eee07-136">Java</span><span class="sxs-lookup"><span data-stu-id="eee07-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-getactivekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eee07-137">响应</span><span class="sxs-lookup"><span data-stu-id="eee07-137">Response</span></span>

<span data-ttu-id="eee07-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eee07-138">The following is an example of the response.</span></span>

> <span data-ttu-id="eee07-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eee07-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "k": "k-value",
  "x5c": [
    "x5c-value"
  ],
  "x5t": "x5t-value",
  "kty": "kty-value",
  "use": "use-value",
  "exp": 99
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: getActiveKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


