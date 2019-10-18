---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 86a50debcddc05eeee41279bd20d3dfd5b12081b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337134"
---
# <a name="add-member"></a><span data-ttu-id="6b4ff-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="6b4ff-103">Add member</span></span>
<span data-ttu-id="6b4ff-104">通过 **members** 导航属性将成员添加到 Office 365 组或安全组中。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="6b4ff-105">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-105">You can add users or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="6b4ff-106">仅能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-106">Important: You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b4ff-107">权限</span><span class="sxs-lookup"><span data-stu-id="6b4ff-107">Permissions</span></span>
<span data-ttu-id="6b4ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b4ff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b4ff-110">Permission type</span></span>      | <span data-ttu-id="6b4ff-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b4ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b4ff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b4ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6b4ff-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b4ff-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b4ff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b4ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b4ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-115">Not supported.</span></span>    |
|<span data-ttu-id="6b4ff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b4ff-116">Application</span></span> | <span data-ttu-id="6b4ff-117">Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b4ff-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b4ff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b4ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6b4ff-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b4ff-119">Request headers</span></span>
| <span data-ttu-id="6b4ff-120">名称</span><span class="sxs-lookup"><span data-stu-id="6b4ff-120">Name</span></span>       | <span data-ttu-id="6b4ff-121">类型</span><span class="sxs-lookup"><span data-stu-id="6b4ff-121">Type</span></span> | <span data-ttu-id="6b4ff-122">说明</span><span class="sxs-lookup"><span data-stu-id="6b4ff-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b4ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b4ff-123">Authorization</span></span>  | <span data-ttu-id="6b4ff-124">string</span><span class="sxs-lookup"><span data-stu-id="6b4ff-124">string</span></span>  | <span data-ttu-id="6b4ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b4ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b4ff-127">Request body</span></span>
<span data-ttu-id="6b4ff-128">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="6b4ff-129">响应</span><span class="sxs-lookup"><span data-stu-id="6b4ff-129">Response</span></span>
<span data-ttu-id="6b4ff-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b4ff-132">示例</span><span class="sxs-lookup"><span data-stu-id="6b4ff-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6b4ff-133">请求</span><span class="sxs-lookup"><span data-stu-id="6b4ff-133">Request</span></span>
<span data-ttu-id="6b4ff-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6b4ff-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b4ff-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b4ff-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b4ff-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b4ff-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b4ff-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="6b4ff-138">C#</span><span class="sxs-lookup"><span data-stu-id="6b4ff-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b4ff-139">Java</span><span class="sxs-lookup"><span data-stu-id="6b4ff-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6b4ff-140">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 `id` 的JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-140">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="6b4ff-141">响应</span><span class="sxs-lookup"><span data-stu-id="6b4ff-141">Response</span></span>
<span data-ttu-id="6b4ff-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-142">The following is an example of the response.</span></span>
><span data-ttu-id="6b4ff-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6b4ff-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6b4ff-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
