---
title: 删除 servicePrincipal
description: 删除 servicePrincipal。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 54e4fbb4c3a764d4b1933439783e59ab79bda23a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058661"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="e0353-103">删除 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e0353-103">Delete servicePrincipal</span></span>

<span data-ttu-id="e0353-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0353-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0353-105">删除 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0353-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0353-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0353-106">Permissions</span></span>
<span data-ttu-id="e0353-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0353-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0353-109">Permission type</span></span>      | <span data-ttu-id="e0353-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0353-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0353-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0353-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0353-112">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="e0353-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e0353-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0353-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0353-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0353-114">Not supported.</span></span>    |
|<span data-ttu-id="e0353-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0353-115">Application</span></span> | <span data-ttu-id="e0353-116">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="e0353-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0353-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0353-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e0353-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0353-118">Request headers</span></span>
| <span data-ttu-id="e0353-119">名称</span><span class="sxs-lookup"><span data-stu-id="e0353-119">Name</span></span>       | <span data-ttu-id="e0353-120">类型</span><span class="sxs-lookup"><span data-stu-id="e0353-120">Type</span></span> | <span data-ttu-id="e0353-121">说明</span><span class="sxs-lookup"><span data-stu-id="e0353-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0353-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0353-122">Authorization</span></span>  | <span data-ttu-id="e0353-123">string</span><span class="sxs-lookup"><span data-stu-id="e0353-123">string</span></span>  | <span data-ttu-id="e0353-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0353-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0353-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0353-126">Request body</span></span>
<span data-ttu-id="e0353-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0353-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0353-128">响应</span><span class="sxs-lookup"><span data-stu-id="e0353-128">Response</span></span>

<span data-ttu-id="e0353-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0353-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0353-131">示例</span><span class="sxs-lookup"><span data-stu-id="e0353-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="e0353-132">请求</span><span class="sxs-lookup"><span data-stu-id="e0353-132">Request</span></span>
<span data-ttu-id="e0353-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0353-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e0353-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0353-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="e0353-135">C#</span><span class="sxs-lookup"><span data-stu-id="e0353-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0353-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0353-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0353-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0353-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e0353-138">响应</span><span class="sxs-lookup"><span data-stu-id="e0353-138">Response</span></span>
<span data-ttu-id="e0353-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0353-139">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


