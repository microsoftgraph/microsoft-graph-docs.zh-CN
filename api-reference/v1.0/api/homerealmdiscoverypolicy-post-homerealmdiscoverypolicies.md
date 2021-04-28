---
title: 创建 homeRealmDiscoveryPolicy
description: 创建新的 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 31b201ea19658361cdb2bf7c3da2326c3e710e29
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051387"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="03f31-103">创建 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="03f31-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="03f31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03f31-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="03f31-105">创建新的 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03f31-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03f31-106">权限</span><span class="sxs-lookup"><span data-stu-id="03f31-106">Permissions</span></span>

<span data-ttu-id="03f31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03f31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="03f31-109">Permission type</span></span>                        | <span data-ttu-id="03f31-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03f31-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03f31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03f31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03f31-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="03f31-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="03f31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03f31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03f31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="03f31-114">Not supported.</span></span> |
| <span data-ttu-id="03f31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="03f31-115">Application</span></span>                            | <span data-ttu-id="03f31-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="03f31-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="03f31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03f31-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="03f31-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="03f31-118">Request headers</span></span>

| <span data-ttu-id="03f31-119">名称</span><span class="sxs-lookup"><span data-stu-id="03f31-119">Name</span></span>          | <span data-ttu-id="03f31-120">说明</span><span class="sxs-lookup"><span data-stu-id="03f31-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03f31-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03f31-121">Authorization</span></span> | <span data-ttu-id="03f31-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03f31-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03f31-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="03f31-124">Content-type</span></span> | <span data-ttu-id="03f31-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="03f31-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03f31-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03f31-127">Request body</span></span>

<span data-ttu-id="03f31-128">在请求正文中，提供 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03f31-128">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03f31-129">响应</span><span class="sxs-lookup"><span data-stu-id="03f31-129">Response</span></span>

<span data-ttu-id="03f31-130">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03f31-130">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03f31-131">示例</span><span class="sxs-lookup"><span data-stu-id="03f31-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03f31-132">请求</span><span class="sxs-lookup"><span data-stu-id="03f31-132">Request</span></span>

<span data-ttu-id="03f31-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03f31-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03f31-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="03f31-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="03f31-135">C#</span><span class="sxs-lookup"><span data-stu-id="03f31-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03f31-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03f31-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03f31-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03f31-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03f31-138">Java</span><span class="sxs-lookup"><span data-stu-id="03f31-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03f31-139">响应</span><span class="sxs-lookup"><span data-stu-id="03f31-139">Response</span></span>

<span data-ttu-id="03f31-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="03f31-140">The following is an example of the response.</span></span>

> <span data-ttu-id="03f31-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03f31-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

