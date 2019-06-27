---
title: 'privilegedRole: selfActivate'
description: 激活分配给请求者的角色。
localization_priority: Normal
ms.openlocfilehash: fa7adc82bab9c25ddee6a301a9f65a60481ff7db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268178"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="f8302-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="f8302-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8302-104">激活分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="f8302-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="f8302-105">**注意:** 12月2018日生效, 此 API 将不再受支持且不应使用。</span><span class="sxs-lookup"><span data-stu-id="f8302-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="f8302-106">请改用[Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) 。</span><span class="sxs-lookup"><span data-stu-id="f8302-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="f8302-107">权限</span><span class="sxs-lookup"><span data-stu-id="f8302-107">Permissions</span></span>
<span data-ttu-id="f8302-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8302-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f8302-110">请求者只能调用```selfActivate```分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="f8302-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="f8302-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8302-111">Permission type</span></span>      | <span data-ttu-id="f8302-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8302-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8302-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8302-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f8302-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8302-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8302-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8302-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8302-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8302-116">Not supported.</span></span>    |
|<span data-ttu-id="f8302-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8302-117">Application</span></span> | <span data-ttu-id="f8302-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8302-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8302-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8302-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="f8302-120">请注意``<id>`` , 它是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="f8302-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8302-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8302-121">Request headers</span></span>
| <span data-ttu-id="f8302-122">名称</span><span class="sxs-lookup"><span data-stu-id="f8302-122">Name</span></span>       | <span data-ttu-id="f8302-123">说明</span><span class="sxs-lookup"><span data-stu-id="f8302-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8302-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8302-124">Authorization</span></span>  | <span data-ttu-id="f8302-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8302-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8302-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8302-127">Request body</span></span>
<span data-ttu-id="f8302-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f8302-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8302-129">参数</span><span class="sxs-lookup"><span data-stu-id="f8302-129">Parameter</span></span>    | <span data-ttu-id="f8302-130">类型</span><span class="sxs-lookup"><span data-stu-id="f8302-130">Type</span></span>   |<span data-ttu-id="f8302-131">说明</span><span class="sxs-lookup"><span data-stu-id="f8302-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8302-132">在于</span><span class="sxs-lookup"><span data-stu-id="f8302-132">reason</span></span>|<span data-ttu-id="f8302-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f8302-133">string</span></span>|<span data-ttu-id="f8302-134">可选。</span><span class="sxs-lookup"><span data-stu-id="f8302-134">Optional.</span></span> <span data-ttu-id="f8302-135">有关此角色激活原因的说明。</span><span class="sxs-lookup"><span data-stu-id="f8302-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="f8302-136">duration</span><span class="sxs-lookup"><span data-stu-id="f8302-136">duration</span></span>|<span data-ttu-id="f8302-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f8302-137">string</span></span>|<span data-ttu-id="f8302-138">可选。</span><span class="sxs-lookup"><span data-stu-id="f8302-138">Optional.</span></span> <span data-ttu-id="f8302-139">有效值可以是```min``` (最小激活持续时间) ```default``` 、(角色的默认激活持续时间) 或双精度值来指定激活的小时数。</span><span class="sxs-lookup"><span data-stu-id="f8302-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="f8302-140">指定的持续时间不能长于角色设置中角色的激活持续时间。</span><span class="sxs-lookup"><span data-stu-id="f8302-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="f8302-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="f8302-141">ticketNumber</span></span>|<span data-ttu-id="f8302-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f8302-142">string</span></span>|<span data-ttu-id="f8302-143">可选。</span><span class="sxs-lookup"><span data-stu-id="f8302-143">Optional.</span></span> <span data-ttu-id="f8302-144">用于跟踪此角色激活的票证编号。</span><span class="sxs-lookup"><span data-stu-id="f8302-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="f8302-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="f8302-145">ticketSystem</span></span>|<span data-ttu-id="f8302-146">字符串</span><span class="sxs-lookup"><span data-stu-id="f8302-146">string</span></span>|<span data-ttu-id="f8302-147">可选。</span><span class="sxs-lookup"><span data-stu-id="f8302-147">Optional.</span></span> <span data-ttu-id="f8302-148">票证系统。</span><span class="sxs-lookup"><span data-stu-id="f8302-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="f8302-149">响应</span><span class="sxs-lookup"><span data-stu-id="f8302-149">Response</span></span>

<span data-ttu-id="f8302-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8302-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="f8302-151">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="f8302-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f8302-152">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="f8302-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f8302-153">示例</span><span class="sxs-lookup"><span data-stu-id="f8302-153">Example</span></span>
<span data-ttu-id="f8302-154">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f8302-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8302-155">请求</span><span class="sxs-lookup"><span data-stu-id="f8302-155">Request</span></span>
<span data-ttu-id="f8302-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8302-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f8302-157">响应</span><span class="sxs-lookup"><span data-stu-id="f8302-157">Response</span></span>
<span data-ttu-id="f8302-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f8302-158">Here is an example of the response.</span></span> 

><span data-ttu-id="f8302-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8302-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8302-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f8302-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8302-162">C#</span><span class="sxs-lookup"><span data-stu-id="f8302-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedrole_selfactivate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8302-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8302-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedrole_selfactivate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f8302-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8302-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedrole_selfactivate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
