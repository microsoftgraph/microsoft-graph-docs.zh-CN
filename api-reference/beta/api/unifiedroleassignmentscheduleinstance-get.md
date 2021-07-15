---
title: 获取 unifiedRoleAssignmentScheduleInstance
description: 读取 unifiedRoleAssignmentScheduleInstance 对象的属性和关系。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6b7a78215ce3311d0f70f24ceba30507969532ca
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442675"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a><span data-ttu-id="832f6-103">获取 unifiedRoleAssignmentScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="832f6-103">Get unifiedRoleAssignmentScheduleInstance</span></span>
<span data-ttu-id="832f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="832f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="832f6-105">读取 [unifiedRoleAssignmentScheduleInstance 对象的属性和](../resources/unifiedroleassignmentscheduleinstance.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="832f6-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="832f6-106">权限</span><span class="sxs-lookup"><span data-stu-id="832f6-106">Permissions</span></span>
<span data-ttu-id="832f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="832f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="832f6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="832f6-109">Permission type</span></span>|<span data-ttu-id="832f6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="832f6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="832f6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="832f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="832f6-112">RoleAssignmentSchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleAssignmentSchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="832f6-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="832f6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="832f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="832f6-114">不支持</span><span class="sxs-lookup"><span data-stu-id="832f6-114">Not supported</span></span>|
|<span data-ttu-id="832f6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="832f6-115">Application</span></span>|<span data-ttu-id="832f6-116">RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="832f6-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="832f6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="832f6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="832f6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="832f6-118">Optional query parameters</span></span>
<span data-ttu-id="832f6-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="832f6-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="832f6-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="832f6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="832f6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="832f6-121">Request headers</span></span>
|<span data-ttu-id="832f6-122">名称</span><span class="sxs-lookup"><span data-stu-id="832f6-122">Name</span></span>|<span data-ttu-id="832f6-123">说明</span><span class="sxs-lookup"><span data-stu-id="832f6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="832f6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="832f6-124">Authorization</span></span>|<span data-ttu-id="832f6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="832f6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="832f6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="832f6-127">Request body</span></span>
<span data-ttu-id="832f6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="832f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="832f6-129">响应</span><span class="sxs-lookup"><span data-stu-id="832f6-129">Response</span></span>

<span data-ttu-id="832f6-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="832f6-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="832f6-131">示例</span><span class="sxs-lookup"><span data-stu-id="832f6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="832f6-132">请求</span><span class="sxs-lookup"><span data-stu-id="832f6-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="832f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="832f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```
# <a name="c"></a>[<span data-ttu-id="832f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="832f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="832f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="832f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="832f6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="832f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="832f6-137">Java</span><span class="sxs-lookup"><span data-stu-id="832f6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="832f6-138">响应</span><span class="sxs-lookup"><span data-stu-id="832f6-138">Response</span></span>
<span data-ttu-id="832f6-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="832f6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "startDateTime": "2020-09-09T21:35:27.91Z",
    "endDateTime": "2020-09-09T21:35:27.91Z",
    "assignmentType": "eligible",
    "memberType": "direct",
    "roleAssignmentOriginId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleAssignmentScheduleId": "eb18c026-c026-eb18-26c0-18eb26c018eb"
  }
}
```

