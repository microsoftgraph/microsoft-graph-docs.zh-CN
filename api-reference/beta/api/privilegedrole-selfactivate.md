---
title: 'privilegedRole: selfActivate'
description: 激活分配给请求者的角色。
localization_priority: Normal
ms.openlocfilehash: f2a8db8b56af011be1f5a07c02b730da1faa242c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445021"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="dfc08-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="dfc08-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfc08-104">激活分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="dfc08-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="dfc08-105">**注意:** 12月2018日生效, 此 API 将不再受支持且不应使用。</span><span class="sxs-lookup"><span data-stu-id="dfc08-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="dfc08-106">请改用[Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) 。</span><span class="sxs-lookup"><span data-stu-id="dfc08-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="dfc08-107">权限</span><span class="sxs-lookup"><span data-stu-id="dfc08-107">Permissions</span></span>
<span data-ttu-id="dfc08-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfc08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dfc08-110">请求者只能调用```selfActivate```分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="dfc08-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="dfc08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfc08-111">Permission type</span></span>      | <span data-ttu-id="dfc08-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfc08-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfc08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfc08-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc08-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfc08-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfc08-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfc08-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfc08-116">Not supported.</span></span>    |
|<span data-ttu-id="dfc08-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfc08-117">Application</span></span> | <span data-ttu-id="dfc08-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfc08-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfc08-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfc08-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="dfc08-120">请注意``<id>`` , 它是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="dfc08-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dfc08-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfc08-121">Request headers</span></span>
| <span data-ttu-id="dfc08-122">名称</span><span class="sxs-lookup"><span data-stu-id="dfc08-122">Name</span></span>       | <span data-ttu-id="dfc08-123">说明</span><span class="sxs-lookup"><span data-stu-id="dfc08-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dfc08-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfc08-124">Authorization</span></span>  | <span data-ttu-id="dfc08-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfc08-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfc08-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfc08-127">Request body</span></span>
<span data-ttu-id="dfc08-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dfc08-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dfc08-129">参数</span><span class="sxs-lookup"><span data-stu-id="dfc08-129">Parameter</span></span>    | <span data-ttu-id="dfc08-130">类型</span><span class="sxs-lookup"><span data-stu-id="dfc08-130">Type</span></span>   |<span data-ttu-id="dfc08-131">说明</span><span class="sxs-lookup"><span data-stu-id="dfc08-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfc08-132">在于</span><span class="sxs-lookup"><span data-stu-id="dfc08-132">reason</span></span>|<span data-ttu-id="dfc08-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dfc08-133">string</span></span>|<span data-ttu-id="dfc08-134">可选。</span><span class="sxs-lookup"><span data-stu-id="dfc08-134">Optional.</span></span> <span data-ttu-id="dfc08-135">有关此角色激活原因的说明。</span><span class="sxs-lookup"><span data-stu-id="dfc08-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="dfc08-136">duration</span><span class="sxs-lookup"><span data-stu-id="dfc08-136">duration</span></span>|<span data-ttu-id="dfc08-137">字符串</span><span class="sxs-lookup"><span data-stu-id="dfc08-137">string</span></span>|<span data-ttu-id="dfc08-138">可选。</span><span class="sxs-lookup"><span data-stu-id="dfc08-138">Optional.</span></span> <span data-ttu-id="dfc08-139">有效值可以是```min``` (最小激活持续时间) ```default``` 、(角色的默认激活持续时间) 或双精度值来指定激活的小时数。</span><span class="sxs-lookup"><span data-stu-id="dfc08-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="dfc08-140">指定的持续时间不能长于角色设置中角色的激活持续时间。</span><span class="sxs-lookup"><span data-stu-id="dfc08-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="dfc08-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="dfc08-141">ticketNumber</span></span>|<span data-ttu-id="dfc08-142">字符串</span><span class="sxs-lookup"><span data-stu-id="dfc08-142">string</span></span>|<span data-ttu-id="dfc08-143">可选。</span><span class="sxs-lookup"><span data-stu-id="dfc08-143">Optional.</span></span> <span data-ttu-id="dfc08-144">用于跟踪此角色激活的票证编号。</span><span class="sxs-lookup"><span data-stu-id="dfc08-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="dfc08-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="dfc08-145">ticketSystem</span></span>|<span data-ttu-id="dfc08-146">字符串</span><span class="sxs-lookup"><span data-stu-id="dfc08-146">string</span></span>|<span data-ttu-id="dfc08-147">可选。</span><span class="sxs-lookup"><span data-stu-id="dfc08-147">Optional.</span></span> <span data-ttu-id="dfc08-148">票证系统。</span><span class="sxs-lookup"><span data-stu-id="dfc08-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="dfc08-149">响应</span><span class="sxs-lookup"><span data-stu-id="dfc08-149">Response</span></span>

<span data-ttu-id="dfc08-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfc08-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="dfc08-151">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="dfc08-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dfc08-152">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="dfc08-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="dfc08-153">示例</span><span class="sxs-lookup"><span data-stu-id="dfc08-153">Example</span></span>
<span data-ttu-id="dfc08-154">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="dfc08-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dfc08-155">请求</span><span class="sxs-lookup"><span data-stu-id="dfc08-155">Request</span></span>
<span data-ttu-id="dfc08-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfc08-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dfc08-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dfc08-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dfc08-158">C#</span><span class="sxs-lookup"><span data-stu-id="dfc08-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfc08-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfc08-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dfc08-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfc08-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dfc08-161">响应</span><span class="sxs-lookup"><span data-stu-id="dfc08-161">Response</span></span>
<span data-ttu-id="dfc08-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dfc08-162">Here is an example of the response.</span></span> 

><span data-ttu-id="dfc08-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dfc08-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
