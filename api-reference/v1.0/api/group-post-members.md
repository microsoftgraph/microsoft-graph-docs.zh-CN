---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dba7d42ad8ab4e98061f23b4a56e32237dc2225c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815983"
---
# <a name="add-member"></a><span data-ttu-id="5279d-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="5279d-103">Add member</span></span>

<span data-ttu-id="5279d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5279d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5279d-105">通过 **members** 导航属性将成员添加到 Office 365 组或安全组中。</span><span class="sxs-lookup"><span data-stu-id="5279d-105">Add a member to an Office 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="5279d-106">可以添加用户、组织联系人或其他组。</span><span class="sxs-lookup"><span data-stu-id="5279d-106">You can add users, organizational contacts, or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="5279d-107">只能向通过云管理的安全组和 Office 365 组添加用户。</span><span class="sxs-lookup"><span data-stu-id="5279d-107">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="5279d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="5279d-108">Permissions</span></span>
<span data-ttu-id="5279d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5279d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5279d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5279d-111">Permission type</span></span>      | <span data-ttu-id="5279d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5279d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5279d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5279d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5279d-114">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5279d-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5279d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5279d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5279d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5279d-116">Not supported.</span></span>    |
|<span data-ttu-id="5279d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5279d-117">Application</span></span> | <span data-ttu-id="5279d-118">GroupMember.ReadWrite.All、Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5279d-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5279d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5279d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5279d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5279d-120">Request headers</span></span>
| <span data-ttu-id="5279d-121">标头</span><span class="sxs-lookup"><span data-stu-id="5279d-121">Header</span></span>       | <span data-ttu-id="5279d-122">值</span><span class="sxs-lookup"><span data-stu-id="5279d-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5279d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5279d-123">Authorization</span></span>  | <span data-ttu-id="5279d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5279d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5279d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="5279d-126">Content-type</span></span>   | <span data-ttu-id="5279d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5279d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5279d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5279d-129">Request body</span></span>
<span data-ttu-id="5279d-130">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md)、[group](../resources/group.md) 或 [organizational contact](../resources/orgcontact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5279d-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5279d-131">响应</span><span class="sxs-lookup"><span data-stu-id="5279d-131">Response</span></span>
<span data-ttu-id="5279d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5279d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5279d-134">示例</span><span class="sxs-lookup"><span data-stu-id="5279d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5279d-135">请求</span><span class="sxs-lookup"><span data-stu-id="5279d-135">Request</span></span>
<span data-ttu-id="5279d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5279d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5279d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5279d-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="5279d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5279d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5279d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5279d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="5279d-140">C#</span><span class="sxs-lookup"><span data-stu-id="5279d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5279d-141">Java</span><span class="sxs-lookup"><span data-stu-id="5279d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5279d-142">响应</span><span class="sxs-lookup"><span data-stu-id="5279d-142">Response</span></span>
<span data-ttu-id="5279d-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5279d-143">The following is an example of the response.</span></span>

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
