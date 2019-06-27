---
title: 添加成员
description: 使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7bb6e5980ca76d96b544fe07880983de6171e014
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262921"
---
# <a name="add-member"></a><span data-ttu-id="0b945-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="0b945-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b945-104">使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。</span><span class="sxs-lookup"><span data-stu-id="0b945-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="0b945-105">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="0b945-105">You can add users or other groups.</span></span> <span data-ttu-id="0b945-106">重要说明：只能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="0b945-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b945-107">权限</span><span class="sxs-lookup"><span data-stu-id="0b945-107">Permissions</span></span>
<span data-ttu-id="0b945-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b945-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b945-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b945-110">Permission type</span></span>      | <span data-ttu-id="0b945-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b945-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b945-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b945-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b945-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b945-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b945-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b945-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b945-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b945-115">Not supported.</span></span>    |
|<span data-ttu-id="0b945-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b945-116">Application</span></span> | <span data-ttu-id="0b945-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b945-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b945-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b945-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0b945-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b945-119">Request headers</span></span>
| <span data-ttu-id="0b945-120">名称</span><span class="sxs-lookup"><span data-stu-id="0b945-120">Name</span></span>       | <span data-ttu-id="0b945-121">类型</span><span class="sxs-lookup"><span data-stu-id="0b945-121">Type</span></span> | <span data-ttu-id="0b945-122">说明</span><span class="sxs-lookup"><span data-stu-id="0b945-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b945-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b945-123">Authorization</span></span>  | <span data-ttu-id="0b945-124">string</span><span class="sxs-lookup"><span data-stu-id="0b945-124">string</span></span>  | <span data-ttu-id="0b945-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b945-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b945-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b945-127">Request body</span></span>
<span data-ttu-id="0b945-128">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b945-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="0b945-129">响应</span><span class="sxs-lookup"><span data-stu-id="0b945-129">Response</span></span>
<span data-ttu-id="0b945-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0b945-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b945-132">示例</span><span class="sxs-lookup"><span data-stu-id="0b945-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0b945-133">请求</span><span class="sxs-lookup"><span data-stu-id="0b945-133">Request</span></span>
<span data-ttu-id="0b945-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b945-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="0b945-135">在请求正文中, 提供要添加的[directoryObject](../resources/directoryobject.md)、 `id` [USER](../resources/user.md)或[group](../resources/group.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b945-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="0b945-136">响应</span><span class="sxs-lookup"><span data-stu-id="0b945-136">Response</span></span>
<span data-ttu-id="0b945-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b945-137">The following is an example of the response.</span></span>
><span data-ttu-id="0b945-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b945-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b945-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0b945-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b945-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0b945-140">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b945-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b945-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/add_group_member-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0b945-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="0b945-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/add_group_member-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
