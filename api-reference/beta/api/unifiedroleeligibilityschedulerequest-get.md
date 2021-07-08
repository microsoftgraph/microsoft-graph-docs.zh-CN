---
title: 获取 unifiedRoleEligibilityScheduleRequest
description: 读取 unifiedRoleEligibilityScheduleRequest 对象的属性和关系。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7f1321f36a4670adff4ed6474fd1dd71ccf9e5f4
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334666"
---
# <a name="get-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="db7f8-103">获取 unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="db7f8-103">Get unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="db7f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db7f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db7f8-105">读取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db7f8-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db7f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="db7f8-106">Permissions</span></span>
<span data-ttu-id="db7f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db7f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db7f8-109">Permission type</span></span>|<span data-ttu-id="db7f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db7f8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db7f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db7f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="db7f8-112">RoleEligibilitySchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleEligibilitySchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="db7f8-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="db7f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db7f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db7f8-114">不支持</span><span class="sxs-lookup"><span data-stu-id="db7f8-114">Not supported</span></span>|
|<span data-ttu-id="db7f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db7f8-115">Application</span></span>|<span data-ttu-id="db7f8-116">RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="db7f8-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="db7f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db7f8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db7f8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db7f8-118">Optional query parameters</span></span>
<span data-ttu-id="db7f8-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db7f8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="db7f8-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="db7f8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db7f8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="db7f8-121">Request headers</span></span>
|<span data-ttu-id="db7f8-122">名称</span><span class="sxs-lookup"><span data-stu-id="db7f8-122">Name</span></span>|<span data-ttu-id="db7f8-123">说明</span><span class="sxs-lookup"><span data-stu-id="db7f8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="db7f8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="db7f8-124">Authorization</span></span>|<span data-ttu-id="db7f8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db7f8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db7f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db7f8-127">Request body</span></span>
<span data-ttu-id="db7f8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db7f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db7f8-129">响应</span><span class="sxs-lookup"><span data-stu-id="db7f8-129">Response</span></span>

<span data-ttu-id="db7f8-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db7f8-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db7f8-131">示例</span><span class="sxs-lookup"><span data-stu-id="db7f8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db7f8-132">请求</span><span class="sxs-lookup"><span data-stu-id="db7f8-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="db7f8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db7f8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```
# <a name="c"></a>[<span data-ttu-id="db7f8-134">C#</span><span class="sxs-lookup"><span data-stu-id="db7f8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db7f8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db7f8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db7f8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db7f8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db7f8-137">Java</span><span class="sxs-lookup"><span data-stu-id="db7f8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="db7f8-138">响应</span><span class="sxs-lookup"><span data-stu-id="db7f8-138">Response</span></span>
<span data-ttu-id="db7f8-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db7f8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

