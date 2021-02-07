---
title: 删除应用程序
description: 删除应用程序对象。
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: da60fd5c6a3a97a3924fc45448c00f9665748752
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131780"
---
# <a name="delete-application"></a><span data-ttu-id="7fb57-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="7fb57-103">Delete application</span></span>

<span data-ttu-id="7fb57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb57-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fb57-105">删除 [应用程序](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fb57-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fb57-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7fb57-106">Permissions</span></span>
<span data-ttu-id="7fb57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fb57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb57-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fb57-109">Permission type</span></span>      | <span data-ttu-id="7fb57-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fb57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fb57-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fb57-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7fb57-112">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7fb57-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7fb57-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fb57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fb57-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb57-114">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="7fb57-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fb57-115">Application</span></span> | <span data-ttu-id="7fb57-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fb57-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fb57-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fb57-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7fb57-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fb57-118">Request headers</span></span>
| <span data-ttu-id="7fb57-119">名称</span><span class="sxs-lookup"><span data-stu-id="7fb57-119">Name</span></span>       | <span data-ttu-id="7fb57-120">说明</span><span class="sxs-lookup"><span data-stu-id="7fb57-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7fb57-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fb57-121">Authorization</span></span> | <span data-ttu-id="7fb57-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fb57-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fb57-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fb57-124">Request body</span></span>
<span data-ttu-id="7fb57-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7fb57-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb57-126">响应</span><span class="sxs-lookup"><span data-stu-id="7fb57-126">Response</span></span>

<span data-ttu-id="7fb57-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7fb57-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb57-129">示例</span><span class="sxs-lookup"><span data-stu-id="7fb57-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fb57-130">请求</span><span class="sxs-lookup"><span data-stu-id="7fb57-130">Request</span></span>
<span data-ttu-id="7fb57-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7fb57-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7fb57-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb57-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="7fb57-133">C#</span><span class="sxs-lookup"><span data-stu-id="7fb57-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fb57-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fb57-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fb57-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fb57-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fb57-136">Java</span><span class="sxs-lookup"><span data-stu-id="7fb57-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7fb57-137">响应</span><span class="sxs-lookup"><span data-stu-id="7fb57-137">Response</span></span>
<span data-ttu-id="7fb57-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7fb57-138">Here is an example of the response.</span></span> 
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

