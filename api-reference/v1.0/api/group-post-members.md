---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Microsoft 365 组、安全组或启用邮件的安全组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6ffb969b08704ac8235fe630e89c9bec65a140f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057428"
---
# <a name="add-member"></a><span data-ttu-id="342a0-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="342a0-103">Add member</span></span>

<span data-ttu-id="342a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="342a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="342a0-105">通过 **members** 导航属性将成员添加到 Microsoft 365 组或安全组中。</span><span class="sxs-lookup"><span data-stu-id="342a0-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="342a0-106">可以添加用户、组织联系人、服务主体或其他组。</span><span class="sxs-lookup"><span data-stu-id="342a0-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="342a0-107">只能向通过云管理的安全组和 Microsoft 365 组添加用户。</span><span class="sxs-lookup"><span data-stu-id="342a0-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="342a0-108">权限</span><span class="sxs-lookup"><span data-stu-id="342a0-108">Permissions</span></span>

<span data-ttu-id="342a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="342a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="342a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="342a0-111">Permission type</span></span>      | <span data-ttu-id="342a0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="342a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="342a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="342a0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="342a0-114">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="342a0-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="342a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="342a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="342a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="342a0-116">Not supported.</span></span>    |
|<span data-ttu-id="342a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="342a0-117">Application</span></span> | <span data-ttu-id="342a0-118">GroupMember.ReadWrite.All、Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="342a0-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="342a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="342a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="342a0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="342a0-120">Request headers</span></span>

| <span data-ttu-id="342a0-121">标头</span><span class="sxs-lookup"><span data-stu-id="342a0-121">Header</span></span>       | <span data-ttu-id="342a0-122">值</span><span class="sxs-lookup"><span data-stu-id="342a0-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="342a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="342a0-123">Authorization</span></span>  | <span data-ttu-id="342a0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="342a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="342a0-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="342a0-126">Content-type</span></span>   | <span data-ttu-id="342a0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="342a0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="342a0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="342a0-129">Request body</span></span>

<span data-ttu-id="342a0-130">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md)、[group](../resources/group.md) 或 [organizational contact](../resources/orgcontact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="342a0-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="342a0-131">响应</span><span class="sxs-lookup"><span data-stu-id="342a0-131">Response</span></span>

<span data-ttu-id="342a0-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="342a0-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="342a0-134">示例</span><span class="sxs-lookup"><span data-stu-id="342a0-134">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="342a0-135">示例 1：将成员添加到组</span><span class="sxs-lookup"><span data-stu-id="342a0-135">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="342a0-136">请求</span><span class="sxs-lookup"><span data-stu-id="342a0-136">Request</span></span>

<span data-ttu-id="342a0-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="342a0-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="342a0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="342a0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="342a0-139">C#</span><span class="sxs-lookup"><span data-stu-id="342a0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="342a0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="342a0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="342a0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="342a0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="342a0-142">Java</span><span class="sxs-lookup"><span data-stu-id="342a0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="342a0-143">在请求正文中，提供要添加的 directoryObject、user 或 group 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="342a0-143">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="342a0-144">响应</span><span class="sxs-lookup"><span data-stu-id="342a0-144">Response</span></span>

<span data-ttu-id="342a0-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="342a0-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="342a0-146">示例 2：在单个请求中向组添加多个成员</span><span class="sxs-lookup"><span data-stu-id="342a0-146">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="342a0-147">此示例说明了如何在 PATCH 操作中通过 OData 绑定支持向组添加多个成员。</span><span class="sxs-lookup"><span data-stu-id="342a0-147">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="342a0-148">请注意，在单个请求中最多可以添加 20 个成员。</span><span class="sxs-lookup"><span data-stu-id="342a0-148">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="342a0-149">不支持 POST 操作。</span><span class="sxs-lookup"><span data-stu-id="342a0-149">The POST operation is not supported.</span></span>

#### <a name="request"></a><span data-ttu-id="342a0-150">请求</span><span class="sxs-lookup"><span data-stu-id="342a0-150">Request</span></span>

<span data-ttu-id="342a0-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="342a0-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="342a0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="342a0-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{group-id}
Content-type: application/json
Content-length: 30

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="342a0-153">C#</span><span class="sxs-lookup"><span data-stu-id="342a0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="342a0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="342a0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="342a0-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="342a0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="342a0-156">Java</span><span class="sxs-lookup"><span data-stu-id="342a0-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="342a0-157">在请求正文中，提供要添加的 directoryObject、user 或 group 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="342a0-157">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="342a0-158">响应</span><span class="sxs-lookup"><span data-stu-id="342a0-158">Response</span></span>
<span data-ttu-id="342a0-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="342a0-159">The following is an example of the response.</span></span>

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

