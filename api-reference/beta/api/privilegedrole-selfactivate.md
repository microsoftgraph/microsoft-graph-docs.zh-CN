---
title: 'privilegedRole: selfActivate'
description: 激活分配给请求者角色。
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515067"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="a5147-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="a5147-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5147-104">激活分配给请求者角色。</span><span class="sxs-lookup"><span data-stu-id="a5147-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="a5147-105">**注意：** 有效年 12 月 2018年此 API 将不再支持和不应使用。</span><span class="sxs-lookup"><span data-stu-id="a5147-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="a5147-106">请改用[创建 PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) 。</span><span class="sxs-lookup"><span data-stu-id="a5147-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="a5147-107">权限</span><span class="sxs-lookup"><span data-stu-id="a5147-107">Permissions</span></span>
<span data-ttu-id="a5147-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5147-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a5147-110">请求者只能调用```selfActivate```角色分配给他。</span><span class="sxs-lookup"><span data-stu-id="a5147-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="a5147-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5147-111">Permission type</span></span>      | <span data-ttu-id="a5147-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5147-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5147-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5147-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a5147-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5147-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5147-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5147-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5147-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5147-116">Not supported.</span></span>    |
|<span data-ttu-id="a5147-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5147-117">Application</span></span> | <span data-ttu-id="a5147-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5147-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5147-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5147-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="a5147-120">请注意，``<id>``是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="a5147-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5147-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5147-121">Request headers</span></span>
| <span data-ttu-id="a5147-122">名称</span><span class="sxs-lookup"><span data-stu-id="a5147-122">Name</span></span>       | <span data-ttu-id="a5147-123">说明</span><span class="sxs-lookup"><span data-stu-id="a5147-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a5147-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5147-124">Authorization</span></span>  | <span data-ttu-id="a5147-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5147-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5147-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5147-127">Request body</span></span>
<span data-ttu-id="a5147-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a5147-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a5147-129">参数</span><span class="sxs-lookup"><span data-stu-id="a5147-129">Parameter</span></span>    | <span data-ttu-id="a5147-130">类型</span><span class="sxs-lookup"><span data-stu-id="a5147-130">Type</span></span>   |<span data-ttu-id="a5147-131">说明</span><span class="sxs-lookup"><span data-stu-id="a5147-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5147-132">原因</span><span class="sxs-lookup"><span data-stu-id="a5147-132">reason</span></span>|<span data-ttu-id="a5147-133">string</span><span class="sxs-lookup"><span data-stu-id="a5147-133">string</span></span>|<span data-ttu-id="a5147-134">可选。</span><span class="sxs-lookup"><span data-stu-id="a5147-134">Optional.</span></span> <span data-ttu-id="a5147-135">有关此角色激活的原因的说明。</span><span class="sxs-lookup"><span data-stu-id="a5147-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="a5147-136">duration</span><span class="sxs-lookup"><span data-stu-id="a5147-136">duration</span></span>|<span data-ttu-id="a5147-137">string</span><span class="sxs-lookup"><span data-stu-id="a5147-137">string</span></span>|<span data-ttu-id="a5147-138">可选。</span><span class="sxs-lookup"><span data-stu-id="a5147-138">Optional.</span></span> <span data-ttu-id="a5147-139">有效的值可以是```min```（最少激活持续时间） ```default``` （默认激活持续时间的角色），或可指定小时数，则激活一个 double 值。</span><span class="sxs-lookup"><span data-stu-id="a5147-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="a5147-140">指定的持续时间不能超过从角色设置的角色激活持续时间。</span><span class="sxs-lookup"><span data-stu-id="a5147-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="a5147-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="a5147-141">ticketNumber</span></span>|<span data-ttu-id="a5147-142">string</span><span class="sxs-lookup"><span data-stu-id="a5147-142">string</span></span>|<span data-ttu-id="a5147-143">可选。</span><span class="sxs-lookup"><span data-stu-id="a5147-143">Optional.</span></span> <span data-ttu-id="a5147-144">用于跟踪此角色激活票证数量。</span><span class="sxs-lookup"><span data-stu-id="a5147-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="a5147-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="a5147-145">ticketSystem</span></span>|<span data-ttu-id="a5147-146">string</span><span class="sxs-lookup"><span data-stu-id="a5147-146">string</span></span>|<span data-ttu-id="a5147-147">可选。</span><span class="sxs-lookup"><span data-stu-id="a5147-147">Optional.</span></span> <span data-ttu-id="a5147-148">票证系统。</span><span class="sxs-lookup"><span data-stu-id="a5147-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="a5147-149">响应</span><span class="sxs-lookup"><span data-stu-id="a5147-149">Response</span></span>

<span data-ttu-id="a5147-150">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a5147-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a5147-151">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="a5147-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a5147-152">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="a5147-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a5147-153">示例</span><span class="sxs-lookup"><span data-stu-id="a5147-153">Example</span></span>
<span data-ttu-id="a5147-154">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a5147-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a5147-155">请求</span><span class="sxs-lookup"><span data-stu-id="a5147-155">Request</span></span>
<span data-ttu-id="a5147-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5147-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a5147-157">响应</span><span class="sxs-lookup"><span data-stu-id="a5147-157">Response</span></span>
<span data-ttu-id="a5147-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a5147-158">Here is an example of the response.</span></span> 

><span data-ttu-id="a5147-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a5147-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
