---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c43bded94b1c5fd683c2ca5ca72515a12ce2ec9b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999407"
---
# <a name="add-member"></a><span data-ttu-id="45008-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="45008-103">Add member</span></span>
<span data-ttu-id="45008-104">通过 **members** 导航属性将成员添加到 Office 365 组或安全组中。</span><span class="sxs-lookup"><span data-stu-id="45008-104">Add a member to an Office 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="45008-105">可以添加用户、组织联系人或其他组。</span><span class="sxs-lookup"><span data-stu-id="45008-105">You can add users, organizational contacts, or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="45008-106">只能向通过云管理的安全组和 Office 365 组添加用户。</span><span class="sxs-lookup"><span data-stu-id="45008-106">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="45008-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="45008-107">Permissions</span></span>
<span data-ttu-id="45008-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45008-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="45008-110">Permission type</span></span>      | <span data-ttu-id="45008-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45008-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45008-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45008-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45008-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45008-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="45008-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45008-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45008-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="45008-115">Not supported.</span></span>    |
|<span data-ttu-id="45008-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="45008-116">Application</span></span> | <span data-ttu-id="45008-117">Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45008-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45008-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45008-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="45008-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="45008-119">Request headers</span></span>
| <span data-ttu-id="45008-120">标头</span><span class="sxs-lookup"><span data-stu-id="45008-120">Header</span></span>       | <span data-ttu-id="45008-121">值</span><span class="sxs-lookup"><span data-stu-id="45008-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="45008-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45008-122">Authorization</span></span>  | <span data-ttu-id="45008-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45008-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45008-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="45008-125">Content-type</span></span>   | <span data-ttu-id="45008-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="45008-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45008-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="45008-128">Request body</span></span>
<span data-ttu-id="45008-129">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md)、[group](../resources/group.md) 或 [organizational contact](../resources/orgcontact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45008-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="45008-130">响应</span><span class="sxs-lookup"><span data-stu-id="45008-130">Response</span></span>
<span data-ttu-id="45008-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="45008-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45008-133">示例</span><span class="sxs-lookup"><span data-stu-id="45008-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="45008-134">请求</span><span class="sxs-lookup"><span data-stu-id="45008-134">Request</span></span>
<span data-ttu-id="45008-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45008-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="45008-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="45008-136">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45008-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45008-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45008-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45008-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="45008-139">C#</span><span class="sxs-lookup"><span data-stu-id="45008-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="45008-140">Java</span><span class="sxs-lookup"><span data-stu-id="45008-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="45008-141">响应</span><span class="sxs-lookup"><span data-stu-id="45008-141">Response</span></span>
<span data-ttu-id="45008-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45008-142">The following is an example of the response.</span></span>

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
