---
title: 列表已分配 tokenLifetimePolicies
description: 列出分配给应用程序的 tokenLifetimePolicies。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f7b9d70054cc3d0b578917f9b98f8c1083558833
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510538"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="94971-103">列表已分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="94971-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="94971-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94971-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="94971-105">列出分配给[应用程序](../resources/application.md)的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94971-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94971-106">权限</span><span class="sxs-lookup"><span data-stu-id="94971-106">Permissions</span></span>

<span data-ttu-id="94971-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94971-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94971-109">Permission type</span></span>                        | <span data-ttu-id="94971-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94971-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94971-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94971-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94971-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="94971-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="94971-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94971-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94971-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="94971-114">Not supported.</span></span> |
| <span data-ttu-id="94971-115">Application</span><span class="sxs-lookup"><span data-stu-id="94971-115">Application</span></span>                            | <span data-ttu-id="94971-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="94971-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94971-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94971-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="94971-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="94971-118">Request headers</span></span>

| <span data-ttu-id="94971-119">名称</span><span class="sxs-lookup"><span data-stu-id="94971-119">Name</span></span>          | <span data-ttu-id="94971-120">说明</span><span class="sxs-lookup"><span data-stu-id="94971-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="94971-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94971-121">Authorization</span></span> | <span data-ttu-id="94971-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94971-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94971-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="94971-124">Request body</span></span>

<span data-ttu-id="94971-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94971-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94971-126">响应</span><span class="sxs-lookup"><span data-stu-id="94971-126">Response</span></span>

<span data-ttu-id="94971-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="94971-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94971-128">示例</span><span class="sxs-lookup"><span data-stu-id="94971-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94971-129">请求</span><span class="sxs-lookup"><span data-stu-id="94971-129">Request</span></span>

<span data-ttu-id="94971-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94971-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94971-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="94971-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="94971-132">C#</span><span class="sxs-lookup"><span data-stu-id="94971-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94971-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94971-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94971-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94971-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94971-135">Java</span><span class="sxs-lookup"><span data-stu-id="94971-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94971-136">响应</span><span class="sxs-lookup"><span data-stu-id="94971-136">Response</span></span>

<span data-ttu-id="94971-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94971-137">The following is an example of the response.</span></span>

> <span data-ttu-id="94971-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94971-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
