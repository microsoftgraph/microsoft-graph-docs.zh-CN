---
title: 添加成员
description: 通过**members**导航属性将成员添加到 Office 365 组或安全组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6f6b95abf4e1b218744fddc2cbd167671f3acc8c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420642"
---
# <a name="add-member"></a><span data-ttu-id="c723c-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="c723c-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c723c-104">通过**members**导航属性将成员添加到 Office 365 组或安全组。</span><span class="sxs-lookup"><span data-stu-id="c723c-104">Add a member to an Office 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="c723c-105">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="c723c-105">You can add users or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="c723c-106">只能将用户添加到 Office 365 组中。</span><span class="sxs-lookup"><span data-stu-id="c723c-106">You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c723c-107">权限</span><span class="sxs-lookup"><span data-stu-id="c723c-107">Permissions</span></span>
<span data-ttu-id="c723c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c723c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c723c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c723c-110">Permission type</span></span>      | <span data-ttu-id="c723c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c723c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c723c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c723c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c723c-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c723c-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c723c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c723c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c723c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c723c-115">Not supported.</span></span>    |
|<span data-ttu-id="c723c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c723c-116">Application</span></span> | <span data-ttu-id="c723c-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c723c-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c723c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c723c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c723c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c723c-119">Request headers</span></span>
| <span data-ttu-id="c723c-120">名称</span><span class="sxs-lookup"><span data-stu-id="c723c-120">Name</span></span> | <span data-ttu-id="c723c-121">说明</span><span class="sxs-lookup"><span data-stu-id="c723c-121">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="c723c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c723c-122">Authorization</span></span> | <span data-ttu-id="c723c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c723c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c723c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c723c-125">Request body</span></span>
<span data-ttu-id="c723c-126">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c723c-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c723c-127">响应</span><span class="sxs-lookup"><span data-stu-id="c723c-127">Response</span></span>
<span data-ttu-id="c723c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c723c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c723c-130">示例</span><span class="sxs-lookup"><span data-stu-id="c723c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c723c-131">请求</span><span class="sxs-lookup"><span data-stu-id="c723c-131">Request</span></span>
<span data-ttu-id="c723c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c723c-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c723c-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c723c-133">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c723c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c723c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c723c-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="c723c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="c723c-136">C#</span><span class="sxs-lookup"><span data-stu-id="c723c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c723c-137">在请求正文中, 提供要添加的[directoryObject](../resources/directoryobject.md)、 `id` [USER](../resources/user.md)或[group](../resources/group.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c723c-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="c723c-138">响应</span><span class="sxs-lookup"><span data-stu-id="c723c-138">Response</span></span>
<span data-ttu-id="c723c-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c723c-139">The following is an example of the response.</span></span>
><span data-ttu-id="c723c-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c723c-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c723c-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c723c-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
