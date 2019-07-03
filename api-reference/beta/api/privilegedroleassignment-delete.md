---
title: Delete privilegedRoleAssignment
description: 删除 privilegedRoleAssignment。
localization_priority: Normal
ms.openlocfilehash: 76db67452db136d126774f2b7c93e372e7e582f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444993"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="45a2f-103">Delete privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="45a2f-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a2f-104">删除[privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="45a2f-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="45a2f-105">权限</span><span class="sxs-lookup"><span data-stu-id="45a2f-105">Permissions</span></span>
<span data-ttu-id="45a2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45a2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="45a2f-108">请求者需要具有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="45a2f-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="45a2f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45a2f-109">Permission type</span></span>      | <span data-ttu-id="45a2f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45a2f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45a2f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45a2f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45a2f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45a2f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="45a2f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45a2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45a2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45a2f-114">Not supported.</span></span>    |
|<span data-ttu-id="45a2f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45a2f-115">Application</span></span> | <span data-ttu-id="45a2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45a2f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45a2f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45a2f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="45a2f-118">``<id>``请注意, 格式为 "userId_roleId", 其中 UserId 是 azure AD 用户 ID 的 guid 字符串, RoleId 是 azure 管理员角色 ID 的 guid 字符串。</span><span class="sxs-lookup"><span data-stu-id="45a2f-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45a2f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="45a2f-119">Request headers</span></span>
| <span data-ttu-id="45a2f-120">名称</span><span class="sxs-lookup"><span data-stu-id="45a2f-120">Name</span></span>       | <span data-ttu-id="45a2f-121">说明</span><span class="sxs-lookup"><span data-stu-id="45a2f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45a2f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45a2f-122">Authorization</span></span>  | <span data-ttu-id="45a2f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45a2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45a2f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="45a2f-125">Request body</span></span>
<span data-ttu-id="45a2f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45a2f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45a2f-127">响应</span><span class="sxs-lookup"><span data-stu-id="45a2f-127">Response</span></span>

<span data-ttu-id="45a2f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="45a2f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="45a2f-130">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="45a2f-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="45a2f-131">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="45a2f-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="45a2f-132">示例</span><span class="sxs-lookup"><span data-stu-id="45a2f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45a2f-133">请求</span><span class="sxs-lookup"><span data-stu-id="45a2f-133">Request</span></span>
<span data-ttu-id="45a2f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45a2f-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="45a2f-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="45a2f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45a2f-136">C#</span><span class="sxs-lookup"><span data-stu-id="45a2f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45a2f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="45a2f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45a2f-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="45a2f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="45a2f-139">响应</span><span class="sxs-lookup"><span data-stu-id="45a2f-139">Response</span></span>
<span data-ttu-id="45a2f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45a2f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
