---
title: 'privilegedRole: selfDeactivate'
description: 停用的角色分配给请求者。
ms.openlocfilehash: f9f72a4f61dfd154829406eb535b394f8f137069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042006"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="a846e-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="a846e-103">privilegedRole: selfDeactivate</span></span>

> <span data-ttu-id="a846e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a846e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a846e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a846e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a846e-106">停用的角色分配给请求者。</span><span class="sxs-lookup"><span data-stu-id="a846e-106">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="a846e-107">权限</span><span class="sxs-lookup"><span data-stu-id="a846e-107">Permissions</span></span>
<span data-ttu-id="a846e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a846e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a846e-110">请求者只能调用```selfDeactivate```角色分配给他。</span><span class="sxs-lookup"><span data-stu-id="a846e-110">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="a846e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a846e-111">Permission type</span></span>      | <span data-ttu-id="a846e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a846e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a846e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a846e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a846e-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a846e-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a846e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a846e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a846e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a846e-116">Not supported.</span></span>    |
|<span data-ttu-id="a846e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a846e-117">Application</span></span> | <span data-ttu-id="a846e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a846e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a846e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a846e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="a846e-120">请注意，``<id>``是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="a846e-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a846e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a846e-121">Request headers</span></span>
| <span data-ttu-id="a846e-122">名称</span><span class="sxs-lookup"><span data-stu-id="a846e-122">Name</span></span>       | <span data-ttu-id="a846e-123">说明</span><span class="sxs-lookup"><span data-stu-id="a846e-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a846e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a846e-124">Authorization</span></span>  | <span data-ttu-id="a846e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a846e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a846e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a846e-127">Request body</span></span>
<span data-ttu-id="a846e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a846e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a846e-129">响应</span><span class="sxs-lookup"><span data-stu-id="a846e-129">Response</span></span>

<span data-ttu-id="a846e-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a846e-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a846e-131">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="a846e-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a846e-132">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="a846e-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a846e-133">示例</span><span class="sxs-lookup"><span data-stu-id="a846e-133">Example</span></span>
<span data-ttu-id="a846e-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a846e-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a846e-135">请求</span><span class="sxs-lookup"><span data-stu-id="a846e-135">Request</span></span>
<span data-ttu-id="a846e-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a846e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="a846e-137">响应</span><span class="sxs-lookup"><span data-stu-id="a846e-137">Response</span></span>
<span data-ttu-id="a846e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a846e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->