---
title: 添加成员
description: 使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 2457c12654da11cf54fb503bdf752f4fe60dc021
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613986"
---
# <a name="add-member"></a><span data-ttu-id="e0136-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="e0136-103">Add member</span></span>
<span data-ttu-id="e0136-104">使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。</span><span class="sxs-lookup"><span data-stu-id="e0136-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="e0136-105">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="e0136-105">You can add users or other groups.</span></span> <span data-ttu-id="e0136-106">重要说明：只能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="e0136-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0136-107">权限</span><span class="sxs-lookup"><span data-stu-id="e0136-107">Permissions</span></span>
<span data-ttu-id="e0136-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0136-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0136-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0136-110">Permission type</span></span>      | <span data-ttu-id="e0136-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0136-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0136-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0136-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0136-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0136-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0136-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0136-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0136-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0136-115">Not supported.</span></span>    |
|<span data-ttu-id="e0136-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0136-116">Application</span></span> | <span data-ttu-id="e0136-117">Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0136-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0136-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0136-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e0136-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0136-119">Request headers</span></span>
| <span data-ttu-id="e0136-120">名称</span><span class="sxs-lookup"><span data-stu-id="e0136-120">Name</span></span>       | <span data-ttu-id="e0136-121">类型</span><span class="sxs-lookup"><span data-stu-id="e0136-121">Type</span></span> | <span data-ttu-id="e0136-122">说明</span><span class="sxs-lookup"><span data-stu-id="e0136-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0136-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0136-123">Authorization</span></span>  | <span data-ttu-id="e0136-124">string</span><span class="sxs-lookup"><span data-stu-id="e0136-124">string</span></span>  | <span data-ttu-id="e0136-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0136-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0136-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0136-127">Request body</span></span>
<span data-ttu-id="e0136-128">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0136-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e0136-129">响应</span><span class="sxs-lookup"><span data-stu-id="e0136-129">Response</span></span>
<span data-ttu-id="e0136-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0136-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0136-132">示例</span><span class="sxs-lookup"><span data-stu-id="e0136-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e0136-133">请求</span><span class="sxs-lookup"><span data-stu-id="e0136-133">Request</span></span>
<span data-ttu-id="e0136-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0136-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="e0136-135">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 `id` 的JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0136-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="e0136-136">响应</span><span class="sxs-lookup"><span data-stu-id="e0136-136">Response</span></span>
<span data-ttu-id="e0136-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0136-137">The following is an example of the response.</span></span>
><span data-ttu-id="e0136-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0136-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e0136-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0136-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0136-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e0136-140">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0136-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0136-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
