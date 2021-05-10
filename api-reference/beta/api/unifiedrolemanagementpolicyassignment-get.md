---
title: 获取 unifiedRoleManagementPolicyAssignment
description: 读取 unifiedRoleManagementPolicyAssignment 对象的属性和关系。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45c74509b4530981d0417874f1490c3596d88898
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299146"
---
# <a name="get-unifiedrolemanagementpolicyassignment"></a><span data-ttu-id="fb71d-103">获取 unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fb71d-103">Get unifiedRoleManagementPolicyAssignment</span></span>
<span data-ttu-id="fb71d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb71d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb71d-105">读取 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb71d-105">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb71d-106">权限</span><span class="sxs-lookup"><span data-stu-id="fb71d-106">Permissions</span></span>
<span data-ttu-id="fb71d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb71d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb71d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb71d-109">Permission type</span></span>|<span data-ttu-id="fb71d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb71d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb71d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb71d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb71d-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fb71d-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="fb71d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb71d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb71d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="fb71d-114">Not supported</span></span>|
|<span data-ttu-id="fb71d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb71d-115">Application</span></span>|<span data-ttu-id="fb71d-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fb71d-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb71d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb71d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments/{unifiedRoleManagementPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb71d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb71d-118">Optional query parameters</span></span>
<span data-ttu-id="fb71d-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb71d-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fb71d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fb71d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb71d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb71d-121">Request headers</span></span>
|<span data-ttu-id="fb71d-122">名称</span><span class="sxs-lookup"><span data-stu-id="fb71d-122">Name</span></span>|<span data-ttu-id="fb71d-123">说明</span><span class="sxs-lookup"><span data-stu-id="fb71d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb71d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb71d-124">Authorization</span></span>|<span data-ttu-id="fb71d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb71d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb71d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb71d-127">Request body</span></span>
<span data-ttu-id="fb71d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb71d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb71d-129">响应</span><span class="sxs-lookup"><span data-stu-id="fb71d-129">Response</span></span>

<span data-ttu-id="fb71d-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb71d-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb71d-131">示例</span><span class="sxs-lookup"><span data-stu-id="fb71d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb71d-132">请求</span><span class="sxs-lookup"><span data-stu-id="fb71d-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6
```


### <a name="response"></a><span data-ttu-id="fb71d-133">响应</span><span class="sxs-lookup"><span data-stu-id="fb71d-133">Response</span></span>
<span data-ttu-id="fb71d-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fb71d-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeType": "subscription",
    "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
  }
}
```

