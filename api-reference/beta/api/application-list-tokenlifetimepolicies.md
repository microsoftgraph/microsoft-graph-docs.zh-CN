---
title: 列表已分配 tokenLifetimePolicies
description: 列出分配给应用程序或 servicePrincipal 的 tokenLifetimePolicies。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1aab750ef0d2121634343ef9c371bae1645744e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441499"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="b96af-103">列表已分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b96af-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="b96af-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b96af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b96af-105">列出分配给[应用程序](../resources/application.md)或[servicePrincipal](../resources/servicePrincipal.md)的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。。</span><span class="sxs-lookup"><span data-stu-id="b96af-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="b96af-106">权限</span><span class="sxs-lookup"><span data-stu-id="b96af-106">Permissions</span></span>

<span data-ttu-id="b96af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b96af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b96af-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b96af-109">Permission type</span></span>                        | <span data-ttu-id="b96af-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b96af-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b96af-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b96af-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b96af-112">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="b96af-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b96af-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b96af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b96af-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b96af-114">Not supported.</span></span> |
| <span data-ttu-id="b96af-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b96af-115">Application</span></span>                            | <span data-ttu-id="b96af-116">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="b96af-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b96af-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b96af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b96af-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b96af-118">Request headers</span></span>

| <span data-ttu-id="b96af-119">名称</span><span class="sxs-lookup"><span data-stu-id="b96af-119">Name</span></span>          | <span data-ttu-id="b96af-120">说明</span><span class="sxs-lookup"><span data-stu-id="b96af-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b96af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b96af-121">Authorization</span></span> | <span data-ttu-id="b96af-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b96af-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b96af-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b96af-123">Request body</span></span>

<span data-ttu-id="b96af-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b96af-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b96af-125">响应</span><span class="sxs-lookup"><span data-stu-id="b96af-125">Response</span></span>

<span data-ttu-id="b96af-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[tokenLifetimePolicy](../resources/tokenLifetimePolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b96af-126">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b96af-127">示例</span><span class="sxs-lookup"><span data-stu-id="b96af-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b96af-128">请求</span><span class="sxs-lookup"><span data-stu-id="b96af-128">Request</span></span>

<span data-ttu-id="b96af-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b96af-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b96af-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b96af-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="b96af-131">C#</span><span class="sxs-lookup"><span data-stu-id="b96af-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b96af-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b96af-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b96af-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b96af-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b96af-134">响应</span><span class="sxs-lookup"><span data-stu-id="b96af-134">Response</span></span>

<span data-ttu-id="b96af-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b96af-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b96af-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b96af-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
