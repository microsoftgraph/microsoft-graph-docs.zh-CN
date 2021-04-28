---
title: 列出分配的 tokenLifetimePolicies
description: 列出分配给应用程序的 tokenLifetimePolicies。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 68dac1d77011f0d82c9b786b64a2218a09a82535
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035930"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="b2eb3-103">列出分配的 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b2eb3-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="b2eb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2eb3-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b2eb3-105">列出 [分配给应用程序的 tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) [对象](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2eb3-106">权限</span><span class="sxs-lookup"><span data-stu-id="b2eb3-106">Permissions</span></span>

<span data-ttu-id="b2eb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2eb3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2eb3-109">Permission type</span></span>                        | <span data-ttu-id="b2eb3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2eb3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2eb3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2eb3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2eb3-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2eb3-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b2eb3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2eb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2eb3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-114">Not supported.</span></span> |
| <span data-ttu-id="b2eb3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2eb3-115">Application</span></span>                            | <span data-ttu-id="b2eb3-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2eb3-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2eb3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2eb3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b2eb3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2eb3-118">Request headers</span></span>

| <span data-ttu-id="b2eb3-119">名称</span><span class="sxs-lookup"><span data-stu-id="b2eb3-119">Name</span></span>          | <span data-ttu-id="b2eb3-120">说明</span><span class="sxs-lookup"><span data-stu-id="b2eb3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b2eb3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2eb3-121">Authorization</span></span> | <span data-ttu-id="b2eb3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2eb3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2eb3-124">Request body</span></span>

<span data-ttu-id="b2eb3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2eb3-126">响应</span><span class="sxs-lookup"><span data-stu-id="b2eb3-126">Response</span></span>

<span data-ttu-id="b2eb3-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2eb3-128">示例</span><span class="sxs-lookup"><span data-stu-id="b2eb3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2eb3-129">请求</span><span class="sxs-lookup"><span data-stu-id="b2eb3-129">Request</span></span>

<span data-ttu-id="b2eb3-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b2eb3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2eb3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="b2eb3-132">C#</span><span class="sxs-lookup"><span data-stu-id="b2eb3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2eb3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2eb3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2eb3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2eb3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2eb3-135">Java</span><span class="sxs-lookup"><span data-stu-id="b2eb3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2eb3-136">响应</span><span class="sxs-lookup"><span data-stu-id="b2eb3-136">Response</span></span>

<span data-ttu-id="b2eb3-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b2eb3-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2eb3-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

