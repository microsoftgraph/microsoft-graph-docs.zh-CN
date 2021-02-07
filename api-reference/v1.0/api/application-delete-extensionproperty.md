---
title: 删除 extensionProperty
description: 删除 extensionProperty。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 38e5358a39214c060a56513ff31120c3ea12ead8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131822"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="4c1a0-103">删除 extensionProperty</span><span class="sxs-lookup"><span data-stu-id="4c1a0-103">Delete extensionProperty</span></span>

<span data-ttu-id="4c1a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c1a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c1a0-105">删除 [extensionProperty](../resources/extensionproperty.md)。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c1a0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4c1a0-106">Permissions</span></span>

<span data-ttu-id="4c1a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c1a0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c1a0-109">Permission type</span></span>      | <span data-ttu-id="4c1a0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c1a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c1a0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c1a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4c1a0-112">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c1a0-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c1a0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c1a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c1a0-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1a0-114">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="4c1a0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c1a0-115">Application</span></span> | <span data-ttu-id="4c1a0-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c1a0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c1a0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c1a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c1a0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c1a0-118">Request headers</span></span>

| <span data-ttu-id="4c1a0-119">名称</span><span class="sxs-lookup"><span data-stu-id="4c1a0-119">Name</span></span>       | <span data-ttu-id="4c1a0-120">说明</span><span class="sxs-lookup"><span data-stu-id="4c1a0-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4c1a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c1a0-121">Authorization</span></span>  | <span data-ttu-id="4c1a0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c1a0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c1a0-124">Request body</span></span>

<span data-ttu-id="4c1a0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c1a0-126">响应</span><span class="sxs-lookup"><span data-stu-id="4c1a0-126">Response</span></span>

<span data-ttu-id="4c1a0-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c1a0-129">示例</span><span class="sxs-lookup"><span data-stu-id="4c1a0-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c1a0-130">请求</span><span class="sxs-lookup"><span data-stu-id="4c1a0-130">Request</span></span>

<span data-ttu-id="4c1a0-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c1a0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c1a0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="4c1a0-133">C#</span><span class="sxs-lookup"><span data-stu-id="4c1a0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c1a0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c1a0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c1a0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c1a0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c1a0-136">Java</span><span class="sxs-lookup"><span data-stu-id="4c1a0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c1a0-137">响应</span><span class="sxs-lookup"><span data-stu-id="4c1a0-137">Response</span></span>

<span data-ttu-id="4c1a0-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4c1a0-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

