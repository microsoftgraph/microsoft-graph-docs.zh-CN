---
title: 列出 deviceComplianceDeviceStatuses
description: 列出 deviceComplianceDeviceStatus 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0eda119119dd2b85659740a2adf4bf7c828af74
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083580"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="6d6d9-103">列出 deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6d6d9-103">List deviceComplianceDeviceStatuses</span></span>

<span data-ttu-id="6d6d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d6d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d6d9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d6d9-106">列出 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-106">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d6d9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d6d9-107">Prerequisites</span></span>
<span data-ttu-id="6d6d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d6d9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d6d9-110">Permission type</span></span>|<span data-ttu-id="6d6d9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6d6d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d6d9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d6d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d6d9-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d6d9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6d6d9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d6d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d6d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-115">Not supported.</span></span>|
|<span data-ttu-id="6d6d9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d6d9-116">Application</span></span>|<span data-ttu-id="6d6d9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d6d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d6d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6d6d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d6d9-119">Request headers</span></span>
|<span data-ttu-id="6d6d9-120">标头</span><span class="sxs-lookup"><span data-stu-id="6d6d9-120">Header</span></span>|<span data-ttu-id="6d6d9-121">值</span><span class="sxs-lookup"><span data-stu-id="6d6d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d6d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d6d9-122">Authorization</span></span>|<span data-ttu-id="6d6d9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d6d9-124">接受</span><span class="sxs-lookup"><span data-stu-id="6d6d9-124">Accept</span></span>|<span data-ttu-id="6d6d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d6d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d6d9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d6d9-126">Request body</span></span>
<span data-ttu-id="6d6d9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d6d9-128">响应</span><span class="sxs-lookup"><span data-stu-id="6d6d9-128">Response</span></span>
<span data-ttu-id="6d6d9-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d6d9-130">示例</span><span class="sxs-lookup"><span data-stu-id="6d6d9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d6d9-131">请求</span><span class="sxs-lookup"><span data-stu-id="6d6d9-131">Request</span></span>
<span data-ttu-id="6d6d9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="6d6d9-133">响应</span><span class="sxs-lookup"><span data-stu-id="6d6d9-133">Response</span></span>
<span data-ttu-id="6d6d9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d6d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 544

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
      "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```









