---
title: 'privilegedRoleAssignment: makeEligible'
description: 使角色分配符合资格。 如果角色分配在呼叫之前已经有资格, 它将不执行任何操作。 如果角色分配是永久性的, 并且请求程序与目标用户不同, 则角色分配将变为符合条件, 并且将为目标用户停用该角色。 如果请求者是目标用户, 并且角色是安全管理员或特权角色管理员, 则将使用默认过期时间激活该角色。
localization_priority: Normal
ms.openlocfilehash: 6d3e6e58119a7a757da65d08eeeb97247a78d714
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337143"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="df454-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="df454-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df454-107">使角色分配符合资格。</span><span class="sxs-lookup"><span data-stu-id="df454-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="df454-108">如果角色分配在呼叫之前已经有资格, 它将不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="df454-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="df454-109">如果角色分配是永久性的, 并且请求程序与目标用户不同, 则角色分配将变为符合条件, 并且将为目标用户停用该角色。</span><span class="sxs-lookup"><span data-stu-id="df454-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="df454-110">如果请求者是目标用户, 并且角色是安全管理员或特权角色管理员, 则将使用默认过期时间激活该角色。</span><span class="sxs-lookup"><span data-stu-id="df454-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="df454-111">权限</span><span class="sxs-lookup"><span data-stu-id="df454-111">Permissions</span></span>
<span data-ttu-id="df454-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df454-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="df454-114">请求者需要具有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="df454-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="df454-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="df454-115">Permission type</span></span>      | <span data-ttu-id="df454-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df454-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df454-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df454-117">Delegated (work or school account)</span></span> | <span data-ttu-id="df454-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df454-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df454-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df454-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df454-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="df454-120">Not supported.</span></span>    |
|<span data-ttu-id="df454-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="df454-121">Application</span></span> | <span data-ttu-id="df454-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="df454-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df454-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df454-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="df454-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="df454-124">Request headers</span></span>
| <span data-ttu-id="df454-125">名称</span><span class="sxs-lookup"><span data-stu-id="df454-125">Name</span></span>       | <span data-ttu-id="df454-126">说明</span><span class="sxs-lookup"><span data-stu-id="df454-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df454-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="df454-127">Authorization</span></span>  | <span data-ttu-id="df454-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df454-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df454-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="df454-130">Request body</span></span>
<span data-ttu-id="df454-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df454-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df454-132">响应</span><span class="sxs-lookup"><span data-stu-id="df454-132">Response</span></span>

<span data-ttu-id="df454-133">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df454-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="df454-134">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="df454-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="df454-135">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="df454-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="df454-136">示例</span><span class="sxs-lookup"><span data-stu-id="df454-136">Example</span></span>
<span data-ttu-id="df454-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="df454-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="df454-138">请求</span><span class="sxs-lookup"><span data-stu-id="df454-138">Request</span></span>
<span data-ttu-id="df454-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df454-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="df454-140">响应</span><span class="sxs-lookup"><span data-stu-id="df454-140">Response</span></span>
<span data-ttu-id="df454-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df454-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
