---
title: 列出 deviceComplianceDeviceStatuses
description: 列出 deviceComplianceDeviceStatus 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 292677a73b6f62ef4282be81dcf454c189a0943e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168507"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="4ac91-103">列出 deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="4ac91-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="4ac91-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ac91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ac91-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ac91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ac91-106">列出 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ac91-106">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ac91-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ac91-107">Prerequisites</span></span>
<span data-ttu-id="4ac91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ac91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ac91-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ac91-110">Permission type</span></span>|<span data-ttu-id="4ac91-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ac91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ac91-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ac91-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ac91-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ac91-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ac91-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ac91-115">Not supported.</span></span>|
|<span data-ttu-id="4ac91-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ac91-116">Application</span></span>|<span data-ttu-id="4ac91-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ac91-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ac91-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ac91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4ac91-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ac91-119">Request headers</span></span>
|<span data-ttu-id="4ac91-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ac91-120">Header</span></span>|<span data-ttu-id="4ac91-121">值</span><span class="sxs-lookup"><span data-stu-id="4ac91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ac91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ac91-122">Authorization</span></span>|<span data-ttu-id="4ac91-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ac91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ac91-124">接受</span><span class="sxs-lookup"><span data-stu-id="4ac91-124">Accept</span></span>|<span data-ttu-id="4ac91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ac91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ac91-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ac91-126">Request body</span></span>
<span data-ttu-id="4ac91-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ac91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ac91-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ac91-128">Response</span></span>
<span data-ttu-id="4ac91-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ac91-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ac91-130">示例</span><span class="sxs-lookup"><span data-stu-id="4ac91-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ac91-131">请求</span><span class="sxs-lookup"><span data-stu-id="4ac91-131">Request</span></span>
<span data-ttu-id="4ac91-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ac91-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="4ac91-133">响应</span><span class="sxs-lookup"><span data-stu-id="4ac91-133">Response</span></span>
<span data-ttu-id="4ac91-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ac91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
      "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




