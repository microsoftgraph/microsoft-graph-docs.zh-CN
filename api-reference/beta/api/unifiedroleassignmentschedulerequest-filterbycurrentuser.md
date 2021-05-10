---
title: unifiedRoleAssignmentScheduleRequest： filterByCurrentUser
description: 获取由特定用户主体筛选的 unifiedRoleAssignmentScheduleRequest 对象及其属性的列表
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f03402cc6ebffa18ec1a5bf91df095d76f6e6a9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299217"
---
# <a name="unifiedroleassignmentschedulerequest-filterbycurrentuser"></a><span data-ttu-id="66b56-103">unifiedRoleAssignmentScheduleRequest： filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="66b56-103">unifiedRoleAssignmentScheduleRequest: filterByCurrentUser</span></span>
<span data-ttu-id="66b56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66b56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="66b56-105">获取与特定主体对象关联的 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="66b56-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66b56-106">权限</span><span class="sxs-lookup"><span data-stu-id="66b56-106">Permissions</span></span>
<span data-ttu-id="66b56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66b56-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66b56-109">Permission type</span></span>|<span data-ttu-id="66b56-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66b56-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66b56-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66b56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66b56-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="66b56-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="66b56-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66b56-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66b56-114">不支持</span><span class="sxs-lookup"><span data-stu-id="66b56-114">Not supported</span></span>|
|<span data-ttu-id="66b56-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66b56-115">Application</span></span>|<span data-ttu-id="66b56-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="66b56-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="66b56-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66b56-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="66b56-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="66b56-118">Query parameters</span></span>
<span data-ttu-id="66b56-119">下表显示了可用于此方法的查询参数。</span><span class="sxs-lookup"><span data-stu-id="66b56-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="66b56-120">参数</span><span class="sxs-lookup"><span data-stu-id="66b56-120">Parameter</span></span>|<span data-ttu-id="66b56-121">类型</span><span class="sxs-lookup"><span data-stu-id="66b56-121">Type</span></span>|<span data-ttu-id="66b56-122">说明</span><span class="sxs-lookup"><span data-stu-id="66b56-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b56-123">on</span><span class="sxs-lookup"><span data-stu-id="66b56-123">on</span></span>|<span data-ttu-id="66b56-124">RoleAssignmentScheduleRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="66b56-124">RoleAssignmentScheduleRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="66b56-125">主体对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="66b56-125">Id of the principal object.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="66b56-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="66b56-126">Request headers</span></span>
|<span data-ttu-id="66b56-127">名称</span><span class="sxs-lookup"><span data-stu-id="66b56-127">Name</span></span>|<span data-ttu-id="66b56-128">说明</span><span class="sxs-lookup"><span data-stu-id="66b56-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="66b56-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="66b56-129">Authorization</span></span>|<span data-ttu-id="66b56-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66b56-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66b56-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="66b56-132">Request body</span></span>
<span data-ttu-id="66b56-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66b56-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66b56-134">响应</span><span class="sxs-lookup"><span data-stu-id="66b56-134">Response</span></span>

<span data-ttu-id="66b56-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="66b56-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66b56-136">示例</span><span class="sxs-lookup"><span data-stu-id="66b56-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66b56-137">请求</span><span class="sxs-lookup"><span data-stu-id="66b56-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleAssignmentScheduleRequests/filterByCurrentUser(on='d6e4112f-112f-d6e4-2f11-e4d62f11e4d6')
```


### <a name="response"></a><span data-ttu-id="66b56-138">响应</span><span class="sxs-lookup"><span data-stu-id="66b56-138">Response</span></span>
<span data-ttu-id="66b56-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66b56-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "action": "AdminAssign",
      "principalId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "roleDefinitionId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "directoryScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "appScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "isValidationOnly": false,
      "targetScheduleId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "justification": "this is a justification",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```

