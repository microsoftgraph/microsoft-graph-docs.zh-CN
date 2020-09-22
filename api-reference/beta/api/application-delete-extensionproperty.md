---
title: 删除 extensionProperty
description: 删除 extensionProperty。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a3365834c6f637724d470bcd058aac79748e655
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996981"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="84521-103">删除 extensionProperty</span><span class="sxs-lookup"><span data-stu-id="84521-103">Delete extensionProperty</span></span>

<span data-ttu-id="84521-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84521-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84521-105">删除 [extensionProperty](../resources/extensionproperty.md)。</span><span class="sxs-lookup"><span data-stu-id="84521-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="84521-106">权限</span><span class="sxs-lookup"><span data-stu-id="84521-106">Permissions</span></span>

<span data-ttu-id="84521-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84521-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84521-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="84521-109">Permission type</span></span>      | <span data-ttu-id="84521-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84521-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84521-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84521-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84521-112">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="84521-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="84521-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84521-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84521-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="84521-114">Not supported.</span></span>    |
|<span data-ttu-id="84521-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="84521-115">Application</span></span> | <span data-ttu-id="84521-116">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="84521-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84521-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84521-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84521-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="84521-118">Request headers</span></span>

| <span data-ttu-id="84521-119">名称</span><span class="sxs-lookup"><span data-stu-id="84521-119">Name</span></span>       | <span data-ttu-id="84521-120">说明</span><span class="sxs-lookup"><span data-stu-id="84521-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="84521-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84521-121">Authorization</span></span>  | <span data-ttu-id="84521-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84521-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84521-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="84521-124">Request body</span></span>

<span data-ttu-id="84521-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84521-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84521-126">响应</span><span class="sxs-lookup"><span data-stu-id="84521-126">Response</span></span>

<span data-ttu-id="84521-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="84521-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84521-129">示例</span><span class="sxs-lookup"><span data-stu-id="84521-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84521-130">请求</span><span class="sxs-lookup"><span data-stu-id="84521-130">Request</span></span>

<span data-ttu-id="84521-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84521-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84521-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="84521-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="84521-133">C#</span><span class="sxs-lookup"><span data-stu-id="84521-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84521-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84521-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84521-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84521-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84521-136">响应</span><span class="sxs-lookup"><span data-stu-id="84521-136">Response</span></span>

<span data-ttu-id="84521-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84521-137">The following is an example of the response.</span></span>

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


