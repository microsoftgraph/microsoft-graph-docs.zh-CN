---
title: unifiedRoleAssignmentSchedule：filterByCurrentUser
description: 获取 unifiedRoleAssignmentSchedule 对象及其属性的列表，这些对象按特定用户主体进行筛选
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2ec3668023e3fcda0e402d07ba64dea957720675
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679860"
---
# <a name="unifiedroleassignmentschedule-filterbycurrentuser"></a><span data-ttu-id="01d35-103">unifiedRoleAssignmentSchedule：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="01d35-103">unifiedRoleAssignmentSchedule: filterByCurrentUser</span></span>
<span data-ttu-id="01d35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01d35-105">获取与特定主体对象关联的 [unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="01d35-105">Get a list of the [unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="01d35-106">权限</span><span class="sxs-lookup"><span data-stu-id="01d35-106">Permissions</span></span>
<span data-ttu-id="01d35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01d35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d35-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="01d35-109">Permission type</span></span>|<span data-ttu-id="01d35-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01d35-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d35-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01d35-111">Delegated (work or school account)</span></span>|<span data-ttu-id="01d35-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="01d35-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="01d35-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01d35-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d35-114">不支持</span><span class="sxs-lookup"><span data-stu-id="01d35-114">Not supported</span></span>|
|<span data-ttu-id="01d35-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="01d35-115">Application</span></span>|<span data-ttu-id="01d35-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="01d35-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d35-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01d35-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="01d35-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="01d35-118">Query parameters</span></span>
<span data-ttu-id="01d35-119">下表显示了可用于此方法的查询参数。</span><span class="sxs-lookup"><span data-stu-id="01d35-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="01d35-120">参数</span><span class="sxs-lookup"><span data-stu-id="01d35-120">Parameter</span></span>|<span data-ttu-id="01d35-121">类型</span><span class="sxs-lookup"><span data-stu-id="01d35-121">Type</span></span>|<span data-ttu-id="01d35-122">说明</span><span class="sxs-lookup"><span data-stu-id="01d35-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d35-123">on</span><span class="sxs-lookup"><span data-stu-id="01d35-123">on</span></span>|<span data-ttu-id="01d35-124">roleAssignmentScheduleFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="01d35-124">roleAssignmentScheduleFilterByCurrentUserOptions</span></span>|<span data-ttu-id="01d35-125">当前用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="01d35-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="01d35-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="01d35-126">Request headers</span></span>
|<span data-ttu-id="01d35-127">名称</span><span class="sxs-lookup"><span data-stu-id="01d35-127">Name</span></span>|<span data-ttu-id="01d35-128">说明</span><span class="sxs-lookup"><span data-stu-id="01d35-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="01d35-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="01d35-129">Authorization</span></span>|<span data-ttu-id="01d35-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01d35-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d35-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="01d35-132">Request body</span></span>
<span data-ttu-id="01d35-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01d35-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01d35-134">响应</span><span class="sxs-lookup"><span data-stu-id="01d35-134">Response</span></span>

<span data-ttu-id="01d35-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="01d35-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01d35-136">示例</span><span class="sxs-lookup"><span data-stu-id="01d35-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01d35-137">请求</span><span class="sxs-lookup"><span data-stu-id="01d35-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser(on='dce468b2-68b2-dce4-b268-e4dcb268e4dc')
```


### <a name="response"></a><span data-ttu-id="01d35-138">响应</span><span class="sxs-lookup"><span data-stu-id="01d35-138">Response</span></span>
<span data-ttu-id="01d35-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="01d35-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentSchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "assignmentType": "Eligible",
      "memberType": "direct"
    }
  ]
}
```

