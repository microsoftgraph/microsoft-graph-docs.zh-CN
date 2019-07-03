---
title: 添加成员
description: 使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9a819ee95010a6702aabf55c92f0106716fdd80d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456391"
---
# <a name="add-member"></a><span data-ttu-id="b2101-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="b2101-103">Add member</span></span>
<span data-ttu-id="b2101-104">使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。</span><span class="sxs-lookup"><span data-stu-id="b2101-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="b2101-105">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="b2101-105">You can add users or other groups.</span></span> <span data-ttu-id="b2101-106">重要说明：只能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="b2101-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2101-107">权限</span><span class="sxs-lookup"><span data-stu-id="b2101-107">Permissions</span></span>
<span data-ttu-id="b2101-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2101-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2101-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2101-110">Permission type</span></span>      | <span data-ttu-id="b2101-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2101-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2101-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2101-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2101-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2101-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2101-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2101-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2101-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2101-115">Not supported.</span></span>    |
|<span data-ttu-id="b2101-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2101-116">Application</span></span> | <span data-ttu-id="b2101-117">Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2101-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2101-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2101-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b2101-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2101-119">Request headers</span></span>
| <span data-ttu-id="b2101-120">名称</span><span class="sxs-lookup"><span data-stu-id="b2101-120">Name</span></span>       | <span data-ttu-id="b2101-121">类型</span><span class="sxs-lookup"><span data-stu-id="b2101-121">Type</span></span> | <span data-ttu-id="b2101-122">说明</span><span class="sxs-lookup"><span data-stu-id="b2101-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2101-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2101-123">Authorization</span></span>  | <span data-ttu-id="b2101-124">string</span><span class="sxs-lookup"><span data-stu-id="b2101-124">string</span></span>  | <span data-ttu-id="b2101-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2101-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2101-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2101-127">Request body</span></span>
<span data-ttu-id="b2101-128">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2101-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b2101-129">响应</span><span class="sxs-lookup"><span data-stu-id="b2101-129">Response</span></span>
<span data-ttu-id="b2101-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b2101-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2101-132">示例</span><span class="sxs-lookup"><span data-stu-id="b2101-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b2101-133">请求</span><span class="sxs-lookup"><span data-stu-id="b2101-133">Request</span></span>
<span data-ttu-id="b2101-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2101-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2101-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2101-135">--Http</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2101-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b2101-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2101-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2101-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b2101-138">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 `id` 的JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2101-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="b2101-139">响应</span><span class="sxs-lookup"><span data-stu-id="b2101-139">Response</span></span>
<span data-ttu-id="b2101-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b2101-140">The following is an example of the response.</span></span>
><span data-ttu-id="b2101-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2101-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b2101-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b2101-142">All the properties will be returned from an actual call.</span></span>
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
