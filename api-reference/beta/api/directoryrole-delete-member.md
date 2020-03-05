---
title: 删除目录角色成员
description: 从 directoryRole 中删除成员。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f17f3fe1bb79a2d151e23bd4ee8172278e98b64d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434544"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="28ee3-103">删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="28ee3-103">Remove directory role member</span></span>

<span data-ttu-id="28ee3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="28ee3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28ee3-105">从 directoryRole 中删除成员。</span><span class="sxs-lookup"><span data-stu-id="28ee3-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ee3-106">权限</span><span class="sxs-lookup"><span data-stu-id="28ee3-106">Permissions</span></span>

<span data-ttu-id="28ee3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28ee3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="28ee3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="28ee3-109">Permission type</span></span>      | <span data-ttu-id="28ee3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28ee3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28ee3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28ee3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28ee3-112">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="28ee3-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28ee3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28ee3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ee3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="28ee3-114">Not supported.</span></span>    |
|<span data-ttu-id="28ee3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="28ee3-115">Application</span></span> | <span data-ttu-id="28ee3-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="28ee3-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="28ee3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28ee3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="28ee3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="28ee3-118">Request headers</span></span>

| <span data-ttu-id="28ee3-119">名称</span><span class="sxs-lookup"><span data-stu-id="28ee3-119">Name</span></span>       | <span data-ttu-id="28ee3-120">类型</span><span class="sxs-lookup"><span data-stu-id="28ee3-120">Type</span></span> | <span data-ttu-id="28ee3-121">说明</span><span class="sxs-lookup"><span data-stu-id="28ee3-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28ee3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28ee3-122">Authorization</span></span>  | <span data-ttu-id="28ee3-123">string</span><span class="sxs-lookup"><span data-stu-id="28ee3-123">string</span></span>  | <span data-ttu-id="28ee3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28ee3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28ee3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28ee3-126">Request body</span></span>

<span data-ttu-id="28ee3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="28ee3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28ee3-128">响应</span><span class="sxs-lookup"><span data-stu-id="28ee3-128">Response</span></span>

<span data-ttu-id="28ee3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="28ee3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28ee3-131">示例</span><span class="sxs-lookup"><span data-stu-id="28ee3-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="28ee3-132">请求</span><span class="sxs-lookup"><span data-stu-id="28ee3-132">Request</span></span>

<span data-ttu-id="28ee3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28ee3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28ee3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="28ee3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="28ee3-135">C#</span><span class="sxs-lookup"><span data-stu-id="28ee3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28ee3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28ee3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28ee3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28ee3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="28ee3-138">响应</span><span class="sxs-lookup"><span data-stu-id="28ee3-138">Response</span></span>

<span data-ttu-id="28ee3-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="28ee3-139">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
