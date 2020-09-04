---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Microsoft 365 组、安全组或启用邮件的安全组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a9e0ddc322b21d4ac94e6bd3c63f80318be4642
ms.sourcegitcommit: b6ca83070b6f015c09de215a82cf2b581181c33e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2020
ms.locfileid: "47367262"
---
# <a name="add-member"></a><span data-ttu-id="bc2b3-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="bc2b3-103">Add member</span></span>

<span data-ttu-id="bc2b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc2b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc2b3-105">通过 **members** 导航属性将成员添加到 Microsoft 365 组或安全组。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="bc2b3-106">您可以添加用户、组织联系人、服务主体或其他组。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="bc2b3-107">只能向通过云管理的安全和 Microsoft 365 组添加用户。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc2b3-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bc2b3-108">Permissions</span></span>
<span data-ttu-id="bc2b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc2b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc2b3-111">Permission type</span></span>      | <span data-ttu-id="bc2b3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc2b3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc2b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc2b3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc2b3-114">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc2b3-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc2b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc2b3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc2b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-116">Not supported.</span></span>    |
|<span data-ttu-id="bc2b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc2b3-117">Application</span></span> | <span data-ttu-id="bc2b3-118">GroupMember.ReadWrite.All、Group.ReadWrite.All 和 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc2b3-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc2b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc2b3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bc2b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc2b3-120">Request headers</span></span>

| <span data-ttu-id="bc2b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc2b3-121">Header</span></span>       | <span data-ttu-id="bc2b3-122">值</span><span class="sxs-lookup"><span data-stu-id="bc2b3-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bc2b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc2b3-123">Authorization</span></span>  | <span data-ttu-id="bc2b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc2b3-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="bc2b3-126">Content-type</span></span>   | <span data-ttu-id="bc2b3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bc2b3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc2b3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc2b3-129">Request body</span></span>

<span data-ttu-id="bc2b3-130">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md)、[group](../resources/group.md) 或 [organizational contact](../resources/orgcontact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="bc2b3-131">响应</span><span class="sxs-lookup"><span data-stu-id="bc2b3-131">Response</span></span>

<span data-ttu-id="bc2b3-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc2b3-134">示例</span><span class="sxs-lookup"><span data-stu-id="bc2b3-134">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="bc2b3-135">示例1：向组中添加成员</span><span class="sxs-lookup"><span data-stu-id="bc2b3-135">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="bc2b3-136">请求</span><span class="sxs-lookup"><span data-stu-id="bc2b3-136">Request</span></span>

<span data-ttu-id="bc2b3-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

#### <a name="response"></a><span data-ttu-id="bc2b3-138">响应</span><span class="sxs-lookup"><span data-stu-id="bc2b3-138">Response</span></span>
<span data-ttu-id="bc2b3-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="bc2b3-140">示例2：将多个成员添加到单个请求中的组</span><span class="sxs-lookup"><span data-stu-id="bc2b3-140">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="bc2b3-141">本示例演示如何在修补程序操作中将多个成员添加到具有 OData 绑定支持的组中。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-141">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="bc2b3-142">请注意，单个请求中最长可添加20个成员。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-142">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="bc2b3-143">不支持 POST 操作。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-143">The POST operation is not supported.</span></span>

#### <a name="request"></a><span data-ttu-id="bc2b3-144">请求</span><span class="sxs-lookup"><span data-stu-id="bc2b3-144">Request</span></span>

<span data-ttu-id="bc2b3-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
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

#### <a name="response"></a><span data-ttu-id="bc2b3-146">响应</span><span class="sxs-lookup"><span data-stu-id="bc2b3-146">Response</span></span>
<span data-ttu-id="bc2b3-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc2b3-147">The following is an example of the response.</span></span>

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
