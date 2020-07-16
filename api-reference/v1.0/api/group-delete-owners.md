---
title: 删除所有者
description: 使用此 API 可以通过 owners 导航属性从 Microsoft 365 组、安全组或启用邮件的安全组中删除所有者。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 133edd14f1ac71cd2f3f24d3f45c435072be247d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895592"
---
# <a name="remove-owner"></a><span data-ttu-id="f81aa-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="f81aa-103">Remove owner</span></span>

<span data-ttu-id="f81aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f81aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f81aa-105">使用此 API 可以通过 owners 导航属性从 Microsoft 365 组、安全组或启用邮件的安全组中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="f81aa-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f81aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="f81aa-106">Permissions</span></span>
<span data-ttu-id="f81aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f81aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f81aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f81aa-109">Permission type</span></span>      | <span data-ttu-id="f81aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f81aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f81aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f81aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f81aa-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f81aa-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f81aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f81aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f81aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f81aa-114">Not supported.</span></span>    |
|<span data-ttu-id="f81aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f81aa-115">Application</span></span> | <span data-ttu-id="f81aa-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81aa-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f81aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f81aa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f81aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f81aa-118">Request headers</span></span>
| <span data-ttu-id="f81aa-119">名称</span><span class="sxs-lookup"><span data-stu-id="f81aa-119">Name</span></span>       | <span data-ttu-id="f81aa-120">类型</span><span class="sxs-lookup"><span data-stu-id="f81aa-120">Type</span></span> | <span data-ttu-id="f81aa-121">说明</span><span class="sxs-lookup"><span data-stu-id="f81aa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f81aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f81aa-122">Authorization</span></span>  | <span data-ttu-id="f81aa-123">string</span><span class="sxs-lookup"><span data-stu-id="f81aa-123">string</span></span>  | <span data-ttu-id="f81aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f81aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f81aa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f81aa-126">Request body</span></span>
<span data-ttu-id="f81aa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f81aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f81aa-128">响应</span><span class="sxs-lookup"><span data-stu-id="f81aa-128">Response</span></span>
<span data-ttu-id="f81aa-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f81aa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f81aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="f81aa-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f81aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="f81aa-132">Request</span></span>
<span data-ttu-id="f81aa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f81aa-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f81aa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f81aa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f81aa-135">C#</span><span class="sxs-lookup"><span data-stu-id="f81aa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f81aa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f81aa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f81aa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f81aa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f81aa-138">Java</span><span class="sxs-lookup"><span data-stu-id="f81aa-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f81aa-139">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="f81aa-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="f81aa-140">响应</span><span class="sxs-lookup"><span data-stu-id="f81aa-140">Response</span></span>
<span data-ttu-id="f81aa-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f81aa-141">The following is an example of the response.</span></span>
><span data-ttu-id="f81aa-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f81aa-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f81aa-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f81aa-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
