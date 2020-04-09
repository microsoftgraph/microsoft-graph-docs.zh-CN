---
title: 删除 directoryObject
description: 删除 directoryObject。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02311d5908237325e627e61706d25ee1b3d16c2f
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181942"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="16cec-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="16cec-103">Delete directoryObject</span></span>

<span data-ttu-id="16cec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16cec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16cec-105">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="16cec-105">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="16cec-106">权限</span><span class="sxs-lookup"><span data-stu-id="16cec-106">Permissions</span></span>
<span data-ttu-id="16cec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16cec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="16cec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16cec-109">Permission type</span></span>      | <span data-ttu-id="16cec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16cec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16cec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16cec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16cec-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16cec-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16cec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16cec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16cec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16cec-114">Not supported.</span></span>    |
|<span data-ttu-id="16cec-115">Application</span><span class="sxs-lookup"><span data-stu-id="16cec-115">Application</span></span> | <span data-ttu-id="16cec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16cec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16cec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16cec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="16cec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="16cec-118">Request headers</span></span>
| <span data-ttu-id="16cec-119">名称</span><span class="sxs-lookup"><span data-stu-id="16cec-119">Name</span></span>       | <span data-ttu-id="16cec-120">类型</span><span class="sxs-lookup"><span data-stu-id="16cec-120">Type</span></span> | <span data-ttu-id="16cec-121">说明</span><span class="sxs-lookup"><span data-stu-id="16cec-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16cec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16cec-122">Authorization</span></span>  | <span data-ttu-id="16cec-123">string</span><span class="sxs-lookup"><span data-stu-id="16cec-123">string</span></span>  | <span data-ttu-id="16cec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16cec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16cec-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16cec-126">Request body</span></span>
<span data-ttu-id="16cec-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16cec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16cec-128">响应</span><span class="sxs-lookup"><span data-stu-id="16cec-128">Response</span></span>

<span data-ttu-id="16cec-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="16cec-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16cec-131">示例</span><span class="sxs-lookup"><span data-stu-id="16cec-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16cec-132">请求</span><span class="sxs-lookup"><span data-stu-id="16cec-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16cec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="16cec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="16cec-134">C#</span><span class="sxs-lookup"><span data-stu-id="16cec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16cec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16cec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16cec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16cec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16cec-137">Java</span><span class="sxs-lookup"><span data-stu-id="16cec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16cec-138">响应</span><span class="sxs-lookup"><span data-stu-id="16cec-138">Response</span></span>

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
