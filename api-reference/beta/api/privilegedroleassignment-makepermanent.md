---
title: 'privilegedRoleAssignment: makePermanent'
description: 请为永久的角色分配。
localization_priority: Normal
ms.openlocfilehash: 9c6334662cf8496262b49b14ceb3f51f7a4f8dbc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511392"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="c84ad-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="c84ad-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c84ad-104">请为永久的角色分配。</span><span class="sxs-lookup"><span data-stu-id="c84ad-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="c84ad-105">权限</span><span class="sxs-lookup"><span data-stu-id="c84ad-105">Permissions</span></span>
<span data-ttu-id="c84ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c84ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c84ad-108">需要注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="c84ad-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c84ad-109">否则，将返回 HTTP 403 禁止访问错误。</span><span class="sxs-lookup"><span data-stu-id="c84ad-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="c84ad-110">请求者需要有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="c84ad-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="c84ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c84ad-111">Permission type</span></span>      | <span data-ttu-id="c84ad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c84ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c84ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c84ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c84ad-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c84ad-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c84ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c84ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c84ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c84ad-116">Not supported.</span></span>    |
|<span data-ttu-id="c84ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c84ad-117">Application</span></span> | <span data-ttu-id="c84ad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c84ad-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c84ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c84ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="c84ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c84ad-120">Request headers</span></span>
| <span data-ttu-id="c84ad-121">名称</span><span class="sxs-lookup"><span data-stu-id="c84ad-121">Name</span></span>       | <span data-ttu-id="c84ad-122">说明</span><span class="sxs-lookup"><span data-stu-id="c84ad-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c84ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c84ad-123">Authorization</span></span>  | <span data-ttu-id="c84ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c84ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c84ad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c84ad-126">Request body</span></span>
<span data-ttu-id="c84ad-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c84ad-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c84ad-128">参数</span><span class="sxs-lookup"><span data-stu-id="c84ad-128">Parameter</span></span>    | <span data-ttu-id="c84ad-129">类型</span><span class="sxs-lookup"><span data-stu-id="c84ad-129">Type</span></span>   |<span data-ttu-id="c84ad-130">说明</span><span class="sxs-lookup"><span data-stu-id="c84ad-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c84ad-131">原因</span><span class="sxs-lookup"><span data-stu-id="c84ad-131">reason</span></span>|<span data-ttu-id="c84ad-132">string</span><span class="sxs-lookup"><span data-stu-id="c84ad-132">string</span></span>|<span data-ttu-id="c84ad-133">可选。</span><span class="sxs-lookup"><span data-stu-id="c84ad-133">Optional.</span></span> <span data-ttu-id="c84ad-134">若要使此呼叫原因。</span><span class="sxs-lookup"><span data-stu-id="c84ad-134">The reason to make this call.</span></span>|
|<span data-ttu-id="c84ad-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="c84ad-135">ticketNumber</span></span>|<span data-ttu-id="c84ad-136">string</span><span class="sxs-lookup"><span data-stu-id="c84ad-136">string</span></span>|<span data-ttu-id="c84ad-137">可选。</span><span class="sxs-lookup"><span data-stu-id="c84ad-137">Optional.</span></span> <span data-ttu-id="c84ad-138">与此操作关联的票证数。</span><span class="sxs-lookup"><span data-stu-id="c84ad-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="c84ad-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="c84ad-139">ticketSystem</span></span>|<span data-ttu-id="c84ad-140">string</span><span class="sxs-lookup"><span data-stu-id="c84ad-140">string</span></span>|<span data-ttu-id="c84ad-141">可选。</span><span class="sxs-lookup"><span data-stu-id="c84ad-141">Optional.</span></span> <span data-ttu-id="c84ad-142">票证系统。</span><span class="sxs-lookup"><span data-stu-id="c84ad-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="c84ad-143">响应</span><span class="sxs-lookup"><span data-stu-id="c84ad-143">Response</span></span>

<span data-ttu-id="c84ad-144">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c84ad-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84ad-145">示例</span><span class="sxs-lookup"><span data-stu-id="c84ad-145">Example</span></span>
<span data-ttu-id="c84ad-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c84ad-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c84ad-147">请求</span><span class="sxs-lookup"><span data-stu-id="c84ad-147">Request</span></span>
<span data-ttu-id="c84ad-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c84ad-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c84ad-149">响应</span><span class="sxs-lookup"><span data-stu-id="c84ad-149">Response</span></span>
<span data-ttu-id="c84ad-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c84ad-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
