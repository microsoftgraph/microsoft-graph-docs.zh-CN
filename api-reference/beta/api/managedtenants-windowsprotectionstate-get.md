---
title: 获取 windowsProtectionState
description: 读取 windowsProtectionState 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: dc82bbc7dfa7265471cbc6b99f1463d59db5b526
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402364"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="3f3ad-103">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="3f3ad-103">Get windowsProtectionState</span></span>
<span data-ttu-id="3f3ad-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3f3ad-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f3ad-105">读取 [windowsProtectionState 对象的属性和](../resources/managedtenants-windowsprotectionstate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-105">Read the properties and relationships of a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f3ad-106">权限</span><span class="sxs-lookup"><span data-stu-id="3f3ad-106">Permissions</span></span>
<span data-ttu-id="3f3ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f3ad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f3ad-109">Permission type</span></span>|<span data-ttu-id="3f3ad-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f3ad-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f3ad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f3ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f3ad-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f3ad-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3f3ad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f3ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f3ad-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-114">Not supported.</span></span>|
|<span data-ttu-id="3f3ad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f3ad-115">Application</span></span>|<span data-ttu-id="3f3ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f3ad-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f3ad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f3ad-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3f3ad-118">Optional query parameters</span></span>
<span data-ttu-id="3f3ad-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f3ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f3ad-120">Request headers</span></span>
|<span data-ttu-id="3f3ad-121">名称</span><span class="sxs-lookup"><span data-stu-id="3f3ad-121">Name</span></span>|<span data-ttu-id="3f3ad-122">说明</span><span class="sxs-lookup"><span data-stu-id="3f3ad-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3f3ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f3ad-123">Authorization</span></span>|<span data-ttu-id="3f3ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f3ad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f3ad-126">Request body</span></span>
<span data-ttu-id="3f3ad-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f3ad-128">响应</span><span class="sxs-lookup"><span data-stu-id="3f3ad-128">Response</span></span>

<span data-ttu-id="3f3ad-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-129">If successful, this method returns a `200 OK` response code and a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f3ad-130">示例</span><span class="sxs-lookup"><span data-stu-id="3f3ad-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f3ad-131">请求</span><span class="sxs-lookup"><span data-stu-id="3f3ad-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```


### <a name="response"></a><span data-ttu-id="3f3ad-132">响应</span><span class="sxs-lookup"><span data-stu-id="3f3ad-132">Response</span></span>
><span data-ttu-id="3f3ad-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3f3ad-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.windowsProtectionState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/windowsProtectionStates/$entity",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceName": "vm11",
    "malwareProtectionEnabled": true,
    "managedDeviceHealthState": "Clean",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": false,
    "fullScanOverdue": false,
    "signatureUpdateOverdue": false,
    "rebootRequired": false,
    "attentionRequired": false,
    "fullScanRequired": false,
    "engineVersion": "1.1.18300.4",
    "signatureVersion": "1.343.642.0",
    "antiMalwareVersion": "4.18.2106.6",
    "lastQuickScanDateTime": "2021-06-24T14:50:28Z",
    "lastFullScanDateTime": null,
    "lastQuickScanSignatureVersion": "1.341.1288.0",
    "lastFullScanSignatureVersion": "0.0.0.0",
    "lastReportedDateTime": "2021-07-09T14:43:45Z",
    "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
    "deviceDeleted": false,
    "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee",
    "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
}
```
