---
title: 列出 certificateBasedAuthConfigurations
description: 获取 certificatebasedauthconfiguration 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3a4fb6035ffb145f7aaaa3378f7212a9759a92af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440519"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="4df0c-103">列出 certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="4df0c-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="4df0c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4df0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4df0c-105">获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4df0c-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="4df0c-106">集合中只能存在一个 certificateBasedAuthConfiguration 实例。</span><span class="sxs-lookup"><span data-stu-id="4df0c-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="4df0c-107">它始终具有值为 "29728ade-6ae4-4ee9-9103-412912537da5" 的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="4df0c-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="4df0c-108">权限</span><span class="sxs-lookup"><span data-stu-id="4df0c-108">Permissions</span></span>

<span data-ttu-id="4df0c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4df0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4df0c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4df0c-111">Permission type</span></span>                        | <span data-ttu-id="4df0c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4df0c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4df0c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4df0c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4df0c-114">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="4df0c-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="4df0c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4df0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4df0c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4df0c-116">Not supported.</span></span> |
| <span data-ttu-id="4df0c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4df0c-117">Application</span></span>    | <span data-ttu-id="4df0c-118">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="4df0c-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4df0c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4df0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="4df0c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4df0c-120">Request headers</span></span>

| <span data-ttu-id="4df0c-121">名称</span><span class="sxs-lookup"><span data-stu-id="4df0c-121">Name</span></span>      |<span data-ttu-id="4df0c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4df0c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4df0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4df0c-123">Authorization</span></span> | <span data-ttu-id="4df0c-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4df0c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4df0c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4df0c-125">Request body</span></span>

<span data-ttu-id="4df0c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4df0c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4df0c-127">响应</span><span class="sxs-lookup"><span data-stu-id="4df0c-127">Response</span></span>

<span data-ttu-id="4df0c-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4df0c-128">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4df0c-129">示例</span><span class="sxs-lookup"><span data-stu-id="4df0c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4df0c-130">请求</span><span class="sxs-lookup"><span data-stu-id="4df0c-130">Request</span></span>

<span data-ttu-id="4df0c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4df0c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4df0c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4df0c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="4df0c-133">C#</span><span class="sxs-lookup"><span data-stu-id="4df0c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4df0c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4df0c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4df0c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4df0c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4df0c-136">响应</span><span class="sxs-lookup"><span data-stu-id="4df0c-136">Response</span></span>

<span data-ttu-id="4df0c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4df0c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="4df0c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4df0c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
