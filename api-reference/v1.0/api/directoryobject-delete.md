---
title: 删除 directoryObject
description: 删除 directoryObject。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 301fde9286db458b18d952c99239ed3cffd40646
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316148"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="5a7fc-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="5a7fc-103">Delete directoryObject</span></span>

<span data-ttu-id="5a7fc-104">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a7fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="5a7fc-105">Permissions</span></span>
<span data-ttu-id="5a7fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5a7fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a7fc-108">Permission type</span></span>      | <span data-ttu-id="5a7fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a7fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a7fc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a7fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a7fc-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a7fc-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a7fc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a7fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a7fc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-113">Not supported.</span></span>    |
|<span data-ttu-id="5a7fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a7fc-114">Application</span></span> | <span data-ttu-id="5a7fc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a7fc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a7fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5a7fc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a7fc-117">Request headers</span></span>
| <span data-ttu-id="5a7fc-118">名称</span><span class="sxs-lookup"><span data-stu-id="5a7fc-118">Name</span></span>       | <span data-ttu-id="5a7fc-119">类型</span><span class="sxs-lookup"><span data-stu-id="5a7fc-119">Type</span></span> | <span data-ttu-id="5a7fc-120">说明</span><span class="sxs-lookup"><span data-stu-id="5a7fc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a7fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a7fc-121">Authorization</span></span>  | <span data-ttu-id="5a7fc-122">string</span><span class="sxs-lookup"><span data-stu-id="5a7fc-122">string</span></span>  | <span data-ttu-id="5a7fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a7fc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a7fc-125">Request body</span></span>
<span data-ttu-id="5a7fc-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a7fc-127">响应</span><span class="sxs-lookup"><span data-stu-id="5a7fc-127">Response</span></span>

<span data-ttu-id="5a7fc-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5a7fc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a7fc-130">示例</span><span class="sxs-lookup"><span data-stu-id="5a7fc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a7fc-131">请求</span><span class="sxs-lookup"><span data-stu-id="5a7fc-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5a7fc-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5a7fc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a7fc-133">C#</span><span class="sxs-lookup"><span data-stu-id="5a7fc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a7fc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a7fc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a7fc-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="5a7fc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5a7fc-136">Java</span><span class="sxs-lookup"><span data-stu-id="5a7fc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5a7fc-137">响应</span><span class="sxs-lookup"><span data-stu-id="5a7fc-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
