---
title: 删除应用程序
description: 删除应用程序。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 025d9d6b67c545ab49f3b76df6bdd6dd71bcb830
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192523"
---
# <a name="delete-application"></a><span data-ttu-id="cc3c9-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="cc3c9-103">Delete application</span></span>

<span data-ttu-id="cc3c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc3c9-105">删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-105">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc3c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="cc3c9-106">Permissions</span></span>
<span data-ttu-id="cc3c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc3c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc3c9-109">Permission type</span></span>      | <span data-ttu-id="cc3c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc3c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc3c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc3c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc3c9-112">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc3c9-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cc3c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc3c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc3c9-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c9-114">Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc3c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc3c9-115">Application</span></span> | <span data-ttu-id="cc3c9-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c9-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc3c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc3c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cc3c9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc3c9-118">Request headers</span></span>
| <span data-ttu-id="cc3c9-119">名称</span><span class="sxs-lookup"><span data-stu-id="cc3c9-119">Name</span></span>       | <span data-ttu-id="cc3c9-120">说明</span><span class="sxs-lookup"><span data-stu-id="cc3c9-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cc3c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc3c9-121">Authorization</span></span> | <span data-ttu-id="cc3c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc3c9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc3c9-124">Request body</span></span>
<span data-ttu-id="cc3c9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc3c9-126">响应</span><span class="sxs-lookup"><span data-stu-id="cc3c9-126">Response</span></span>

<span data-ttu-id="cc3c9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3c9-129">示例</span><span class="sxs-lookup"><span data-stu-id="cc3c9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc3c9-130">请求</span><span class="sxs-lookup"><span data-stu-id="cc3c9-130">Request</span></span>
<span data-ttu-id="cc3c9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc3c9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc3c9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="cc3c9-133">C#</span><span class="sxs-lookup"><span data-stu-id="cc3c9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc3c9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc3c9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc3c9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc3c9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc3c9-136">响应</span><span class="sxs-lookup"><span data-stu-id="cc3c9-136">Response</span></span>
<span data-ttu-id="cc3c9-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc3c9-137">Here is an example of the response.</span></span> 
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


