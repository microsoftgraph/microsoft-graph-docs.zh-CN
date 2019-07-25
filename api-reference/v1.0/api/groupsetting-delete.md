---
title: 删除组设置
description: 删除组设置。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5cb7a47e7ee376a33f8bb4cbbe2c577b05d3f063
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886788"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="d41b1-103">删除组设置</span><span class="sxs-lookup"><span data-stu-id="d41b1-103">Delete a group setting</span></span>

<span data-ttu-id="d41b1-104">删除组设置。</span><span class="sxs-lookup"><span data-stu-id="d41b1-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="d41b1-105">权限</span><span class="sxs-lookup"><span data-stu-id="d41b1-105">Permissions</span></span>

<span data-ttu-id="d41b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d41b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d41b1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d41b1-108">Permission type</span></span>      | <span data-ttu-id="d41b1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d41b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d41b1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d41b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d41b1-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d41b1-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d41b1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d41b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d41b1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d41b1-113">Not supported.</span></span>    |
|<span data-ttu-id="d41b1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d41b1-114">Application</span></span> | <span data-ttu-id="d41b1-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d41b1-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d41b1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d41b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="d41b1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d41b1-117">Request headers</span></span>

| <span data-ttu-id="d41b1-118">名称</span><span class="sxs-lookup"><span data-stu-id="d41b1-118">Name</span></span> | <span data-ttu-id="d41b1-119">说明</span><span class="sxs-lookup"><span data-stu-id="d41b1-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d41b1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d41b1-120">Authorization</span></span>  | <span data-ttu-id="d41b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d41b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d41b1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d41b1-123">Content-Type</span></span>  | <span data-ttu-id="d41b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d41b1-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d41b1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d41b1-125">Request body</span></span>
<span data-ttu-id="d41b1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d41b1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d41b1-127">响应</span><span class="sxs-lookup"><span data-stu-id="d41b1-127">Response</span></span>

<span data-ttu-id="d41b1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d41b1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d41b1-130">示例</span><span class="sxs-lookup"><span data-stu-id="d41b1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d41b1-131">请求</span><span class="sxs-lookup"><span data-stu-id="d41b1-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d41b1-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d41b1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d41b1-133">C#</span><span class="sxs-lookup"><span data-stu-id="d41b1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d41b1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d41b1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d41b1-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="d41b1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d41b1-136">Java</span><span class="sxs-lookup"><span data-stu-id="d41b1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d41b1-137">响应</span><span class="sxs-lookup"><span data-stu-id="d41b1-137">Response</span></span>
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
