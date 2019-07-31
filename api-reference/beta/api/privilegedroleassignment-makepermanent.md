---
title: 'privilegedRoleAssignment: makePermanent'
description: 将角色分配标记为永久。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: aa0ac75a74b7bba089b40826e4709f2c557f632e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978769"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="4abed-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="4abed-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4abed-104">将角色分配标记为永久。</span><span class="sxs-lookup"><span data-stu-id="4abed-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="4abed-105">权限</span><span class="sxs-lookup"><span data-stu-id="4abed-105">Permissions</span></span>
<span data-ttu-id="4abed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4abed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4abed-108">需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="4abed-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4abed-109">否则, 将返回 HTTP 403 禁止错误。</span><span class="sxs-lookup"><span data-stu-id="4abed-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="4abed-110">请求者需要具有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="4abed-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="4abed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4abed-111">Permission type</span></span>      | <span data-ttu-id="4abed-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4abed-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4abed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4abed-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4abed-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4abed-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4abed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4abed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4abed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4abed-116">Not supported.</span></span>    |
|<span data-ttu-id="4abed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4abed-117">Application</span></span> | <span data-ttu-id="4abed-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4abed-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4abed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4abed-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="4abed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4abed-120">Request headers</span></span>
| <span data-ttu-id="4abed-121">名称</span><span class="sxs-lookup"><span data-stu-id="4abed-121">Name</span></span>       | <span data-ttu-id="4abed-122">说明</span><span class="sxs-lookup"><span data-stu-id="4abed-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4abed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4abed-123">Authorization</span></span>  | <span data-ttu-id="4abed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4abed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4abed-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4abed-126">Request body</span></span>
<span data-ttu-id="4abed-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4abed-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4abed-128">参数</span><span class="sxs-lookup"><span data-stu-id="4abed-128">Parameter</span></span>    | <span data-ttu-id="4abed-129">类型</span><span class="sxs-lookup"><span data-stu-id="4abed-129">Type</span></span>   |<span data-ttu-id="4abed-130">说明</span><span class="sxs-lookup"><span data-stu-id="4abed-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4abed-131">在于</span><span class="sxs-lookup"><span data-stu-id="4abed-131">reason</span></span>|<span data-ttu-id="4abed-132">字符串</span><span class="sxs-lookup"><span data-stu-id="4abed-132">string</span></span>|<span data-ttu-id="4abed-133">可选。</span><span class="sxs-lookup"><span data-stu-id="4abed-133">Optional.</span></span> <span data-ttu-id="4abed-134">执行此调用的原因。</span><span class="sxs-lookup"><span data-stu-id="4abed-134">The reason to make this call.</span></span>|
|<span data-ttu-id="4abed-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="4abed-135">ticketNumber</span></span>|<span data-ttu-id="4abed-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4abed-136">string</span></span>|<span data-ttu-id="4abed-137">可选。</span><span class="sxs-lookup"><span data-stu-id="4abed-137">Optional.</span></span> <span data-ttu-id="4abed-138">与此操作相关联的票证编号。</span><span class="sxs-lookup"><span data-stu-id="4abed-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="4abed-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="4abed-139">ticketSystem</span></span>|<span data-ttu-id="4abed-140">字符串</span><span class="sxs-lookup"><span data-stu-id="4abed-140">string</span></span>|<span data-ttu-id="4abed-141">可选。</span><span class="sxs-lookup"><span data-stu-id="4abed-141">Optional.</span></span> <span data-ttu-id="4abed-142">票证系统。</span><span class="sxs-lookup"><span data-stu-id="4abed-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="4abed-143">响应</span><span class="sxs-lookup"><span data-stu-id="4abed-143">Response</span></span>

<span data-ttu-id="4abed-144">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4abed-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4abed-145">示例</span><span class="sxs-lookup"><span data-stu-id="4abed-145">Example</span></span>
<span data-ttu-id="4abed-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4abed-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4abed-147">请求</span><span class="sxs-lookup"><span data-stu-id="4abed-147">Request</span></span>
<span data-ttu-id="4abed-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4abed-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4abed-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4abed-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4abed-150">C#</span><span class="sxs-lookup"><span data-stu-id="4abed-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4abed-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="4abed-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4abed-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="4abed-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4abed-153">Java</span><span class="sxs-lookup"><span data-stu-id="4abed-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4abed-154">响应</span><span class="sxs-lookup"><span data-stu-id="4abed-154">Response</span></span>
<span data-ttu-id="4abed-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4abed-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
