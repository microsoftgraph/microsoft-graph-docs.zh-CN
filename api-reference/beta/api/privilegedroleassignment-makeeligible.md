---
title: privilegedRoleAssignment：makeEligible
description: 使角色分配合格。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 14777dc2e680e4345ec4e1f3b32944d317b812cd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441212"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="b7b02-103">privilegedRoleAssignment：makeEligible</span><span class="sxs-lookup"><span data-stu-id="b7b02-103">privilegedRoleAssignment: makeEligible</span></span>

<span data-ttu-id="b7b02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b02-105">使角色分配合格。</span><span class="sxs-lookup"><span data-stu-id="b7b02-105">Make the role assignment eligible.</span></span> <span data-ttu-id="b7b02-106">如果角色分配在调用之前已符合条件，则不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="b7b02-106">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="b7b02-107">如果角色分配是永久性的，并且请求者与目标用户不同，角色分配将变为合格状态，并且该角色将停用目标用户。</span><span class="sxs-lookup"><span data-stu-id="b7b02-107">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="b7b02-108">如果请求者是目标用户，并且该角色是安全管理员或特权角色管理员，则角色将在默认过期后激活。</span><span class="sxs-lookup"><span data-stu-id="b7b02-108">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7b02-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b7b02-109">Permissions</span></span>
<span data-ttu-id="b7b02-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7b02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b7b02-112">请求者需要具有 _Privileged Role Administrator_ 角色。</span><span class="sxs-lookup"><span data-stu-id="b7b02-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="b7b02-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7b02-113">Permission type</span></span>      | <span data-ttu-id="b7b02-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7b02-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7b02-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b02-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b7b02-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7b02-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7b02-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b02-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7b02-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7b02-118">Not supported.</span></span>    |
|<span data-ttu-id="b7b02-119">Application</span><span class="sxs-lookup"><span data-stu-id="b7b02-119">Application</span></span> | <span data-ttu-id="b7b02-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7b02-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7b02-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7b02-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="b7b02-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7b02-122">Request headers</span></span>
| <span data-ttu-id="b7b02-123">名称</span><span class="sxs-lookup"><span data-stu-id="b7b02-123">Name</span></span>       | <span data-ttu-id="b7b02-124">说明</span><span class="sxs-lookup"><span data-stu-id="b7b02-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7b02-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7b02-125">Authorization</span></span>  | <span data-ttu-id="b7b02-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7b02-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7b02-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7b02-128">Request body</span></span>
<span data-ttu-id="b7b02-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7b02-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7b02-130">响应</span><span class="sxs-lookup"><span data-stu-id="b7b02-130">Response</span></span>

<span data-ttu-id="b7b02-131">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7b02-131">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="b7b02-132">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="b7b02-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b7b02-133">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="b7b02-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b7b02-134">示例</span><span class="sxs-lookup"><span data-stu-id="b7b02-134">Example</span></span>
<span data-ttu-id="b7b02-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b7b02-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7b02-136">请求</span><span class="sxs-lookup"><span data-stu-id="b7b02-136">Request</span></span>
<span data-ttu-id="b7b02-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7b02-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7b02-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b02-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="c"></a>[<span data-ttu-id="b7b02-139">C#</span><span class="sxs-lookup"><span data-stu-id="b7b02-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7b02-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7b02-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7b02-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7b02-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7b02-142">Java</span><span class="sxs-lookup"><span data-stu-id="b7b02-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makeeligible-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b7b02-143">响应</span><span class="sxs-lookup"><span data-stu-id="b7b02-143">Response</span></span>
<span data-ttu-id="b7b02-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7b02-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


