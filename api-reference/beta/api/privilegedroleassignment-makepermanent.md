---
title: privilegedRoleAssignment：makePermanent
description: 使角色分配永久。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a66834f5937b8dea55391553536670ff06ae83c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037373"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="6d4be-103">privilegedRoleAssignment：makePermanent</span><span class="sxs-lookup"><span data-stu-id="6d4be-103">privilegedRoleAssignment: makePermanent</span></span>

<span data-ttu-id="6d4be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d4be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d4be-105">使角色分配永久。</span><span class="sxs-lookup"><span data-stu-id="6d4be-105">Make the role assignment permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d4be-106">权限</span><span class="sxs-lookup"><span data-stu-id="6d4be-106">Permissions</span></span>
<span data-ttu-id="6d4be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d4be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6d4be-109">租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="6d4be-109">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6d4be-110">否则，将返回 HTTP 403 禁止错误。</span><span class="sxs-lookup"><span data-stu-id="6d4be-110">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="6d4be-111">请求者需要具有 _Privileged Role Administrator_ 角色。</span><span class="sxs-lookup"><span data-stu-id="6d4be-111">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="6d4be-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d4be-112">Permission type</span></span>      | <span data-ttu-id="6d4be-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d4be-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d4be-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d4be-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6d4be-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d4be-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d4be-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d4be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d4be-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d4be-117">Not supported.</span></span>    |
|<span data-ttu-id="6d4be-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d4be-118">Application</span></span> | <span data-ttu-id="6d4be-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d4be-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d4be-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d4be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="6d4be-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d4be-121">Request headers</span></span>
| <span data-ttu-id="6d4be-122">名称</span><span class="sxs-lookup"><span data-stu-id="6d4be-122">Name</span></span>       | <span data-ttu-id="6d4be-123">说明</span><span class="sxs-lookup"><span data-stu-id="6d4be-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d4be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d4be-124">Authorization</span></span>  | <span data-ttu-id="6d4be-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d4be-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d4be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d4be-127">Request body</span></span>
<span data-ttu-id="6d4be-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6d4be-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6d4be-129">参数</span><span class="sxs-lookup"><span data-stu-id="6d4be-129">Parameter</span></span>    | <span data-ttu-id="6d4be-130">类型</span><span class="sxs-lookup"><span data-stu-id="6d4be-130">Type</span></span>   |<span data-ttu-id="6d4be-131">说明</span><span class="sxs-lookup"><span data-stu-id="6d4be-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d4be-132">reason</span><span class="sxs-lookup"><span data-stu-id="6d4be-132">reason</span></span>|<span data-ttu-id="6d4be-133">string</span><span class="sxs-lookup"><span data-stu-id="6d4be-133">string</span></span>|<span data-ttu-id="6d4be-134">可选。</span><span class="sxs-lookup"><span data-stu-id="6d4be-134">Optional.</span></span> <span data-ttu-id="6d4be-135">进行此调用的原因。</span><span class="sxs-lookup"><span data-stu-id="6d4be-135">The reason to make this call.</span></span>|
|<span data-ttu-id="6d4be-136">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="6d4be-136">ticketNumber</span></span>|<span data-ttu-id="6d4be-137">string</span><span class="sxs-lookup"><span data-stu-id="6d4be-137">string</span></span>|<span data-ttu-id="6d4be-138">可选。</span><span class="sxs-lookup"><span data-stu-id="6d4be-138">Optional.</span></span> <span data-ttu-id="6d4be-139">与此操作关联的票证编号。</span><span class="sxs-lookup"><span data-stu-id="6d4be-139">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="6d4be-140">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="6d4be-140">ticketSystem</span></span>|<span data-ttu-id="6d4be-141">string</span><span class="sxs-lookup"><span data-stu-id="6d4be-141">string</span></span>|<span data-ttu-id="6d4be-142">可选。</span><span class="sxs-lookup"><span data-stu-id="6d4be-142">Optional.</span></span> <span data-ttu-id="6d4be-143">票证系统。</span><span class="sxs-lookup"><span data-stu-id="6d4be-143">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="6d4be-144">响应</span><span class="sxs-lookup"><span data-stu-id="6d4be-144">Response</span></span>

<span data-ttu-id="6d4be-145">如果成功，此方法在 `200 OK` 响应正文中返回 [响应代码和 privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d4be-145">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d4be-146">示例</span><span class="sxs-lookup"><span data-stu-id="6d4be-146">Example</span></span>
<span data-ttu-id="6d4be-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6d4be-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6d4be-148">请求</span><span class="sxs-lookup"><span data-stu-id="6d4be-148">Request</span></span>
<span data-ttu-id="6d4be-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d4be-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d4be-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d4be-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6d4be-151">C#</span><span class="sxs-lookup"><span data-stu-id="6d4be-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d4be-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d4be-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d4be-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d4be-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d4be-154">Java</span><span class="sxs-lookup"><span data-stu-id="6d4be-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d4be-155">响应</span><span class="sxs-lookup"><span data-stu-id="6d4be-155">Response</span></span>
<span data-ttu-id="6d4be-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6d4be-156">Here is an example of the response.</span></span> <span data-ttu-id="6d4be-157">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6d4be-157">Note: The response object shown here might be shortened for readability.</span></span>
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


