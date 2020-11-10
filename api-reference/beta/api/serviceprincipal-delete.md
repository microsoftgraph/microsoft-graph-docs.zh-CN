---
title: 删除 servicePrincipal
description: 删除 servicePrincipal。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 96464d54e6dee547b6c67903d5f833c874868919
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969638"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="90748-103">删除 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="90748-103">Delete servicePrincipal</span></span>

<span data-ttu-id="90748-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90748-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90748-105">删除 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90748-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90748-106">权限</span><span class="sxs-lookup"><span data-stu-id="90748-106">Permissions</span></span>
<span data-ttu-id="90748-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90748-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90748-109">Permission type</span></span>      | <span data-ttu-id="90748-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90748-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90748-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90748-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90748-112">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90748-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="90748-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90748-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90748-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90748-114">Not supported.</span></span>    |
|<span data-ttu-id="90748-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90748-115">Application</span></span> | <span data-ttu-id="90748-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90748-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90748-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90748-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="90748-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="90748-118">Request headers</span></span>
| <span data-ttu-id="90748-119">名称</span><span class="sxs-lookup"><span data-stu-id="90748-119">Name</span></span>       | <span data-ttu-id="90748-120">类型</span><span class="sxs-lookup"><span data-stu-id="90748-120">Type</span></span> | <span data-ttu-id="90748-121">说明</span><span class="sxs-lookup"><span data-stu-id="90748-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="90748-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90748-122">Authorization</span></span>  | <span data-ttu-id="90748-123">string</span><span class="sxs-lookup"><span data-stu-id="90748-123">string</span></span>  | <span data-ttu-id="90748-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90748-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90748-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90748-126">Request body</span></span>
<span data-ttu-id="90748-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90748-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90748-128">响应</span><span class="sxs-lookup"><span data-stu-id="90748-128">Response</span></span>

<span data-ttu-id="90748-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="90748-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90748-131">示例</span><span class="sxs-lookup"><span data-stu-id="90748-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="90748-132">请求</span><span class="sxs-lookup"><span data-stu-id="90748-132">Request</span></span>
<span data-ttu-id="90748-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90748-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="90748-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="90748-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="90748-135">C#</span><span class="sxs-lookup"><span data-stu-id="90748-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90748-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90748-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90748-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90748-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90748-138">Java</span><span class="sxs-lookup"><span data-stu-id="90748-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="90748-139">响应</span><span class="sxs-lookup"><span data-stu-id="90748-139">Response</span></span>
<span data-ttu-id="90748-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="90748-140">Here is an example of the response.</span></span> 
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


