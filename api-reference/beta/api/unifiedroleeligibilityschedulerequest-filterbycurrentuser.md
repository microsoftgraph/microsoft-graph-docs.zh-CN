---
title: unifiedRoleEligibilityScheduleRequest： filterByCurrentUser
description: 获取 unifiedRoleEligibilityScheduleRequest 对象及其属性的列表，这些对象按特定用户主体进行筛选
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8ad251e390eae9f328b425c1083f189d5c6989a5
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334673"
---
# <a name="unifiedroleeligibilityschedulerequest-filterbycurrentuser"></a><span data-ttu-id="45ebf-103">unifiedRoleEligibilityScheduleRequest： filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="45ebf-103">unifiedRoleEligibilityScheduleRequest: filterByCurrentUser</span></span>
<span data-ttu-id="45ebf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45ebf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45ebf-105">获取与特定主体对象关联的 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="45ebf-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45ebf-106">权限</span><span class="sxs-lookup"><span data-stu-id="45ebf-106">Permissions</span></span>
<span data-ttu-id="45ebf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45ebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45ebf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45ebf-109">Permission type</span></span>|<span data-ttu-id="45ebf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45ebf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45ebf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45ebf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45ebf-112">RoleEligibilitySchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleEligibilitySchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="45ebf-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="45ebf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45ebf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45ebf-114">不支持</span><span class="sxs-lookup"><span data-stu-id="45ebf-114">Not supported</span></span>|
|<span data-ttu-id="45ebf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45ebf-115">Application</span></span>|<span data-ttu-id="45ebf-116">RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="45ebf-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="45ebf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45ebf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="45ebf-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="45ebf-118">Function parameters</span></span>
<span data-ttu-id="45ebf-119">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="45ebf-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="45ebf-120">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="45ebf-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="45ebf-121">参数</span><span class="sxs-lookup"><span data-stu-id="45ebf-121">Parameter</span></span>|<span data-ttu-id="45ebf-122">类型</span><span class="sxs-lookup"><span data-stu-id="45ebf-122">Type</span></span>|<span data-ttu-id="45ebf-123">说明</span><span class="sxs-lookup"><span data-stu-id="45ebf-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45ebf-124">on</span><span class="sxs-lookup"><span data-stu-id="45ebf-124">on</span></span>|<span data-ttu-id="45ebf-125">RoleEligibilityScheduleRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="45ebf-125">RoleEligibilityScheduleRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="45ebf-126">主体对象的 ID</span><span class="sxs-lookup"><span data-stu-id="45ebf-126">ID of the principal object</span></span>|


## <a name="request-headers"></a><span data-ttu-id="45ebf-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="45ebf-127">Request headers</span></span>
|<span data-ttu-id="45ebf-128">名称</span><span class="sxs-lookup"><span data-stu-id="45ebf-128">Name</span></span>|<span data-ttu-id="45ebf-129">说明</span><span class="sxs-lookup"><span data-stu-id="45ebf-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45ebf-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="45ebf-130">Authorization</span></span>|<span data-ttu-id="45ebf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45ebf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45ebf-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="45ebf-133">Request body</span></span>
<span data-ttu-id="45ebf-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45ebf-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45ebf-135">响应</span><span class="sxs-lookup"><span data-stu-id="45ebf-135">Response</span></span>

<span data-ttu-id="45ebf-136">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="45ebf-136">If successful, this function returns a `200 OK` response code and a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45ebf-137">示例</span><span class="sxs-lookup"><span data-stu-id="45ebf-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45ebf-138">请求</span><span class="sxs-lookup"><span data-stu-id="45ebf-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedRoleEligibilityScheduleRequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser(on='parameterValue')
```


### <a name="response"></a><span data-ttu-id="45ebf-139">响应</span><span class="sxs-lookup"><span data-stu-id="45ebf-139">Response</span></span>
<span data-ttu-id="45ebf-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="45ebf-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "String (identifier)",
      "action": "String",
      "principalId": "String",
      "roleDefinitionId": "String",
      "directoryScopeId": "String",
      "appScopeId": "String",
      "isValidationOnly": "Boolean",
      "targetScheduleId": "String",
      "justification": "String",
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

