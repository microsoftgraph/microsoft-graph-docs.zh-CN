---
title: 删除所有者
description: 使用此 API 可以通过 owners 导航属性Microsoft 365组、安全组或启用邮件的安全组中删除所有者。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2887284cbd5bdf644c161d790f1cd832a410dae4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053095"
---
# <a name="remove-owner"></a><span data-ttu-id="9b274-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="9b274-103">Remove owner</span></span>

<span data-ttu-id="9b274-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b274-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b274-105">使用此 API 可以通过 owners 导航属性Microsoft 365组、安全组或启用邮件的安全组中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="9b274-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span> <span data-ttu-id="9b274-106">将所有者分配给组后，无法删除组的最后一个所有者。</span><span class="sxs-lookup"><span data-stu-id="9b274-106">Once owners are assigned to a group, the last owner of the group cannot be removed.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9b274-107">权限</span><span class="sxs-lookup"><span data-stu-id="9b274-107">Permissions</span></span>
<span data-ttu-id="9b274-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b274-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b274-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b274-110">Permission type</span></span>      | <span data-ttu-id="9b274-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b274-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b274-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b274-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9b274-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b274-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9b274-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b274-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b274-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b274-115">Not supported.</span></span>    |
|<span data-ttu-id="9b274-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b274-116">Application</span></span> | <span data-ttu-id="9b274-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b274-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b274-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b274-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9b274-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b274-119">Request headers</span></span>
| <span data-ttu-id="9b274-120">名称</span><span class="sxs-lookup"><span data-stu-id="9b274-120">Name</span></span>       | <span data-ttu-id="9b274-121">类型</span><span class="sxs-lookup"><span data-stu-id="9b274-121">Type</span></span> | <span data-ttu-id="9b274-122">说明</span><span class="sxs-lookup"><span data-stu-id="9b274-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b274-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b274-123">Authorization</span></span>  | <span data-ttu-id="9b274-124">string</span><span class="sxs-lookup"><span data-stu-id="9b274-124">string</span></span>  | <span data-ttu-id="9b274-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b274-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b274-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b274-127">Request body</span></span>
<span data-ttu-id="9b274-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b274-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b274-129">响应</span><span class="sxs-lookup"><span data-stu-id="9b274-129">Response</span></span>
<span data-ttu-id="9b274-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9b274-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b274-132">示例</span><span class="sxs-lookup"><span data-stu-id="9b274-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9b274-133">请求</span><span class="sxs-lookup"><span data-stu-id="9b274-133">Request</span></span>
<span data-ttu-id="9b274-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b274-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b274-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b274-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="9b274-136">C#</span><span class="sxs-lookup"><span data-stu-id="9b274-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b274-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b274-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b274-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b274-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b274-139">Java</span><span class="sxs-lookup"><span data-stu-id="9b274-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9b274-140">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="9b274-140">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="9b274-141">响应</span><span class="sxs-lookup"><span data-stu-id="9b274-141">Response</span></span>
<span data-ttu-id="9b274-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b274-142">The following is an example of the response.</span></span>
><span data-ttu-id="9b274-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9b274-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

