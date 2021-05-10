---
title: accessPackageAssignmentRequest：cancel
description: 取消处于可取消状态的访问PackageAssignmentRequest 对象。
localization_priority: Normal
author: sbounouh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5079de33f7ef3c7536baf50a876a84d5ca3711b4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299142"
---
# <a name="accesspackageassignmentrequest-cancel"></a><span data-ttu-id="b4848-103">accessPackageAssignmentRequest：cancel</span><span class="sxs-lookup"><span data-stu-id="b4848-103">accessPackageAssignmentRequest: cancel</span></span>
<span data-ttu-id="b4848-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4848-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4848-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，取消处于可取消状态（、）的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) `accepted` `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` 对象。</span><span class="sxs-lookup"><span data-stu-id="b4848-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4848-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4848-106">Permissions</span></span>
<span data-ttu-id="b4848-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4848-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4848-109">Permission type</span></span>|<span data-ttu-id="b4848-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4848-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4848-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4848-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4848-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4848-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="b4848-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4848-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4848-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4848-114">Not supported.</span></span>|
|<span data-ttu-id="b4848-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4848-115">Application</span></span>|<span data-ttu-id="b4848-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4848-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4848-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4848-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="b4848-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4848-118">Request headers</span></span>
|<span data-ttu-id="b4848-119">名称</span><span class="sxs-lookup"><span data-stu-id="b4848-119">Name</span></span>|<span data-ttu-id="b4848-120">说明</span><span class="sxs-lookup"><span data-stu-id="b4848-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4848-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4848-121">Authorization</span></span>|<span data-ttu-id="b4848-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4848-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4848-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4848-124">Request body</span></span>
<span data-ttu-id="b4848-125">在请求正文中，提供 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4848-125">In the request body, supply a JSON representation of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="b4848-126">对于取消自己的请求的非管理员用户，请求必须包含 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)的 **ID** 和值为 的 **requestStatus。** `cancelled`</span><span class="sxs-lookup"><span data-stu-id="b4848-126">For a non-administrator user to cancel their own request, the request must contain the **id** of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) and a **requestStatus** with a value of `cancelled`.</span></span>

## <a name="response"></a><span data-ttu-id="b4848-127">响应</span><span class="sxs-lookup"><span data-stu-id="b4848-127">Response</span></span>

<span data-ttu-id="b4848-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b4848-128">If successful, this method returns a `200 OK` response code.</span></span>  <span data-ttu-id="b4848-129">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4848-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4848-130">示例</span><span class="sxs-lookup"><span data-stu-id="b4848-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4848-131">请求</span><span class="sxs-lookup"><span data-stu-id="b4848-131">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="b4848-132">响应</span><span class="sxs-lookup"><span data-stu-id="b4848-132">Response</span></span>
<span data-ttu-id="b4848-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4848-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

