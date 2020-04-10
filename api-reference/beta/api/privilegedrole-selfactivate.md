---
title: 'privilegedRole: selfActivate'
description: 激活分配给请求者的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 79891be7aa63269cb0d1f96393756f9d41d046d0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218750"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="59966-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="59966-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="59966-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59966-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59966-105">激活分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="59966-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="59966-106">**注意：** 12月2018日生效，此 API 将不再受支持且不应使用。</span><span class="sxs-lookup"><span data-stu-id="59966-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="59966-107">请改用[Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) 。</span><span class="sxs-lookup"><span data-stu-id="59966-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="59966-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="59966-108">Permissions</span></span>
<span data-ttu-id="59966-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59966-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="59966-111">请求者只能调用```selfActivate```分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="59966-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="59966-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="59966-112">Permission type</span></span>      | <span data-ttu-id="59966-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59966-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59966-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59966-114">Delegated (work or school account)</span></span> | <span data-ttu-id="59966-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59966-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="59966-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59966-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59966-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="59966-117">Not supported.</span></span>    |
|<span data-ttu-id="59966-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="59966-118">Application</span></span> | <span data-ttu-id="59966-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="59966-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59966-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59966-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="59966-121">请注意``{id}`` ，它是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="59966-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59966-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="59966-122">Request headers</span></span>
| <span data-ttu-id="59966-123">名称</span><span class="sxs-lookup"><span data-stu-id="59966-123">Name</span></span>       | <span data-ttu-id="59966-124">说明</span><span class="sxs-lookup"><span data-stu-id="59966-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59966-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59966-125">Authorization</span></span>  | <span data-ttu-id="59966-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59966-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59966-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="59966-128">Request body</span></span>
<span data-ttu-id="59966-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="59966-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59966-130">参数</span><span class="sxs-lookup"><span data-stu-id="59966-130">Parameter</span></span>    | <span data-ttu-id="59966-131">类型</span><span class="sxs-lookup"><span data-stu-id="59966-131">Type</span></span>   |<span data-ttu-id="59966-132">说明</span><span class="sxs-lookup"><span data-stu-id="59966-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59966-133">reason</span><span class="sxs-lookup"><span data-stu-id="59966-133">reason</span></span>|<span data-ttu-id="59966-134">string</span><span class="sxs-lookup"><span data-stu-id="59966-134">string</span></span>|<span data-ttu-id="59966-135">可选。</span><span class="sxs-lookup"><span data-stu-id="59966-135">Optional.</span></span> <span data-ttu-id="59966-136">有关此角色激活原因的说明。</span><span class="sxs-lookup"><span data-stu-id="59966-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="59966-137">duration</span><span class="sxs-lookup"><span data-stu-id="59966-137">duration</span></span>|<span data-ttu-id="59966-138">string</span><span class="sxs-lookup"><span data-stu-id="59966-138">string</span></span>|<span data-ttu-id="59966-139">可选。</span><span class="sxs-lookup"><span data-stu-id="59966-139">Optional.</span></span> <span data-ttu-id="59966-140">有效值可以是```min``` （最小激活持续时间） ```default``` 、（角色的默认激活持续时间）或双精度值来指定激活的小时数。</span><span class="sxs-lookup"><span data-stu-id="59966-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="59966-141">指定的持续时间不能长于角色设置中角色的激活持续时间。</span><span class="sxs-lookup"><span data-stu-id="59966-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="59966-142">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="59966-142">ticketNumber</span></span>|<span data-ttu-id="59966-143">string</span><span class="sxs-lookup"><span data-stu-id="59966-143">string</span></span>|<span data-ttu-id="59966-144">可选。</span><span class="sxs-lookup"><span data-stu-id="59966-144">Optional.</span></span> <span data-ttu-id="59966-145">用于跟踪此角色激活的票证编号。</span><span class="sxs-lookup"><span data-stu-id="59966-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="59966-146">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="59966-146">ticketSystem</span></span>|<span data-ttu-id="59966-147">string</span><span class="sxs-lookup"><span data-stu-id="59966-147">string</span></span>|<span data-ttu-id="59966-148">可选。</span><span class="sxs-lookup"><span data-stu-id="59966-148">Optional.</span></span> <span data-ttu-id="59966-149">票证系统。</span><span class="sxs-lookup"><span data-stu-id="59966-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="59966-150">响应</span><span class="sxs-lookup"><span data-stu-id="59966-150">Response</span></span>

<span data-ttu-id="59966-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59966-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="59966-152">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="59966-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="59966-153">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="59966-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="59966-154">示例</span><span class="sxs-lookup"><span data-stu-id="59966-154">Example</span></span>
<span data-ttu-id="59966-155">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="59966-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59966-156">请求</span><span class="sxs-lookup"><span data-stu-id="59966-156">Request</span></span>
<span data-ttu-id="59966-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59966-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59966-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="59966-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="59966-159">C#</span><span class="sxs-lookup"><span data-stu-id="59966-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59966-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59966-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59966-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59966-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59966-162">响应</span><span class="sxs-lookup"><span data-stu-id="59966-162">Response</span></span>
<span data-ttu-id="59966-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="59966-163">Here is an example of the response.</span></span> 

><span data-ttu-id="59966-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="59966-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
