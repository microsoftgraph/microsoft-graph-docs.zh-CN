---
title: 列出 deviceCompliancePolicySettingStateSummary
description: 获取 deviceCompliancePolicySettingStateSummary 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 46374c975bbb8d33d7ad8d74eece3f163d9f9165
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402029"
---
# <a name="list-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="0d6d2-103">列出 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="0d6d2-103">List deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="0d6d2-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0d6d2-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d6d2-105">获取 [deviceCompliancePolicySettingStateSummary 对象](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-105">Get a list of the [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d6d2-106">权限</span><span class="sxs-lookup"><span data-stu-id="0d6d2-106">Permissions</span></span>
<span data-ttu-id="0d6d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d6d2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d6d2-109">Permission type</span></span>|<span data-ttu-id="0d6d2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d6d2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d6d2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d6d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d6d2-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d6d2-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0d6d2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d6d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d6d2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-114">Not supported.</span></span>|
|<span data-ttu-id="0d6d2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d6d2-115">Application</span></span>|<span data-ttu-id="0d6d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d6d2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d6d2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d6d2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0d6d2-118">Optional query parameters</span></span>
<span data-ttu-id="0d6d2-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d6d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d6d2-120">Request headers</span></span>
|<span data-ttu-id="0d6d2-121">名称</span><span class="sxs-lookup"><span data-stu-id="0d6d2-121">Name</span></span>|<span data-ttu-id="0d6d2-122">说明</span><span class="sxs-lookup"><span data-stu-id="0d6d2-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d6d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d6d2-123">Authorization</span></span>|<span data-ttu-id="0d6d2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d6d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d6d2-126">Request body</span></span>
<span data-ttu-id="0d6d2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d6d2-128">响应</span><span class="sxs-lookup"><span data-stu-id="0d6d2-128">Response</span></span>

<span data-ttu-id="0d6d2-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d6d2-130">示例</span><span class="sxs-lookup"><span data-stu-id="0d6d2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d6d2-131">请求</span><span class="sxs-lookup"><span data-stu-id="0d6d2-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```


### <a name="response"></a><span data-ttu-id="0d6d2-132">响应</span><span class="sxs-lookup"><span data-stu-id="0d6d2-132">Response</span></span>
><span data-ttu-id="0d6d2-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d6d2-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
      "id": "9f6922d9-5a58-4f4d-b6e3-708f7659e5b2",
      "tenantId": "String",
      "tenantDisplayName": "String",
      "conflictDeviceCount": "Integer",
      "errorDeviceCount": "Integer",
      "failedDeviceCount": "Integer",
      "intuneAccountId": "String",
      "intuneSettingId": "String",
      "notApplicableDeviceCount": "Integer",
      "pendingDeviceCount": "Integer",
      "policyType": "String",
      "settingName": "String",
      "succeededDeviceCount": "Integer",
      "lastRefreshedDateTime": "String (timestamp)"
    }
  ]
}
```
