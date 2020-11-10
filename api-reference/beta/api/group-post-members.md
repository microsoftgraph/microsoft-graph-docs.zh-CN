---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Microsoft 365 组或安全组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1e7e214c23aab13c45abf73e1242aa64ec71bfa3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964991"
---
# <a name="add-member"></a><span data-ttu-id="32716-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="32716-103">Add member</span></span>

<span data-ttu-id="32716-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32716-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32716-105">通过 **members** 导航属性将成员添加到 Microsoft 365 组或安全组。</span><span class="sxs-lookup"><span data-stu-id="32716-105">Add a member to a Microsoft 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="32716-106">您可以添加用户、服务主体或其他组。</span><span class="sxs-lookup"><span data-stu-id="32716-106">You can add users, service principals or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="32716-107">只能向通过云管理的安全组和 Microsoft 365 组添加用户。</span><span class="sxs-lookup"><span data-stu-id="32716-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="32716-108">权限</span><span class="sxs-lookup"><span data-stu-id="32716-108">Permissions</span></span>
<span data-ttu-id="32716-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32716-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="32716-111">Permission type</span></span>      | <span data-ttu-id="32716-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32716-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32716-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32716-113">Delegated (work or school account)</span></span> | <span data-ttu-id="32716-114">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="32716-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="32716-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32716-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32716-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="32716-116">Not supported.</span></span>    |
|<span data-ttu-id="32716-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="32716-117">Application</span></span> | <span data-ttu-id="32716-118">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32716-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32716-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32716-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="32716-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="32716-120">Request headers</span></span>
| <span data-ttu-id="32716-121">名称</span><span class="sxs-lookup"><span data-stu-id="32716-121">Name</span></span> | <span data-ttu-id="32716-122">说明</span><span class="sxs-lookup"><span data-stu-id="32716-122">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="32716-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32716-123">Authorization</span></span> | <span data-ttu-id="32716-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32716-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32716-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="32716-126">Request body</span></span>
<span data-ttu-id="32716-127">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32716-127">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="32716-128">响应</span><span class="sxs-lookup"><span data-stu-id="32716-128">Response</span></span>
<span data-ttu-id="32716-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32716-129">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="32716-130">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="32716-130">It does not return anything in the response body.</span></span> <span data-ttu-id="32716-131">当对象已是组的成员时，此方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32716-131">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="32716-132">当添加的对象不存在时，此方法返回 `404 Not Found` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32716-132">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span> 

## <a name="example"></a><span data-ttu-id="32716-133">示例</span><span class="sxs-lookup"><span data-stu-id="32716-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="32716-134">请求</span><span class="sxs-lookup"><span data-stu-id="32716-134">Request</span></span>
<span data-ttu-id="32716-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="32716-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32716-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="32716-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="32716-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32716-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32716-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32716-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="32716-139">C#</span><span class="sxs-lookup"><span data-stu-id="32716-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32716-140">Java</span><span class="sxs-lookup"><span data-stu-id="32716-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="32716-141">在请求正文中，提供 `id` 要添加的 [directoryObject](../resources/directoryobject.md)、 [user](../resources/user.md)或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32716-141">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="32716-142">响应</span><span class="sxs-lookup"><span data-stu-id="32716-142">Response</span></span>
<span data-ttu-id="32716-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="32716-143">The following is an example of the response.</span></span>
><span data-ttu-id="32716-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="32716-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


