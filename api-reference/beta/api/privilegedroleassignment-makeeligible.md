---
title: 'privilegedRoleAssignment: makeEligible'
description: 使角色分配符合资格。 如果角色分配在呼叫之前已经有资格, 它将不执行任何操作。 如果角色分配是永久性的, 并且请求程序与目标用户不同, 则角色分配将变为符合条件, 并且将为目标用户停用该角色。 如果请求者是目标用户, 并且角色是安全管理员或特权角色管理员, 则将使用默认过期时间激活该角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d44cbbd682a02d5a8d89bbfe148f310c31b0313b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992078"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="ca110-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="ca110-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca110-107">使角色分配符合资格。</span><span class="sxs-lookup"><span data-stu-id="ca110-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="ca110-108">如果角色分配在呼叫之前已经有资格, 它将不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="ca110-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="ca110-109">如果角色分配是永久性的, 并且请求程序与目标用户不同, 则角色分配将变为符合条件, 并且将为目标用户停用该角色。</span><span class="sxs-lookup"><span data-stu-id="ca110-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="ca110-110">如果请求者是目标用户, 并且角色是安全管理员或特权角色管理员, 则将使用默认过期时间激活该角色。</span><span class="sxs-lookup"><span data-stu-id="ca110-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca110-111">权限</span><span class="sxs-lookup"><span data-stu-id="ca110-111">Permissions</span></span>
<span data-ttu-id="ca110-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca110-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ca110-114">请求者需要具有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="ca110-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="ca110-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca110-115">Permission type</span></span>      | <span data-ttu-id="ca110-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca110-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca110-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca110-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ca110-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca110-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca110-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca110-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca110-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca110-120">Not supported.</span></span>    |
|<span data-ttu-id="ca110-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca110-121">Application</span></span> | <span data-ttu-id="ca110-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca110-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca110-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca110-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="ca110-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca110-124">Request headers</span></span>
| <span data-ttu-id="ca110-125">名称</span><span class="sxs-lookup"><span data-stu-id="ca110-125">Name</span></span>       | <span data-ttu-id="ca110-126">说明</span><span class="sxs-lookup"><span data-stu-id="ca110-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca110-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca110-127">Authorization</span></span>  | <span data-ttu-id="ca110-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca110-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca110-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca110-130">Request body</span></span>
<span data-ttu-id="ca110-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca110-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca110-132">响应</span><span class="sxs-lookup"><span data-stu-id="ca110-132">Response</span></span>

<span data-ttu-id="ca110-133">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca110-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ca110-134">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="ca110-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ca110-135">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="ca110-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ca110-136">示例</span><span class="sxs-lookup"><span data-stu-id="ca110-136">Example</span></span>
<span data-ttu-id="ca110-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ca110-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ca110-138">请求</span><span class="sxs-lookup"><span data-stu-id="ca110-138">Request</span></span>
<span data-ttu-id="ca110-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca110-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ca110-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ca110-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca110-141">C#</span><span class="sxs-lookup"><span data-stu-id="ca110-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca110-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ca110-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca110-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="ca110-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ca110-144">Java</span><span class="sxs-lookup"><span data-stu-id="ca110-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makeeligible-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ca110-145">响应</span><span class="sxs-lookup"><span data-stu-id="ca110-145">Response</span></span>
<span data-ttu-id="ca110-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca110-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
