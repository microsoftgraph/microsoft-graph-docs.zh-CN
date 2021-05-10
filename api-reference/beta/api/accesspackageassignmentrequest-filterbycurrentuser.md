---
title: accessPackageAssignmentRequest： filterByCurrentUser
description: 检索在已登录用户上筛选的 accesspackageassignmentrequest 对象列表。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d9e034f4ab2e95a487abf3a03e35bf78bd69ae9b
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299140"
---
# <a name="accesspackageassignmentrequest-filterbycurrentuser"></a><span data-ttu-id="5dc63-103">accessPackageAssignmentRequest： filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="5dc63-103">accessPackageAssignmentRequest: filterByCurrentUser</span></span>
<span data-ttu-id="5dc63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dc63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc63-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索在已登录用户上筛选的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="5dc63-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc63-106">权限</span><span class="sxs-lookup"><span data-stu-id="5dc63-106">Permissions</span></span>
<span data-ttu-id="5dc63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dc63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc63-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dc63-109">Permission type</span></span>|<span data-ttu-id="5dc63-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dc63-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dc63-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dc63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5dc63-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc63-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="5dc63-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dc63-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dc63-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dc63-114">Not supported.</span></span>|
|<span data-ttu-id="5dc63-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dc63-115">Application</span></span>|<span data-ttu-id="5dc63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dc63-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dc63-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dc63-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="5dc63-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="5dc63-118">Function parameters</span></span>
<span data-ttu-id="5dc63-119">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="5dc63-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5dc63-120">参数</span><span class="sxs-lookup"><span data-stu-id="5dc63-120">Parameter</span></span>|<span data-ttu-id="5dc63-121">类型</span><span class="sxs-lookup"><span data-stu-id="5dc63-121">Type</span></span>|<span data-ttu-id="5dc63-122">说明</span><span class="sxs-lookup"><span data-stu-id="5dc63-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc63-123">on</span><span class="sxs-lookup"><span data-stu-id="5dc63-123">on</span></span>|[<span data-ttu-id="5dc63-124">accessPackageAssignmentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="5dc63-124">accessPackageAssignmentRequestFilterByCurrentUserOptions</span></span>](../resources/accesspackageassignmentrequest-accesspackageassignmentrequestfilterbycurrentuseroptions.md)|<span data-ttu-id="5dc63-125">可用于对访问包分配请求列表进行筛选的当前用户选项的列表。</span><span class="sxs-lookup"><span data-stu-id="5dc63-125">The list of current user options that can be used to filter on the access package assignment requests list.</span></span>|

- <span data-ttu-id="5dc63-126">`target` 用于获取 `accessPackageAssignmentRequest` 已登录用户作为目标的对象。</span><span class="sxs-lookup"><span data-stu-id="5dc63-126">`target` is used to get the `accessPackageAssignmentRequest` objects where the signed-in user is the target.</span></span> <span data-ttu-id="5dc63-127">结果列表包括所有目录和访问包中调用方或调用方请求的所有分配请求（当前和已过期）。</span><span class="sxs-lookup"><span data-stu-id="5dc63-127">The resulting list includes all the assignment requests, current and expired, that were requested by the caller or for the caller, across all catalogs and access packages.</span></span>

- <span data-ttu-id="5dc63-128">`createdBy` 用于获取 `accessPackageAssignmentRequest` 已登录用户创建的对象。</span><span class="sxs-lookup"><span data-stu-id="5dc63-128">`createdBy` is used to get the `accessPackageAssignmentRequest` objects created by the signed-in user.</span></span> <span data-ttu-id="5dc63-129">结果列表包括所有目录和访问包中调用方自己或代表其他人创建的所有分配请求，例如管理员直接分配。</span><span class="sxs-lookup"><span data-stu-id="5dc63-129">The resulting list includes all of the assignment requests that the caller has created for themselves or on behalf of others, such as in case of admin direct assignment, across all catalogs and access packages.</span></span>

- <span data-ttu-id="5dc63-130">`approver` 用于获取已登录用户是任何包含的用户或用户中的允许审批 `accessPackageAssignmentRequest` `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` 者 `primaryApprovers` `escalationApprovers` () 。</span><span class="sxs-lookup"><span data-stu-id="5dc63-130">`approver` is used to get the `accessPackageAssignmentRequest` objects where the signed-in user is an allowed approver in any contained `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` (`primaryApprovers` or `escalationApprovers`).</span></span> <span data-ttu-id="5dc63-131">生成的列表包括所有目录和访问包中挂起且需要调用方做出决策的分配请求。</span><span class="sxs-lookup"><span data-stu-id="5dc63-131">The resulting list includes the assignment requests in *pending* state, across all catalogs and access packages and that need a decision from the caller.</span></span> <span data-ttu-id="5dc63-132">生成的列表包括状态中跨所有目录和访问包的分配请求，并且需要调用方 `pending` 做出决策。</span><span class="sxs-lookup"><span data-stu-id="5dc63-132">The resulting list includes the assignment requests in a `pending` state, across all catalogs and access packages and that need a decision from the caller.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dc63-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dc63-133">Request headers</span></span>
|<span data-ttu-id="5dc63-134">名称</span><span class="sxs-lookup"><span data-stu-id="5dc63-134">Name</span></span>|<span data-ttu-id="5dc63-135">说明</span><span class="sxs-lookup"><span data-stu-id="5dc63-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5dc63-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dc63-136">Authorization</span></span>|<span data-ttu-id="5dc63-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dc63-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc63-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dc63-139">Request body</span></span>
<span data-ttu-id="5dc63-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dc63-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dc63-141">响应</span><span class="sxs-lookup"><span data-stu-id="5dc63-141">Response</span></span>

<span data-ttu-id="5dc63-142">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5dc63-142">If successful, this method returns a `200 OK` response code and an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5dc63-143">示例</span><span class="sxs-lookup"><span data-stu-id="5dc63-143">Examples</span></span>

<span data-ttu-id="5dc63-144">以下示例获取针对已登录用户的访问包分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="5dc63-144">The following example gets the status of access package assignment requests targeted for the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="5dc63-145">请求</span><span class="sxs-lookup"><span data-stu-id="5dc63-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser(on='target')
```


### <a name="response"></a><span data-ttu-id="5dc63-146">响应</span><span class="sxs-lookup"><span data-stu-id="5dc63-146">Response</span></span>
> <span data-ttu-id="5dc63-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5dc63-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
            "createdDateTime": "2021-01-19T20:02:23.907Z",
            "completedDate": "2021-01-19T20:02:40.97Z",
            "id": "46c1410d-ef96-44c5-ae9c-a577d014fe0e",
            "requestType": "AdminAdd",
            "requestState": "Delivered",
            "requestStatus": "Fulfilled",
            "isValidationOnly": false,
            "expirationDateTime": null,
            "justification": null,
            "answers": [],
            "schedule": {
                "startDateTime": "2021-01-19T20:01:57.643Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": null,
                    "duration": null,
                    "type": "noExpiration"
                }
            }
        }
    ]
}
```

