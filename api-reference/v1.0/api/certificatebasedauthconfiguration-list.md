---
title: 列出 certificateBasedAuthConfigurations
description: 获取 certificatebasedauthconfiguration 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f045eee24c9c4150419e69adc7279987206510d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518628"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="ea3f4-103">列出 certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="ea3f4-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="ea3f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea3f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea3f4-105">获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="ea3f4-106">集合中只能存在一个 certificateBasedAuthConfiguration 实例。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="ea3f4-107">它始终具有值为 "29728ade-6ae4-4ee9-9103-412912537da5" 的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea3f4-108">权限</span><span class="sxs-lookup"><span data-stu-id="ea3f4-108">Permissions</span></span>

<span data-ttu-id="ea3f4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea3f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea3f4-111">Permission type</span></span>                        | <span data-ttu-id="ea3f4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea3f4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ea3f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea3f4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea3f4-114">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="ea3f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea3f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea3f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-116">Not supported.</span></span> |
| <span data-ttu-id="ea3f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea3f4-117">Application</span></span>    | <span data-ttu-id="ea3f4-118">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea3f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea3f4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="ea3f4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea3f4-120">Request headers</span></span>

| <span data-ttu-id="ea3f4-121">名称</span><span class="sxs-lookup"><span data-stu-id="ea3f4-121">Name</span></span>      |<span data-ttu-id="ea3f4-122">说明</span><span class="sxs-lookup"><span data-stu-id="ea3f4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea3f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea3f4-123">Authorization</span></span> | <span data-ttu-id="ea3f4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea3f4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea3f4-126">Request body</span></span>

<span data-ttu-id="ea3f4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea3f4-128">响应</span><span class="sxs-lookup"><span data-stu-id="ea3f4-128">Response</span></span>

<span data-ttu-id="ea3f4-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-129">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea3f4-130">示例</span><span class="sxs-lookup"><span data-stu-id="ea3f4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea3f4-131">请求</span><span class="sxs-lookup"><span data-stu-id="ea3f4-131">Request</span></span>

<span data-ttu-id="ea3f4-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea3f4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea3f4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="ea3f4-134">C#</span><span class="sxs-lookup"><span data-stu-id="ea3f4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea3f4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea3f4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea3f4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea3f4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea3f4-137">Java</span><span class="sxs-lookup"><span data-stu-id="ea3f4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="ea3f4-138">响应</span><span class="sxs-lookup"><span data-stu-id="ea3f4-138">Response</span></span>

<span data-ttu-id="ea3f4-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-139">The following is an example of the response.</span></span>

> <span data-ttu-id="ea3f4-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ea3f4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
