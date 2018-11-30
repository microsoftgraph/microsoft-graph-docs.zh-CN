---
title: 删除 privilegedRoleAssignment
description: 删除 privilegedRoleAssignment。
ms.openlocfilehash: 345ebbfbf32a8d5e6f9399e5746ca9ece9b91d3b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042758"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="6020c-103">删除 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6020c-103">Delete privilegedRoleAssignment</span></span>

> <span data-ttu-id="6020c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6020c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6020c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6020c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6020c-106">删除[privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="6020c-106">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6020c-107">权限</span><span class="sxs-lookup"><span data-stu-id="6020c-107">Permissions</span></span>
<span data-ttu-id="6020c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6020c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6020c-110">请求者需要有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="6020c-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="6020c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6020c-111">Permission type</span></span>      | <span data-ttu-id="6020c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6020c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6020c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6020c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6020c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6020c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6020c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6020c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6020c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6020c-116">Not supported.</span></span>    |
|<span data-ttu-id="6020c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6020c-117">Application</span></span> | <span data-ttu-id="6020c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6020c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6020c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6020c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="6020c-120">请注意， ``<id>`` userId_roleId，其中 userId 是 Azure AD 用户 id 的 GUID 字符串，roleId 是 Azure 管理员角色 id 的 GUID 字符串的格式。</span><span class="sxs-lookup"><span data-stu-id="6020c-120">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6020c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6020c-121">Request headers</span></span>
| <span data-ttu-id="6020c-122">名称</span><span class="sxs-lookup"><span data-stu-id="6020c-122">Name</span></span>       | <span data-ttu-id="6020c-123">说明</span><span class="sxs-lookup"><span data-stu-id="6020c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6020c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6020c-124">Authorization</span></span>  | <span data-ttu-id="6020c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6020c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6020c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6020c-127">Request body</span></span>
<span data-ttu-id="6020c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6020c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6020c-129">响应</span><span class="sxs-lookup"><span data-stu-id="6020c-129">Response</span></span>

<span data-ttu-id="6020c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6020c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="6020c-132">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="6020c-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6020c-133">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="6020c-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6020c-134">示例</span><span class="sxs-lookup"><span data-stu-id="6020c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6020c-135">请求</span><span class="sxs-lookup"><span data-stu-id="6020c-135">Request</span></span>
<span data-ttu-id="6020c-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6020c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="6020c-137">响应</span><span class="sxs-lookup"><span data-stu-id="6020c-137">Response</span></span>
<span data-ttu-id="6020c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6020c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->