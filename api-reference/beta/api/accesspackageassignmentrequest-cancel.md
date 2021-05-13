---
title: accessPackageAssignmentRequest：cancel
description: 取消处于可取消状态的访问PackageAssignmentRequest 对象。
localization_priority: Normal
author: sbounouh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d32f7e21bf8bf618b762f2a39b9fdd92eac102d0
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473976"
---
# <a name="accesspackageassignmentrequest-cancel"></a><span data-ttu-id="f0897-103">accessPackageAssignmentRequest：cancel</span><span class="sxs-lookup"><span data-stu-id="f0897-103">accessPackageAssignmentRequest: cancel</span></span>
<span data-ttu-id="f0897-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0897-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，取消处于可取消状态（、）的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) `accepted` `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` 对象。</span><span class="sxs-lookup"><span data-stu-id="f0897-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0897-106">权限</span><span class="sxs-lookup"><span data-stu-id="f0897-106">Permissions</span></span>
<span data-ttu-id="f0897-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0897-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0897-109">Permission type</span></span>|<span data-ttu-id="f0897-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0897-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0897-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0897-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0897-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0897-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="f0897-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0897-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0897-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0897-114">Not supported.</span></span>|
|<span data-ttu-id="f0897-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0897-115">Application</span></span>|<span data-ttu-id="f0897-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0897-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0897-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0897-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="f0897-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0897-118">Request headers</span></span>
|<span data-ttu-id="f0897-119">名称</span><span class="sxs-lookup"><span data-stu-id="f0897-119">Name</span></span>|<span data-ttu-id="f0897-120">说明</span><span class="sxs-lookup"><span data-stu-id="f0897-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f0897-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0897-121">Authorization</span></span>|<span data-ttu-id="f0897-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0897-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0897-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0897-124">Request body</span></span>
<span data-ttu-id="f0897-125">在请求正文中，提供 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0897-125">In the request body, supply a JSON representation of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="f0897-126">对于取消自己的请求的非管理员用户，请求必须包含 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)的 **ID** 和值为 的 **requestStatus。** `cancelled`</span><span class="sxs-lookup"><span data-stu-id="f0897-126">For a non-administrator user to cancel their own request, the request must contain the **id** of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) and a **requestStatus** with a value of `cancelled`.</span></span>

## <a name="response"></a><span data-ttu-id="f0897-127">响应</span><span class="sxs-lookup"><span data-stu-id="f0897-127">Response</span></span>

<span data-ttu-id="f0897-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f0897-128">If successful, this method returns a `200 OK` response code.</span></span>  <span data-ttu-id="f0897-129">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f0897-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0897-130">示例</span><span class="sxs-lookup"><span data-stu-id="f0897-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0897-131">请求</span><span class="sxs-lookup"><span data-stu-id="f0897-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f0897-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0897-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel

{
  "id":"request-id",
  "requestStatus":"cancelled"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f0897-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0897-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0897-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0897-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f0897-135">响应</span><span class="sxs-lookup"><span data-stu-id="f0897-135">Response</span></span>
<span data-ttu-id="f0897-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0897-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

