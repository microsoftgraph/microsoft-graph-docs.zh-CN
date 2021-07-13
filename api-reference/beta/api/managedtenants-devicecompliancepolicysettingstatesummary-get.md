---
title: 获取 deviceCompliancePolicySettingStateSummary
description: 读取 deviceCompliancePolicySettingStateSummary 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e1396b66dda6925be6c895aac741d81122d64c98
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402048"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="d9a67-103">获取 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9a67-103">Get deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="d9a67-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d9a67-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9a67-105">读取 [deviceCompliancePolicySettingStateSummary 对象的属性和](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d9a67-105">Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9a67-106">权限</span><span class="sxs-lookup"><span data-stu-id="d9a67-106">Permissions</span></span>
<span data-ttu-id="d9a67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9a67-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9a67-109">Permission type</span></span>|<span data-ttu-id="d9a67-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9a67-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9a67-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9a67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9a67-112">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a67-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9a67-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9a67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9a67-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9a67-114">Not supported.</span></span>|
|<span data-ttu-id="d9a67-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9a67-115">Application</span></span>|<span data-ttu-id="d9a67-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9a67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9a67-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9a67-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9a67-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d9a67-118">Optional query parameters</span></span>
<span data-ttu-id="d9a67-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="d9a67-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9a67-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9a67-120">Request headers</span></span>
|<span data-ttu-id="d9a67-121">名称</span><span class="sxs-lookup"><span data-stu-id="d9a67-121">Name</span></span>|<span data-ttu-id="d9a67-122">说明</span><span class="sxs-lookup"><span data-stu-id="d9a67-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9a67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9a67-123">Authorization</span></span>|<span data-ttu-id="d9a67-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9a67-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9a67-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9a67-126">Request body</span></span>
<span data-ttu-id="d9a67-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9a67-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9a67-128">响应</span><span class="sxs-lookup"><span data-stu-id="d9a67-128">Response</span></span>

<span data-ttu-id="d9a67-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9a67-129">If successful, this method returns a `200 OK` response code and a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9a67-130">示例</span><span class="sxs-lookup"><span data-stu-id="d9a67-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9a67-131">请求</span><span class="sxs-lookup"><span data-stu-id="d9a67-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```


### <a name="response"></a><span data-ttu-id="d9a67-132">响应</span><span class="sxs-lookup"><span data-stu-id="d9a67-132">Response</span></span>
><span data-ttu-id="d9a67-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d9a67-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_277f9230-81f7-ffc3-af78-4662ec3dca09",
    "intuneAccountId": "6f3e6534-b466-4fac-9a31-4c305cc40833",
    "intuneSettingId": "277f9230-81f7-ffc3-af78-4662ec3dca09",
    "policyType": "DefaultDeviceCompliancePolicy",
    "settingName": "RequireDeviceCompliancePolicyAssigned",
    "failedDeviceCount": 0,
    "errorDeviceCount": 4,
    "conflictDeviceCount": 0,
    "lastRefreshedDateTime": "2021-07-11T00:00:00Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
