---
title: 获取 deviceComplianceDeviceOverview
description: 读取 deviceComplianceDeviceOverview 对象的属性和关系。
ms.openlocfilehash: e20838865964b397fc70415e34e32a9bdc24aa29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047339"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="94a3f-103">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="94a3f-103">Get deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="94a3f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94a3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94a3f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94a3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94a3f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="94a3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94a3f-107">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94a3f-107">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94a3f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="94a3f-108">Prerequisites</span></span>
<span data-ttu-id="94a3f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="94a3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a3f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94a3f-111">Permission type</span></span>|<span data-ttu-id="94a3f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="94a3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94a3f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94a3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94a3f-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94a3f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="94a3f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94a3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94a3f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94a3f-116">Not supported.</span></span>|
|<span data-ttu-id="94a3f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94a3f-117">Application</span></span>|<span data-ttu-id="94a3f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="94a3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94a3f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94a3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94a3f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94a3f-120">Optional query parameters</span></span>
<span data-ttu-id="94a3f-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="94a3f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94a3f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="94a3f-122">Request headers</span></span>
|<span data-ttu-id="94a3f-123">标头</span><span class="sxs-lookup"><span data-stu-id="94a3f-123">Header</span></span>|<span data-ttu-id="94a3f-124">值</span><span class="sxs-lookup"><span data-stu-id="94a3f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94a3f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="94a3f-125">Authorization</span></span>|<span data-ttu-id="94a3f-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94a3f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94a3f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="94a3f-127">Accept</span></span>|<span data-ttu-id="94a3f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="94a3f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a3f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="94a3f-129">Request body</span></span>
<span data-ttu-id="94a3f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94a3f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a3f-131">响应</span><span class="sxs-lookup"><span data-stu-id="94a3f-131">Response</span></span>
<span data-ttu-id="94a3f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94a3f-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a3f-133">示例</span><span class="sxs-lookup"><span data-stu-id="94a3f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="94a3f-134">请求</span><span class="sxs-lookup"><span data-stu-id="94a3f-134">Request</span></span>
<span data-ttu-id="94a3f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94a3f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="94a3f-136">响应</span><span class="sxs-lookup"><span data-stu-id="94a3f-136">Response</span></span>
<span data-ttu-id="94a3f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94a3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 432

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "886f167b-167b-886f-7b16-6f887b166f88",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





