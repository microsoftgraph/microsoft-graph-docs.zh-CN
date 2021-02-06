---
title: 删除应用程序
description: 删除应用程序。
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5a2eb41fe80a2e84f2fbe60ad3876f9840a8beed
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129231"
---
# <a name="delete-application"></a><span data-ttu-id="6030f-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="6030f-103">Delete application</span></span>

<span data-ttu-id="6030f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6030f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6030f-105">删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="6030f-105">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6030f-106">权限</span><span class="sxs-lookup"><span data-stu-id="6030f-106">Permissions</span></span>
<span data-ttu-id="6030f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6030f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6030f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6030f-109">Permission type</span></span>      | <span data-ttu-id="6030f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6030f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6030f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6030f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6030f-112">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6030f-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6030f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6030f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6030f-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6030f-114">Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="6030f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6030f-115">Application</span></span> | <span data-ttu-id="6030f-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6030f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6030f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6030f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6030f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6030f-118">Request headers</span></span>
| <span data-ttu-id="6030f-119">名称</span><span class="sxs-lookup"><span data-stu-id="6030f-119">Name</span></span>       | <span data-ttu-id="6030f-120">说明</span><span class="sxs-lookup"><span data-stu-id="6030f-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="6030f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6030f-121">Authorization</span></span> | <span data-ttu-id="6030f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6030f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6030f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6030f-124">Request body</span></span>
<span data-ttu-id="6030f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6030f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6030f-126">响应</span><span class="sxs-lookup"><span data-stu-id="6030f-126">Response</span></span>

<span data-ttu-id="6030f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6030f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6030f-129">示例</span><span class="sxs-lookup"><span data-stu-id="6030f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6030f-130">请求</span><span class="sxs-lookup"><span data-stu-id="6030f-130">Request</span></span>
<span data-ttu-id="6030f-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6030f-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6030f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6030f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="6030f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6030f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6030f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6030f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6030f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6030f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6030f-136">Java</span><span class="sxs-lookup"><span data-stu-id="6030f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6030f-137">响应</span><span class="sxs-lookup"><span data-stu-id="6030f-137">Response</span></span>
<span data-ttu-id="6030f-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6030f-138">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



