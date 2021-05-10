---
title: 列出 unifiedRoleEligibilityScheduleRequests
description: 获取 unifiedRoleEligibilityScheduleRequest 对象及其属性的列表。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ff80105188d8106528805cf92b8300db25fdcec
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299200"
---
# <a name="list-unifiedroleeligibilityschedulerequests"></a><span data-ttu-id="7fe08-103">列出 unifiedRoleEligibilityScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="7fe08-103">List unifiedRoleEligibilityScheduleRequests</span></span>
<span data-ttu-id="7fe08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fe08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fe08-105">获取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="7fe08-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fe08-106">权限</span><span class="sxs-lookup"><span data-stu-id="7fe08-106">Permissions</span></span>
<span data-ttu-id="7fe08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fe08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe08-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fe08-109">Permission type</span></span>|<span data-ttu-id="7fe08-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fe08-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe08-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe08-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7fe08-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="7fe08-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe08-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe08-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7fe08-114">Not supported</span></span>|
|<span data-ttu-id="7fe08-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fe08-115">Application</span></span>|<span data-ttu-id="7fe08-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7fe08-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe08-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fe08-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fe08-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7fe08-118">Optional query parameters</span></span>
<span data-ttu-id="7fe08-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7fe08-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7fe08-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7fe08-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fe08-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fe08-121">Request headers</span></span>
|<span data-ttu-id="7fe08-122">名称</span><span class="sxs-lookup"><span data-stu-id="7fe08-122">Name</span></span>|<span data-ttu-id="7fe08-123">说明</span><span class="sxs-lookup"><span data-stu-id="7fe08-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7fe08-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fe08-124">Authorization</span></span>|<span data-ttu-id="7fe08-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fe08-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe08-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fe08-127">Request body</span></span>
<span data-ttu-id="7fe08-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7fe08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fe08-129">响应</span><span class="sxs-lookup"><span data-stu-id="7fe08-129">Response</span></span>

<span data-ttu-id="7fe08-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7fe08-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fe08-131">示例</span><span class="sxs-lookup"><span data-stu-id="7fe08-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fe08-132">请求</span><span class="sxs-lookup"><span data-stu-id="7fe08-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
```


### <a name="response"></a><span data-ttu-id="7fe08-133">响应</span><span class="sxs-lookup"><span data-stu-id="7fe08-133">Response</span></span>
<span data-ttu-id="7fe08-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7fe08-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
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

