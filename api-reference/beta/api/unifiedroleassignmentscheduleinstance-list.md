---
title: 列出 unifiedRoleAssignmentScheduleInstances
description: 获取 unifiedRoleAssignmentScheduleInstance 对象及其属性的列表。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b38fdad1f83e62b40ce2336492fe5f49e3bc1ff0
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299221"
---
# <a name="list-unifiedroleassignmentscheduleinstances"></a><span data-ttu-id="63379-103">列出 unifiedRoleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="63379-103">List unifiedRoleAssignmentScheduleInstances</span></span>
<span data-ttu-id="63379-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63379-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63379-105">获取 [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="63379-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="63379-106">权限</span><span class="sxs-lookup"><span data-stu-id="63379-106">Permissions</span></span>
<span data-ttu-id="63379-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63379-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63379-109">Permission type</span></span>|<span data-ttu-id="63379-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63379-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63379-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63379-111">Delegated (work or school account)</span></span>|<span data-ttu-id="63379-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="63379-112">RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="63379-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63379-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63379-114">不支持</span><span class="sxs-lookup"><span data-stu-id="63379-114">Not supported</span></span>|
|<span data-ttu-id="63379-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="63379-115">Application</span></span>|<span data-ttu-id="63379-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="63379-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="63379-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63379-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63379-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63379-118">Optional query parameters</span></span>
<span data-ttu-id="63379-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63379-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="63379-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="63379-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="63379-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="63379-121">Request headers</span></span>
|<span data-ttu-id="63379-122">名称</span><span class="sxs-lookup"><span data-stu-id="63379-122">Name</span></span>|<span data-ttu-id="63379-123">说明</span><span class="sxs-lookup"><span data-stu-id="63379-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="63379-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="63379-124">Authorization</span></span>|<span data-ttu-id="63379-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63379-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63379-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63379-127">Request body</span></span>
<span data-ttu-id="63379-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63379-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63379-129">响应</span><span class="sxs-lookup"><span data-stu-id="63379-129">Response</span></span>

<span data-ttu-id="63379-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="63379-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63379-131">示例</span><span class="sxs-lookup"><span data-stu-id="63379-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63379-132">请求</span><span class="sxs-lookup"><span data-stu-id="63379-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances
```


### <a name="response"></a><span data-ttu-id="63379-133">响应</span><span class="sxs-lookup"><span data-stu-id="63379-133">Response</span></span>
<span data-ttu-id="63379-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63379-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

