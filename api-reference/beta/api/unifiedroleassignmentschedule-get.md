---
title: 获取 unifiedRoleAssignmentSchedule
description: 读取 unifiedRoleAssignmentSchedule 对象的属性和关系。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ab460a395fe535928fb590e367bb008174d70c43
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334470"
---
# <a name="get-unifiedroleassignmentschedule"></a><span data-ttu-id="294d4-103">获取 unifiedRoleAssignmentSchedule</span><span class="sxs-lookup"><span data-stu-id="294d4-103">Get unifiedRoleAssignmentSchedule</span></span>
<span data-ttu-id="294d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="294d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="294d4-105">读取 [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="294d4-105">Read the properties and relationships of an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="294d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="294d4-106">Permissions</span></span>
<span data-ttu-id="294d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="294d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="294d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="294d4-109">Permission type</span></span>|<span data-ttu-id="294d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="294d4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="294d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="294d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="294d4-112">RoleAssignmentSchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="294d4-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>|
|<span data-ttu-id="294d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="294d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="294d4-114">不支持</span><span class="sxs-lookup"><span data-stu-id="294d4-114">Not supported</span></span>|
|<span data-ttu-id="294d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="294d4-115">Application</span></span>|<span data-ttu-id="294d4-116">RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="294d4-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="294d4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="294d4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentSchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="294d4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="294d4-118">Optional query parameters</span></span>
<span data-ttu-id="294d4-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="294d4-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="294d4-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="294d4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="294d4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="294d4-121">Request headers</span></span>
|<span data-ttu-id="294d4-122">名称</span><span class="sxs-lookup"><span data-stu-id="294d4-122">Name</span></span>|<span data-ttu-id="294d4-123">说明</span><span class="sxs-lookup"><span data-stu-id="294d4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="294d4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="294d4-124">Authorization</span></span>|<span data-ttu-id="294d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="294d4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="294d4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="294d4-127">Request body</span></span>
<span data-ttu-id="294d4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="294d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="294d4-129">响应</span><span class="sxs-lookup"><span data-stu-id="294d4-129">Response</span></span>

<span data-ttu-id="294d4-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="294d4-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="294d4-131">示例</span><span class="sxs-lookup"><span data-stu-id="294d4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="294d4-132">请求</span><span class="sxs-lookup"><span data-stu-id="294d4-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413
```


### <a name="response"></a><span data-ttu-id="294d4-133">响应</span><span class="sxs-lookup"><span data-stu-id="294d4-133">Response</span></span>
<span data-ttu-id="294d4-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="294d4-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

