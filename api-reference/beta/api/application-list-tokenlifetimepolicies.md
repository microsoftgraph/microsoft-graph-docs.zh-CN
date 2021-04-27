---
title: 列出分配的 tokenLifetimePolicies
description: 列出分配给应用程序或 servicePrincipal 的 tokenLifetimePolicies。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 77216d297c108871ef8be7543e10d7f263d53d34
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048097"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="bd9b6-103">列出分配的 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="bd9b6-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="bd9b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd9b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd9b6-105">列出分配给应用程序或[servicePrincipal](../resources/servicePrincipal.md)的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。 [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="bd9b6-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="bd9b6-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd9b6-106">Permissions</span></span>

<span data-ttu-id="bd9b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd9b6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd9b6-109">Permission type</span></span>                        | <span data-ttu-id="bd9b6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd9b6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd9b6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd9b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd9b6-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9b6-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="bd9b6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd9b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd9b6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-114">Not supported.</span></span> |
| <span data-ttu-id="bd9b6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd9b6-115">Application</span></span>                            | <span data-ttu-id="bd9b6-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9b6-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd9b6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd9b6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bd9b6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd9b6-118">Request headers</span></span>

| <span data-ttu-id="bd9b6-119">名称</span><span class="sxs-lookup"><span data-stu-id="bd9b6-119">Name</span></span>          | <span data-ttu-id="bd9b6-120">说明</span><span class="sxs-lookup"><span data-stu-id="bd9b6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd9b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd9b6-121">Authorization</span></span> | <span data-ttu-id="bd9b6-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="bd9b6-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd9b6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd9b6-123">Request body</span></span>

<span data-ttu-id="bd9b6-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd9b6-125">响应</span><span class="sxs-lookup"><span data-stu-id="bd9b6-125">Response</span></span>

<span data-ttu-id="bd9b6-126">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-126">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd9b6-127">示例</span><span class="sxs-lookup"><span data-stu-id="bd9b6-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd9b6-128">请求</span><span class="sxs-lookup"><span data-stu-id="bd9b6-128">Request</span></span>

<span data-ttu-id="bd9b6-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd9b6-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd9b6-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="bd9b6-131">C#</span><span class="sxs-lookup"><span data-stu-id="bd9b6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd9b6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd9b6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd9b6-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd9b6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd9b6-134">Java</span><span class="sxs-lookup"><span data-stu-id="bd9b6-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd9b6-135">响应</span><span class="sxs-lookup"><span data-stu-id="bd9b6-135">Response</span></span>

<span data-ttu-id="bd9b6-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-136">The following is an example of the response.</span></span>

> <span data-ttu-id="bd9b6-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bd9b6-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



