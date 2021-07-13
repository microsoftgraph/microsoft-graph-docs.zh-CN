---
title: 获取 managementActionTenantDeploymentStatus
description: 读取 managementActionTenantDeploymentStatus 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9efb91eed729ed88d7f95554d752d85e1510480b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402232"
---
# <a name="get-managementactiontenantdeploymentstatus"></a><span data-ttu-id="0ea0a-103">获取 managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="0ea0a-103">Get managementActionTenantDeploymentStatus</span></span>
<span data-ttu-id="0ea0a-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0ea0a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea0a-105">读取 [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-105">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ea0a-106">Permissions</span></span>
<span data-ttu-id="0ea0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ea0a-109">Permission type</span></span>|<span data-ttu-id="0ea0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ea0a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ea0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ea0a-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea0a-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="0ea0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ea0a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-114">Not supported.</span></span>|
|<span data-ttu-id="0ea0a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ea0a-115">Application</span></span>|<span data-ttu-id="0ea0a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ea0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ea0a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ea0a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ea0a-118">Optional query parameters</span></span>
<span data-ttu-id="0ea0a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea0a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ea0a-120">Request headers</span></span>
|<span data-ttu-id="0ea0a-121">名称</span><span class="sxs-lookup"><span data-stu-id="0ea0a-121">Name</span></span>|<span data-ttu-id="0ea0a-122">说明</span><span class="sxs-lookup"><span data-stu-id="0ea0a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ea0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea0a-123">Authorization</span></span>|<span data-ttu-id="0ea0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ea0a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ea0a-126">Request body</span></span>
<span data-ttu-id="0ea0a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea0a-128">响应</span><span class="sxs-lookup"><span data-stu-id="0ea0a-128">Response</span></span>

<span data-ttu-id="0ea0a-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-129">If successful, this method returns a `200 OK` response code and a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ea0a-130">示例</span><span class="sxs-lookup"><span data-stu-id="0ea0a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ea0a-131">请求</span><span class="sxs-lookup"><span data-stu-id="0ea0a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

### <a name="response"></a><span data-ttu-id="0ea0a-132">响应</span><span class="sxs-lookup"><span data-stu-id="0ea0a-132">Response</span></span>
><span data-ttu-id="0ea0a-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/$entity",
    "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "statuses": [
        {
            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "status": "completed",
                    "deployedPolicyId": "949e8893-68fb-4c9d-b8a0-13c229a7e397",
                    "lastDeploymentDateTime": "2021-06-22T04:09:20.3054223Z",
                    "error": null
                }
            ]
        },
        {
            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
            "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                    "status": "completed",
                    "deployedPolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
                    "lastDeploymentDateTime": "2021-06-22T17:01:44.851214Z",
                    "error": null
                }
            ]
        }
    ]
}
```
