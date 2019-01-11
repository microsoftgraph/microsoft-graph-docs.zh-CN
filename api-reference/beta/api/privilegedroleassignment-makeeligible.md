---
title: 'privilegedRoleAssignment: makeEligible'
description: 请作为合格的角色分配。 如果角色分配已合格呼叫之前，它无实际作用。 如果是永久性的角色分配，请求者是不同于目标用户的角色分配将成为合格和角色将被停用的目标用户。 如果请求程序是目标用户和角色是安全管理员或具有权限的角色管理员，将默认过期激活角色。
localization_priority: Normal
ms.openlocfilehash: 90f606ed1550f6341251e5185e620c29838a9ac9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822587"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="8362f-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="8362f-106">privilegedRoleAssignment: makeEligible</span></span>

> <span data-ttu-id="8362f-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8362f-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8362f-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8362f-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8362f-109">请作为合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="8362f-109">Make the role assignment as eligible.</span></span> <span data-ttu-id="8362f-110">如果角色分配已合格呼叫之前，它无实际作用。</span><span class="sxs-lookup"><span data-stu-id="8362f-110">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="8362f-111">如果是永久性的角色分配，请求者是不同于目标用户的角色分配将成为合格和角色将被停用的目标用户。</span><span class="sxs-lookup"><span data-stu-id="8362f-111">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="8362f-112">如果请求程序是目标用户和角色是安全管理员或具有权限的角色管理员，将默认过期激活角色。</span><span class="sxs-lookup"><span data-stu-id="8362f-112">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="8362f-113">权限</span><span class="sxs-lookup"><span data-stu-id="8362f-113">Permissions</span></span>
<span data-ttu-id="8362f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8362f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8362f-116">请求者需要有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="8362f-116">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="8362f-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="8362f-117">Permission type</span></span>      | <span data-ttu-id="8362f-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8362f-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8362f-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8362f-119">Delegated (work or school account)</span></span> | <span data-ttu-id="8362f-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8362f-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8362f-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8362f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8362f-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="8362f-122">Not supported.</span></span>    |
|<span data-ttu-id="8362f-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="8362f-123">Application</span></span> | <span data-ttu-id="8362f-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="8362f-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8362f-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8362f-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="8362f-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8362f-126">Request headers</span></span>
| <span data-ttu-id="8362f-127">名称</span><span class="sxs-lookup"><span data-stu-id="8362f-127">Name</span></span>       | <span data-ttu-id="8362f-128">说明</span><span class="sxs-lookup"><span data-stu-id="8362f-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8362f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8362f-129">Authorization</span></span>  | <span data-ttu-id="8362f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8362f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8362f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="8362f-132">Request body</span></span>
<span data-ttu-id="8362f-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8362f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8362f-134">响应</span><span class="sxs-lookup"><span data-stu-id="8362f-134">Response</span></span>

<span data-ttu-id="8362f-135">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8362f-135">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="8362f-136">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="8362f-136">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8362f-137">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="8362f-137">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8362f-138">示例</span><span class="sxs-lookup"><span data-stu-id="8362f-138">Example</span></span>
<span data-ttu-id="8362f-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8362f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8362f-140">请求</span><span class="sxs-lookup"><span data-stu-id="8362f-140">Request</span></span>
<span data-ttu-id="8362f-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8362f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="8362f-142">响应</span><span class="sxs-lookup"><span data-stu-id="8362f-142">Response</span></span>
<span data-ttu-id="8362f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8362f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
