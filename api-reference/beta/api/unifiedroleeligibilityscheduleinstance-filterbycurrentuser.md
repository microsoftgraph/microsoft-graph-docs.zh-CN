---
title: unifiedRoleEligibilityScheduleInstance：filterByCurrentUser
description: 获取 unifiedRoleEligibilityScheduleInstance 对象及其属性的列表，这些对象按特定用户主体进行筛选
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 724933c90a7a404b360e19a76304ba1d99be25bb
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679909"
---
# <a name="unifiedroleeligibilityscheduleinstance-filterbycurrentuser"></a><span data-ttu-id="b55f8-103">unifiedRoleEligibilityScheduleInstance：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="b55f8-103">unifiedRoleEligibilityScheduleInstance: filterByCurrentUser</span></span>
<span data-ttu-id="b55f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b55f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b55f8-105">获取 [unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) 对象及其与特定主体对象关联的属性的列表。</span><span class="sxs-lookup"><span data-stu-id="b55f8-105">Get a list of the [unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b55f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="b55f8-106">Permissions</span></span>
<span data-ttu-id="b55f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b55f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b55f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b55f8-109">Permission type</span></span>|<span data-ttu-id="b55f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b55f8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b55f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b55f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b55f8-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b55f8-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="b55f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b55f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b55f8-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b55f8-114">Not supported</span></span>|
|<span data-ttu-id="b55f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b55f8-115">Application</span></span>|<span data-ttu-id="b55f8-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b55f8-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="b55f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b55f8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="b55f8-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="b55f8-118">Query parameters</span></span>
<span data-ttu-id="b55f8-119">下表显示了可用于此方法的查询参数。</span><span class="sxs-lookup"><span data-stu-id="b55f8-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="b55f8-120">参数</span><span class="sxs-lookup"><span data-stu-id="b55f8-120">Parameter</span></span>|<span data-ttu-id="b55f8-121">类型</span><span class="sxs-lookup"><span data-stu-id="b55f8-121">Type</span></span>|<span data-ttu-id="b55f8-122">说明</span><span class="sxs-lookup"><span data-stu-id="b55f8-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b55f8-123">on</span><span class="sxs-lookup"><span data-stu-id="b55f8-123">on</span></span>|<span data-ttu-id="b55f8-124">roleEligibilityScheduleInstanceFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="b55f8-124">roleEligibilityScheduleInstanceFilterByCurrentUserOptions</span></span>|<span data-ttu-id="b55f8-125">当前用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="b55f8-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="b55f8-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="b55f8-126">Request headers</span></span>
|<span data-ttu-id="b55f8-127">名称</span><span class="sxs-lookup"><span data-stu-id="b55f8-127">Name</span></span>|<span data-ttu-id="b55f8-128">说明</span><span class="sxs-lookup"><span data-stu-id="b55f8-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b55f8-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b55f8-129">Authorization</span></span>|<span data-ttu-id="b55f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b55f8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b55f8-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b55f8-132">Request body</span></span>
<span data-ttu-id="b55f8-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b55f8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b55f8-134">响应</span><span class="sxs-lookup"><span data-stu-id="b55f8-134">Response</span></span>

<span data-ttu-id="b55f8-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="b55f8-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b55f8-136">示例</span><span class="sxs-lookup"><span data-stu-id="b55f8-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b55f8-137">请求</span><span class="sxs-lookup"><span data-stu-id="b55f8-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityscheduleinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser(on='5cfd7709-7709-5cfd-0977-fd5c0977fd5c')
```


### <a name="response"></a><span data-ttu-id="b55f8-138">响应</span><span class="sxs-lookup"><span data-stu-id="b55f8-138">Response</span></span>
<span data-ttu-id="b55f8-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b55f8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "memberType": "direct",
      "roleEligibilityScheduleId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c"
    }
  ]
}
```

