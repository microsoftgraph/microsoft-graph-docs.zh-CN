---
title: 'privilegedRoleAssignment: makePermanent'
description: 请为永久的角色分配。
ms.openlocfilehash: 06875fc62539598a5e1e806714fcae3d973ba29c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049162"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="b0268-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="b0268-103">privilegedRoleAssignment: makePermanent</span></span>

> <span data-ttu-id="b0268-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b0268-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0268-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b0268-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0268-106">请为永久的角色分配。</span><span class="sxs-lookup"><span data-stu-id="b0268-106">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0268-107">权限</span><span class="sxs-lookup"><span data-stu-id="b0268-107">Permissions</span></span>
<span data-ttu-id="b0268-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0268-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b0268-110">需要注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="b0268-110">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b0268-111">否则，将返回 HTTP 403 禁止访问错误。</span><span class="sxs-lookup"><span data-stu-id="b0268-111">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="b0268-112">请求者需要有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="b0268-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="b0268-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0268-113">Permission type</span></span>      | <span data-ttu-id="b0268-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0268-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0268-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0268-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b0268-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0268-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0268-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0268-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0268-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0268-118">Not supported.</span></span>    |
|<span data-ttu-id="b0268-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0268-119">Application</span></span> | <span data-ttu-id="b0268-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0268-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0268-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0268-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="b0268-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0268-122">Request headers</span></span>
| <span data-ttu-id="b0268-123">名称</span><span class="sxs-lookup"><span data-stu-id="b0268-123">Name</span></span>       | <span data-ttu-id="b0268-124">说明</span><span class="sxs-lookup"><span data-stu-id="b0268-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0268-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0268-125">Authorization</span></span>  | <span data-ttu-id="b0268-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0268-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0268-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0268-128">Request body</span></span>
<span data-ttu-id="b0268-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b0268-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b0268-130">参数</span><span class="sxs-lookup"><span data-stu-id="b0268-130">Parameter</span></span>    | <span data-ttu-id="b0268-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0268-131">Type</span></span>   |<span data-ttu-id="b0268-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0268-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0268-133">原因</span><span class="sxs-lookup"><span data-stu-id="b0268-133">reason</span></span>|<span data-ttu-id="b0268-134">string</span><span class="sxs-lookup"><span data-stu-id="b0268-134">string</span></span>|<span data-ttu-id="b0268-135">可选。</span><span class="sxs-lookup"><span data-stu-id="b0268-135">Optional.</span></span> <span data-ttu-id="b0268-136">若要使此呼叫原因。</span><span class="sxs-lookup"><span data-stu-id="b0268-136">The reason to make this call.</span></span>|
|<span data-ttu-id="b0268-137">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="b0268-137">ticketNumber</span></span>|<span data-ttu-id="b0268-138">string</span><span class="sxs-lookup"><span data-stu-id="b0268-138">string</span></span>|<span data-ttu-id="b0268-139">可选。</span><span class="sxs-lookup"><span data-stu-id="b0268-139">Optional.</span></span> <span data-ttu-id="b0268-140">与此操作关联的票证数。</span><span class="sxs-lookup"><span data-stu-id="b0268-140">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="b0268-141">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="b0268-141">ticketSystem</span></span>|<span data-ttu-id="b0268-142">string</span><span class="sxs-lookup"><span data-stu-id="b0268-142">string</span></span>|<span data-ttu-id="b0268-143">可选。</span><span class="sxs-lookup"><span data-stu-id="b0268-143">Optional.</span></span> <span data-ttu-id="b0268-144">票证系统。</span><span class="sxs-lookup"><span data-stu-id="b0268-144">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="b0268-145">响应</span><span class="sxs-lookup"><span data-stu-id="b0268-145">Response</span></span>

<span data-ttu-id="b0268-146">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0268-146">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0268-147">示例</span><span class="sxs-lookup"><span data-stu-id="b0268-147">Example</span></span>
<span data-ttu-id="b0268-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b0268-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0268-149">请求</span><span class="sxs-lookup"><span data-stu-id="b0268-149">Request</span></span>
<span data-ttu-id="b0268-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0268-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makepermanent"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makePermanent
Content-type: application/json
Content-length: 110

{
  "reason": "reason-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```

##### <a name="response"></a><span data-ttu-id="b0268-151">响应</span><span class="sxs-lookup"><span data-stu-id="b0268-151">Response</span></span>
<span data-ttu-id="b0268-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0268-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->