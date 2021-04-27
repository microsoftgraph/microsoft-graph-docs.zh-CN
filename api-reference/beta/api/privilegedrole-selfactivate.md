---
title: privilegedRole： selfActivate
description: 激活分配给请求者的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 970435589de932ad10051196ef51da8764444260
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055251"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="46bb3-103">privilegedRole： selfActivate</span><span class="sxs-lookup"><span data-stu-id="46bb3-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="46bb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46bb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46bb3-105">激活分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="46bb3-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="46bb3-106">**注意：** 自 2018 年 12 月起，将不再支持此 API，也不应使用。</span><span class="sxs-lookup"><span data-stu-id="46bb3-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="46bb3-107">请[改为使用 Create PrivilegedRoleAssignmentRequest。](privilegedroleassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="46bb3-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="46bb3-108">权限</span><span class="sxs-lookup"><span data-stu-id="46bb3-108">Permissions</span></span>
<span data-ttu-id="46bb3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46bb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="46bb3-111">请求者只能 ```selfActivate``` 调用分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="46bb3-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="46bb3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="46bb3-112">Permission type</span></span>      | <span data-ttu-id="46bb3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46bb3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46bb3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46bb3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="46bb3-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46bb3-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46bb3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46bb3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46bb3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="46bb3-117">Not supported.</span></span>    |
|<span data-ttu-id="46bb3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="46bb3-118">Application</span></span> | <span data-ttu-id="46bb3-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="46bb3-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46bb3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46bb3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="46bb3-121">请注意 ``{id}`` ，这是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="46bb3-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="46bb3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="46bb3-122">Request headers</span></span>
| <span data-ttu-id="46bb3-123">名称</span><span class="sxs-lookup"><span data-stu-id="46bb3-123">Name</span></span>       | <span data-ttu-id="46bb3-124">说明</span><span class="sxs-lookup"><span data-stu-id="46bb3-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46bb3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="46bb3-125">Authorization</span></span>  | <span data-ttu-id="46bb3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46bb3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46bb3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="46bb3-128">Request body</span></span>
<span data-ttu-id="46bb3-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="46bb3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46bb3-130">参数</span><span class="sxs-lookup"><span data-stu-id="46bb3-130">Parameter</span></span>    | <span data-ttu-id="46bb3-131">类型</span><span class="sxs-lookup"><span data-stu-id="46bb3-131">Type</span></span>   |<span data-ttu-id="46bb3-132">说明</span><span class="sxs-lookup"><span data-stu-id="46bb3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46bb3-133">reason</span><span class="sxs-lookup"><span data-stu-id="46bb3-133">reason</span></span>|<span data-ttu-id="46bb3-134">string</span><span class="sxs-lookup"><span data-stu-id="46bb3-134">string</span></span>|<span data-ttu-id="46bb3-135">可选。</span><span class="sxs-lookup"><span data-stu-id="46bb3-135">Optional.</span></span> <span data-ttu-id="46bb3-136">有关此角色激活原因的说明。</span><span class="sxs-lookup"><span data-stu-id="46bb3-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="46bb3-137">duration</span><span class="sxs-lookup"><span data-stu-id="46bb3-137">duration</span></span>|<span data-ttu-id="46bb3-138">string</span><span class="sxs-lookup"><span data-stu-id="46bb3-138">string</span></span>|<span data-ttu-id="46bb3-139">可选。</span><span class="sxs-lookup"><span data-stu-id="46bb3-139">Optional.</span></span> <span data-ttu-id="46bb3-140">有效值可以是 (最短激活) 、 (角色) 的默认激活持续时间或一个双精度值来指定激活 ```min``` ```default``` 小时数。</span><span class="sxs-lookup"><span data-stu-id="46bb3-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="46bb3-141">指定持续时间不能长于角色设置中角色的激活持续时间。</span><span class="sxs-lookup"><span data-stu-id="46bb3-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="46bb3-142">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="46bb3-142">ticketNumber</span></span>|<span data-ttu-id="46bb3-143">string</span><span class="sxs-lookup"><span data-stu-id="46bb3-143">string</span></span>|<span data-ttu-id="46bb3-144">可选。</span><span class="sxs-lookup"><span data-stu-id="46bb3-144">Optional.</span></span> <span data-ttu-id="46bb3-145">用于跟踪此角色激活的票证编号。</span><span class="sxs-lookup"><span data-stu-id="46bb3-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="46bb3-146">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="46bb3-146">ticketSystem</span></span>|<span data-ttu-id="46bb3-147">string</span><span class="sxs-lookup"><span data-stu-id="46bb3-147">string</span></span>|<span data-ttu-id="46bb3-148">可选。</span><span class="sxs-lookup"><span data-stu-id="46bb3-148">Optional.</span></span> <span data-ttu-id="46bb3-149">票证系统。</span><span class="sxs-lookup"><span data-stu-id="46bb3-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="46bb3-150">响应</span><span class="sxs-lookup"><span data-stu-id="46bb3-150">Response</span></span>

<span data-ttu-id="46bb3-151">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46bb3-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="46bb3-152">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="46bb3-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="46bb3-153">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="46bb3-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="46bb3-154">示例</span><span class="sxs-lookup"><span data-stu-id="46bb3-154">Example</span></span>
<span data-ttu-id="46bb3-155">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="46bb3-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46bb3-156">请求</span><span class="sxs-lookup"><span data-stu-id="46bb3-156">Request</span></span>
<span data-ttu-id="46bb3-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46bb3-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46bb3-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="46bb3-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="c"></a>[<span data-ttu-id="46bb3-159">C#</span><span class="sxs-lookup"><span data-stu-id="46bb3-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46bb3-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46bb3-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46bb3-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46bb3-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46bb3-162">Java</span><span class="sxs-lookup"><span data-stu-id="46bb3-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="46bb3-163">响应</span><span class="sxs-lookup"><span data-stu-id="46bb3-163">Response</span></span>
<span data-ttu-id="46bb3-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="46bb3-164">Here is an example of the response.</span></span> 

><span data-ttu-id="46bb3-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="46bb3-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


