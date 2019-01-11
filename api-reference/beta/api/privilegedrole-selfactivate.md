---
title: 'privilegedRole: selfActivate'
description: 激活分配给请求者角色。
localization_priority: Normal
ms.openlocfilehash: 9423d87714fcd4a7b7cce1dd5cd03bcef3e0ef9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872126"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="03151-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="03151-103">privilegedRole: selfActivate</span></span>

><span data-ttu-id="03151-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03151-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03151-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03151-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03151-106">激活分配给请求者角色。</span><span class="sxs-lookup"><span data-stu-id="03151-106">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="03151-107">**注意：** 有效年 12 月 2018年此 API 将不再支持和不应使用。</span><span class="sxs-lookup"><span data-stu-id="03151-107">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="03151-108">请改用[创建 PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) 。</span><span class="sxs-lookup"><span data-stu-id="03151-108">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="03151-109">权限</span><span class="sxs-lookup"><span data-stu-id="03151-109">Permissions</span></span>
<span data-ttu-id="03151-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03151-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="03151-112">请求者只能调用```selfActivate```角色分配给他。</span><span class="sxs-lookup"><span data-stu-id="03151-112">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="03151-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="03151-113">Permission type</span></span>      | <span data-ttu-id="03151-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03151-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03151-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03151-115">Delegated (work or school account)</span></span> | <span data-ttu-id="03151-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03151-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03151-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03151-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03151-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="03151-118">Not supported.</span></span>    |
|<span data-ttu-id="03151-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="03151-119">Application</span></span> | <span data-ttu-id="03151-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="03151-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03151-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03151-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="03151-122">请注意，``<id>``是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="03151-122">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="03151-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="03151-123">Request headers</span></span>
| <span data-ttu-id="03151-124">名称</span><span class="sxs-lookup"><span data-stu-id="03151-124">Name</span></span>       | <span data-ttu-id="03151-125">说明</span><span class="sxs-lookup"><span data-stu-id="03151-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03151-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="03151-126">Authorization</span></span>  | <span data-ttu-id="03151-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03151-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03151-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="03151-129">Request body</span></span>
<span data-ttu-id="03151-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="03151-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03151-131">参数</span><span class="sxs-lookup"><span data-stu-id="03151-131">Parameter</span></span>    | <span data-ttu-id="03151-132">类型</span><span class="sxs-lookup"><span data-stu-id="03151-132">Type</span></span>   |<span data-ttu-id="03151-133">Description</span><span class="sxs-lookup"><span data-stu-id="03151-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03151-134">原因</span><span class="sxs-lookup"><span data-stu-id="03151-134">reason</span></span>|<span data-ttu-id="03151-135">string</span><span class="sxs-lookup"><span data-stu-id="03151-135">string</span></span>|<span data-ttu-id="03151-136">可选。</span><span class="sxs-lookup"><span data-stu-id="03151-136">Optional.</span></span> <span data-ttu-id="03151-137">有关此角色激活的原因的说明。</span><span class="sxs-lookup"><span data-stu-id="03151-137">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="03151-138">duration</span><span class="sxs-lookup"><span data-stu-id="03151-138">duration</span></span>|<span data-ttu-id="03151-139">string</span><span class="sxs-lookup"><span data-stu-id="03151-139">string</span></span>|<span data-ttu-id="03151-140">可选。</span><span class="sxs-lookup"><span data-stu-id="03151-140">Optional.</span></span> <span data-ttu-id="03151-141">有效的值可以是```min```（最少激活持续时间） ```default``` （默认激活持续时间的角色），或可指定小时数，则激活一个 double 值。</span><span class="sxs-lookup"><span data-stu-id="03151-141">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="03151-142">指定的持续时间不能超过从角色设置的角色激活持续时间。</span><span class="sxs-lookup"><span data-stu-id="03151-142">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="03151-143">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="03151-143">ticketNumber</span></span>|<span data-ttu-id="03151-144">string</span><span class="sxs-lookup"><span data-stu-id="03151-144">string</span></span>|<span data-ttu-id="03151-145">可选。</span><span class="sxs-lookup"><span data-stu-id="03151-145">Optional.</span></span> <span data-ttu-id="03151-146">用于跟踪此角色激活票证数量。</span><span class="sxs-lookup"><span data-stu-id="03151-146">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="03151-147">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="03151-147">ticketSystem</span></span>|<span data-ttu-id="03151-148">string</span><span class="sxs-lookup"><span data-stu-id="03151-148">string</span></span>|<span data-ttu-id="03151-149">可选。</span><span class="sxs-lookup"><span data-stu-id="03151-149">Optional.</span></span> <span data-ttu-id="03151-150">票证系统。</span><span class="sxs-lookup"><span data-stu-id="03151-150">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="03151-151">响应</span><span class="sxs-lookup"><span data-stu-id="03151-151">Response</span></span>

<span data-ttu-id="03151-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="03151-152">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="03151-153">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="03151-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="03151-154">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="03151-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="03151-155">示例</span><span class="sxs-lookup"><span data-stu-id="03151-155">Example</span></span>
<span data-ttu-id="03151-156">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="03151-156">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03151-157">请求</span><span class="sxs-lookup"><span data-stu-id="03151-157">Request</span></span>
<span data-ttu-id="03151-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03151-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="03151-159">响应</span><span class="sxs-lookup"><span data-stu-id="03151-159">Response</span></span>
<span data-ttu-id="03151-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03151-160">Here is an example of the response.</span></span> 

><span data-ttu-id="03151-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03151-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
