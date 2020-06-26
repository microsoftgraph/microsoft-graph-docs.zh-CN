---
title: 删除所有者
description: 使用此 API 可以通过 owners 导航属性从 Microsoft 365 组、安全组或启用邮件的安全组中删除所有者。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 89e400b56bb4fd3aa318e29d3863c63a3e0af5f6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895858"
---
# <a name="remove-owner"></a><span data-ttu-id="341a3-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="341a3-103">Remove owner</span></span>

<span data-ttu-id="341a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="341a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="341a3-105">使用此 API 可以通过 owners 导航属性从 Microsoft 365 组、安全组或启用邮件的安全组中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="341a3-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="341a3-106">权限</span><span class="sxs-lookup"><span data-stu-id="341a3-106">Permissions</span></span>
<span data-ttu-id="341a3-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="341a3-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="341a3-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="341a3-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="341a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="341a3-109">Permission type</span></span>      | <span data-ttu-id="341a3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="341a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="341a3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="341a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="341a3-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="341a3-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="341a3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="341a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="341a3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="341a3-114">Not supported.</span></span>    |
|<span data-ttu-id="341a3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="341a3-115">Application</span></span> | <span data-ttu-id="341a3-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="341a3-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="341a3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="341a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="341a3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="341a3-118">Request headers</span></span>
| <span data-ttu-id="341a3-119">名称</span><span class="sxs-lookup"><span data-stu-id="341a3-119">Name</span></span>       | <span data-ttu-id="341a3-120">类型</span><span class="sxs-lookup"><span data-stu-id="341a3-120">Type</span></span> | <span data-ttu-id="341a3-121">说明</span><span class="sxs-lookup"><span data-stu-id="341a3-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="341a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="341a3-122">Authorization</span></span>  | <span data-ttu-id="341a3-123">string</span><span class="sxs-lookup"><span data-stu-id="341a3-123">string</span></span>  | <span data-ttu-id="341a3-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="341a3-124">Bearer {token}.</span></span> <span data-ttu-id="341a3-125">Required.</span><span class="sxs-lookup"><span data-stu-id="341a3-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="341a3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="341a3-126">Request body</span></span>
<span data-ttu-id="341a3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="341a3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="341a3-128">响应</span><span class="sxs-lookup"><span data-stu-id="341a3-128">Response</span></span>
<span data-ttu-id="341a3-129">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="341a3-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="341a3-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="341a3-130">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="341a3-131">示例</span><span class="sxs-lookup"><span data-stu-id="341a3-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="341a3-132">请求</span><span class="sxs-lookup"><span data-stu-id="341a3-132">Request</span></span>
<span data-ttu-id="341a3-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="341a3-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="341a3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="341a3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="341a3-135">C#</span><span class="sxs-lookup"><span data-stu-id="341a3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="341a3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="341a3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="341a3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="341a3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="341a3-138">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="341a3-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="341a3-139">响应</span><span class="sxs-lookup"><span data-stu-id="341a3-139">Response</span></span>
<span data-ttu-id="341a3-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="341a3-140">The following is an example of the response.</span></span>
><span data-ttu-id="341a3-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="341a3-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="341a3-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="341a3-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
