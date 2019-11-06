---
title: 删除 extensionProperty
description: 删除 extensionProperty。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d9685a285ef82241ace355dd43d0b694b3816901
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999341"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="0c5cb-103">删除 extensionProperty</span><span class="sxs-lookup"><span data-stu-id="0c5cb-103">Delete extensionProperty</span></span>

<span data-ttu-id="0c5cb-104">删除[extensionProperty](../resources/extensionproperty.md)。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-104">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c5cb-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="0c5cb-105">Permissions</span></span>

<span data-ttu-id="0c5cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c5cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c5cb-108">Permission type</span></span>      | <span data-ttu-id="0c5cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c5cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c5cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c5cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c5cb-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c5cb-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c5cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c5cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c5cb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-113">Not supported.</span></span>    |
|<span data-ttu-id="0c5cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c5cb-114">Application</span></span> | <span data-ttu-id="0c5cb-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c5cb-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c5cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c5cb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0c5cb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c5cb-117">Request headers</span></span>

| <span data-ttu-id="0c5cb-118">名称</span><span class="sxs-lookup"><span data-stu-id="0c5cb-118">Name</span></span>       | <span data-ttu-id="0c5cb-119">说明</span><span class="sxs-lookup"><span data-stu-id="0c5cb-119">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0c5cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c5cb-120">Authorization</span></span>  | <span data-ttu-id="0c5cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c5cb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c5cb-123">Request body</span></span>

<span data-ttu-id="0c5cb-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c5cb-125">响应</span><span class="sxs-lookup"><span data-stu-id="0c5cb-125">Response</span></span>

<span data-ttu-id="0c5cb-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c5cb-128">示例</span><span class="sxs-lookup"><span data-stu-id="0c5cb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c5cb-129">请求</span><span class="sxs-lookup"><span data-stu-id="0c5cb-129">Request</span></span>

<span data-ttu-id="0c5cb-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c5cb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c5cb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c5cb-132">C#</span><span class="sxs-lookup"><span data-stu-id="0c5cb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c5cb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c5cb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c5cb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c5cb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c5cb-135">Java</span><span class="sxs-lookup"><span data-stu-id="0c5cb-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c5cb-136">响应</span><span class="sxs-lookup"><span data-stu-id="0c5cb-136">Response</span></span>

<span data-ttu-id="0c5cb-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0c5cb-137">The following is an example of the response.</span></span>

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
