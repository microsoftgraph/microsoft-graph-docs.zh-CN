---
title: 获取 deviceComplianceDeviceOverview
description: 读取 deviceComplianceDeviceOverview 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9dc2a7ced8193f1d9f9bc324378b65236e33682d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692049"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="c7c38-103">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c7c38-103">Get deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="c7c38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7c38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7c38-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7c38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7c38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c38-107">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7c38-107">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c38-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7c38-108">Prerequisites</span></span>
<span data-ttu-id="c7c38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c38-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7c38-111">Permission type</span></span>|<span data-ttu-id="c7c38-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7c38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c38-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c38-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7c38-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7c38-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c38-116">Not supported.</span></span>|
|<span data-ttu-id="c7c38-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7c38-117">Application</span></span>|<span data-ttu-id="c7c38-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7c38-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c38-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7c38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7c38-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7c38-120">Optional query parameters</span></span>
<span data-ttu-id="c7c38-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7c38-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7c38-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7c38-122">Request headers</span></span>
|<span data-ttu-id="c7c38-123">标头</span><span class="sxs-lookup"><span data-stu-id="c7c38-123">Header</span></span>|<span data-ttu-id="c7c38-124">值</span><span class="sxs-lookup"><span data-stu-id="c7c38-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c38-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c38-125">Authorization</span></span>|<span data-ttu-id="c7c38-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7c38-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c38-127">接受</span><span class="sxs-lookup"><span data-stu-id="c7c38-127">Accept</span></span>|<span data-ttu-id="c7c38-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c38-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c38-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7c38-129">Request body</span></span>
<span data-ttu-id="c7c38-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7c38-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7c38-131">响应</span><span class="sxs-lookup"><span data-stu-id="c7c38-131">Response</span></span>
<span data-ttu-id="c7c38-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7c38-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c38-133">示例</span><span class="sxs-lookup"><span data-stu-id="c7c38-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c38-134">请求</span><span class="sxs-lookup"><span data-stu-id="c7c38-134">Request</span></span>
<span data-ttu-id="c7c38-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7c38-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="c7c38-136">响应</span><span class="sxs-lookup"><span data-stu-id="c7c38-136">Response</span></span>
<span data-ttu-id="c7c38-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7c38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





