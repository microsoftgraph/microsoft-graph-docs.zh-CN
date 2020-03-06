---
title: 删除组设置
description: 删除组设置。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 20a6bded37bb2b881b0f9f85d313d0c25fd20560
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516841"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="532d4-103">删除组设置</span><span class="sxs-lookup"><span data-stu-id="532d4-103">Delete a group setting</span></span>

<span data-ttu-id="532d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="532d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="532d4-105">删除组设置。</span><span class="sxs-lookup"><span data-stu-id="532d4-105">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="532d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="532d4-106">Permissions</span></span>

<span data-ttu-id="532d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="532d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="532d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="532d4-109">Permission type</span></span>      | <span data-ttu-id="532d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="532d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="532d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="532d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="532d4-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="532d4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="532d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="532d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="532d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="532d4-114">Not supported.</span></span>    |
|<span data-ttu-id="532d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="532d4-115">Application</span></span> | <span data-ttu-id="532d4-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="532d4-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="532d4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="532d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="532d4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="532d4-118">Request headers</span></span>

| <span data-ttu-id="532d4-119">名称</span><span class="sxs-lookup"><span data-stu-id="532d4-119">Name</span></span> | <span data-ttu-id="532d4-120">说明</span><span class="sxs-lookup"><span data-stu-id="532d4-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="532d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="532d4-121">Authorization</span></span>  | <span data-ttu-id="532d4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="532d4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="532d4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="532d4-124">Content-Type</span></span>  | <span data-ttu-id="532d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="532d4-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="532d4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="532d4-126">Request body</span></span>
<span data-ttu-id="532d4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="532d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="532d4-128">响应</span><span class="sxs-lookup"><span data-stu-id="532d4-128">Response</span></span>

<span data-ttu-id="532d4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="532d4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="532d4-131">示例</span><span class="sxs-lookup"><span data-stu-id="532d4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="532d4-132">请求</span><span class="sxs-lookup"><span data-stu-id="532d4-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="532d4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="532d4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="532d4-134">C#</span><span class="sxs-lookup"><span data-stu-id="532d4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="532d4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="532d4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="532d4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="532d4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="532d4-137">Java</span><span class="sxs-lookup"><span data-stu-id="532d4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="532d4-138">响应</span><span class="sxs-lookup"><span data-stu-id="532d4-138">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
