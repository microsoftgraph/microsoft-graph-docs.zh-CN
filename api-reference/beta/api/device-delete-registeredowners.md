---
title: 删除 registeredowners
description: 删除用户作为设备的注册所有者。
localization_priority: Normal
author: michaelrm97
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 094c7aa46102d10cd61267b0056654d3e463a335
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437232"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="383ec-103">删除 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="383ec-103">Delete registeredOwner</span></span>

<span data-ttu-id="383ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="383ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="383ec-105">删除用户作为设备的注册所有者。</span><span class="sxs-lookup"><span data-stu-id="383ec-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="383ec-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="383ec-106">Permissions</span></span>

<span data-ttu-id="383ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="383ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="383ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="383ec-109">Permission type</span></span>      | <span data-ttu-id="383ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="383ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="383ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="383ec-111">Delegated (work or school account)</span></span> |<span data-ttu-id="383ec-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="383ec-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="383ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="383ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="383ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="383ec-114">Not supported.</span></span>    |
|<span data-ttu-id="383ec-115">Application</span><span class="sxs-lookup"><span data-stu-id="383ec-115">Application</span></span> | <span data-ttu-id="383ec-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="383ec-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="383ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="383ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="383ec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="383ec-118">Request headers</span></span>
| <span data-ttu-id="383ec-119">名称</span><span class="sxs-lookup"><span data-stu-id="383ec-119">Name</span></span>       | <span data-ttu-id="383ec-120">类型</span><span class="sxs-lookup"><span data-stu-id="383ec-120">Type</span></span> | <span data-ttu-id="383ec-121">说明</span><span class="sxs-lookup"><span data-stu-id="383ec-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="383ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="383ec-122">Authorization</span></span>  | <span data-ttu-id="383ec-123">string</span><span class="sxs-lookup"><span data-stu-id="383ec-123">string</span></span>  | <span data-ttu-id="383ec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="383ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="383ec-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="383ec-126">Request body</span></span>
<span data-ttu-id="383ec-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="383ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="383ec-128">响应</span><span class="sxs-lookup"><span data-stu-id="383ec-128">Response</span></span>

<span data-ttu-id="383ec-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="383ec-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="383ec-130">示例</span><span class="sxs-lookup"><span data-stu-id="383ec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="383ec-131">请求</span><span class="sxs-lookup"><span data-stu-id="383ec-131">Request</span></span>
<span data-ttu-id="383ec-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="383ec-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="383ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="383ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredOwners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="383ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="383ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="383ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="383ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="383ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="383ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="383ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="383ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="383ec-138">响应</span><span class="sxs-lookup"><span data-stu-id="383ec-138">Response</span></span>
<span data-ttu-id="383ec-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="383ec-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


