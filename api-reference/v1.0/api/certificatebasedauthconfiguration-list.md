---
title: 列出 certificateBasedAuthConfigurations
description: 获取 certificatebasedauthconfiguration 对象的列表。
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c9f3d4dbfab59164c28bbd5b68e57f2728ff207f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035825"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="4ee61-103">列出 certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="4ee61-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="4ee61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ee61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ee61-105">获取 [certificateBasedAuthConfiguration 对象](../resources/certificateBasedAuthConfiguration.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="4ee61-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="4ee61-106">集合中只能存在一个 certificateBasedAuthConfiguration 实例。</span><span class="sxs-lookup"><span data-stu-id="4ee61-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="4ee61-107">它始终具有值为"29728ade-6ae4-4ee9-9103-412912537da5"的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="4ee61-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ee61-108">权限</span><span class="sxs-lookup"><span data-stu-id="4ee61-108">Permissions</span></span>

<span data-ttu-id="4ee61-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ee61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ee61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ee61-111">Permission type</span></span>                        | <span data-ttu-id="4ee61-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ee61-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4ee61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ee61-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ee61-114">Organization.Read.All、Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee61-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="4ee61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ee61-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ee61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ee61-116">Not supported.</span></span> |
| <span data-ttu-id="4ee61-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ee61-117">Application</span></span>    | <span data-ttu-id="4ee61-118">Organization.Read.All、Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee61-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ee61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ee61-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="4ee61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ee61-120">Request headers</span></span>

| <span data-ttu-id="4ee61-121">名称</span><span class="sxs-lookup"><span data-stu-id="4ee61-121">Name</span></span>      |<span data-ttu-id="4ee61-122">说明</span><span class="sxs-lookup"><span data-stu-id="4ee61-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ee61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ee61-123">Authorization</span></span> | <span data-ttu-id="4ee61-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ee61-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ee61-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ee61-126">Request body</span></span>

<span data-ttu-id="4ee61-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ee61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ee61-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ee61-128">Response</span></span>

<span data-ttu-id="4ee61-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ee61-129">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ee61-130">示例</span><span class="sxs-lookup"><span data-stu-id="4ee61-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ee61-131">请求</span><span class="sxs-lookup"><span data-stu-id="4ee61-131">Request</span></span>

<span data-ttu-id="4ee61-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ee61-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ee61-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ee61-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="4ee61-134">C#</span><span class="sxs-lookup"><span data-stu-id="4ee61-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ee61-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ee61-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ee61-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ee61-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ee61-137">Java</span><span class="sxs-lookup"><span data-stu-id="4ee61-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="4ee61-138">响应</span><span class="sxs-lookup"><span data-stu-id="4ee61-138">Response</span></span>

<span data-ttu-id="4ee61-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ee61-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4ee61-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ee61-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "certificateAuthorities": [
        {
          "isRootAuthority": true,
          "certificateRevocationListUrl": "CRLUrl-value",
          "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
          "certificate": "Binary",
          "issuer": "issuer-value",
          "issuerSki": "issuerSki-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

