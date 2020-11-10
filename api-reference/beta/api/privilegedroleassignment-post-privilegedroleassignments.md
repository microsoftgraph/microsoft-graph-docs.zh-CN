---
title: 创建 privilegedRoleAssignment
description: 使用此 API 创建新的 privilegedRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3bb20ddcc8d1746ce1e567f6ce951d9e4c57ed62
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981959"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="0aec3-103">创建 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0aec3-103">Create privilegedRoleAssignment</span></span>

<span data-ttu-id="0aec3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aec3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aec3-105">使用此 API 创建新的  [privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="0aec3-105">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0aec3-106">权限</span><span class="sxs-lookup"><span data-stu-id="0aec3-106">Permissions</span></span>
<span data-ttu-id="0aec3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0aec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0aec3-109">请求者需要具有 _特权角色管理员_ 角色。</span><span class="sxs-lookup"><span data-stu-id="0aec3-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="0aec3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0aec3-110">Permission type</span></span>      | <span data-ttu-id="0aec3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0aec3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aec3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0aec3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0aec3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0aec3-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0aec3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0aec3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aec3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0aec3-115">Not supported.</span></span>    |
|<span data-ttu-id="0aec3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0aec3-116">Application</span></span> | <span data-ttu-id="0aec3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0aec3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aec3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0aec3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="0aec3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0aec3-119">Request headers</span></span>
| <span data-ttu-id="0aec3-120">名称</span><span class="sxs-lookup"><span data-stu-id="0aec3-120">Name</span></span>       | <span data-ttu-id="0aec3-121">说明</span><span class="sxs-lookup"><span data-stu-id="0aec3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0aec3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aec3-122">Authorization</span></span>  | <span data-ttu-id="0aec3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0aec3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aec3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0aec3-125">Request body</span></span>
<span data-ttu-id="0aec3-126">在请求正文中，提供 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aec3-126">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0aec3-127">响应</span><span class="sxs-lookup"><span data-stu-id="0aec3-127">Response</span></span>

<span data-ttu-id="0aec3-128">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0aec3-128">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="0aec3-129">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="0aec3-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0aec3-130">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="0aec3-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="0aec3-131">示例</span><span class="sxs-lookup"><span data-stu-id="0aec3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aec3-132">请求</span><span class="sxs-lookup"><span data-stu-id="0aec3-132">Request</span></span>
<span data-ttu-id="0aec3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0aec3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0aec3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0aec3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="0aec3-135">C#</span><span class="sxs-lookup"><span data-stu-id="0aec3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0aec3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0aec3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0aec3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0aec3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0aec3-138">Java</span><span class="sxs-lookup"><span data-stu-id="0aec3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0aec3-139">在请求正文中，提供 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aec3-139">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0aec3-140">响应</span><span class="sxs-lookup"><span data-stu-id="0aec3-140">Response</span></span>
<span data-ttu-id="0aec3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0aec3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


