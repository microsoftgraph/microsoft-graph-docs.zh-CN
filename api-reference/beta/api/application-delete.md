---
title: 删除应用程序
description: 删除应用程序。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d7b07cf00005f7fed6918983858d9d9b9357f21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996939"
---
# <a name="delete-application"></a><span data-ttu-id="a56af-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="a56af-103">Delete application</span></span>

<span data-ttu-id="a56af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a56af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a56af-105">删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="a56af-105">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="a56af-106">权限</span><span class="sxs-lookup"><span data-stu-id="a56af-106">Permissions</span></span>
<span data-ttu-id="a56af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a56af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a56af-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a56af-109">Permission type</span></span>      | <span data-ttu-id="a56af-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a56af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a56af-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a56af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a56af-112">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="a56af-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a56af-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a56af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a56af-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a56af-114">Not supported.</span></span>    |
|<span data-ttu-id="a56af-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a56af-115">Application</span></span> | <span data-ttu-id="a56af-116">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="a56af-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a56af-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a56af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a56af-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a56af-118">Request headers</span></span>
| <span data-ttu-id="a56af-119">名称</span><span class="sxs-lookup"><span data-stu-id="a56af-119">Name</span></span>       | <span data-ttu-id="a56af-120">说明</span><span class="sxs-lookup"><span data-stu-id="a56af-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="a56af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a56af-121">Authorization</span></span> | <span data-ttu-id="a56af-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a56af-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a56af-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a56af-124">Request body</span></span>
<span data-ttu-id="a56af-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a56af-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a56af-126">响应</span><span class="sxs-lookup"><span data-stu-id="a56af-126">Response</span></span>

<span data-ttu-id="a56af-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a56af-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a56af-129">示例</span><span class="sxs-lookup"><span data-stu-id="a56af-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a56af-130">请求</span><span class="sxs-lookup"><span data-stu-id="a56af-130">Request</span></span>
<span data-ttu-id="a56af-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a56af-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a56af-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a56af-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="a56af-133">C#</span><span class="sxs-lookup"><span data-stu-id="a56af-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a56af-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a56af-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a56af-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a56af-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a56af-136">响应</span><span class="sxs-lookup"><span data-stu-id="a56af-136">Response</span></span>
<span data-ttu-id="a56af-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a56af-137">Here is an example of the response.</span></span> 
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


