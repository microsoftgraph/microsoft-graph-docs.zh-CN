---
title: 获取 deviceComplianceDeviceOverview
description: 读取 deviceComplianceDeviceOverview 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 567595a61cb282b2b26ac9ec1a3ee2d06a5cd6c4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774020"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="fedad-103">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fedad-103">Get deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="fedad-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fedad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fedad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fedad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fedad-106">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fedad-106">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fedad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fedad-107">Prerequisites</span></span>
<span data-ttu-id="fedad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fedad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fedad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fedad-110">Permission type</span></span>|<span data-ttu-id="fedad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fedad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fedad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fedad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fedad-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fedad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fedad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fedad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fedad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fedad-115">Not supported.</span></span>|
|<span data-ttu-id="fedad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fedad-116">Application</span></span>|<span data-ttu-id="fedad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fedad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fedad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fedad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fedad-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fedad-119">Optional query parameters</span></span>
<span data-ttu-id="fedad-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fedad-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fedad-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fedad-121">Request headers</span></span>
|<span data-ttu-id="fedad-122">标头</span><span class="sxs-lookup"><span data-stu-id="fedad-122">Header</span></span>|<span data-ttu-id="fedad-123">值</span><span class="sxs-lookup"><span data-stu-id="fedad-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fedad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fedad-124">Authorization</span></span>|<span data-ttu-id="fedad-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fedad-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fedad-126">接受</span><span class="sxs-lookup"><span data-stu-id="fedad-126">Accept</span></span>|<span data-ttu-id="fedad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fedad-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fedad-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fedad-128">Request body</span></span>
<span data-ttu-id="fedad-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fedad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fedad-130">响应</span><span class="sxs-lookup"><span data-stu-id="fedad-130">Response</span></span>
<span data-ttu-id="fedad-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fedad-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fedad-132">示例</span><span class="sxs-lookup"><span data-stu-id="fedad-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fedad-133">请求</span><span class="sxs-lookup"><span data-stu-id="fedad-133">Request</span></span>
<span data-ttu-id="fedad-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fedad-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="fedad-135">响应</span><span class="sxs-lookup"><span data-stu-id="fedad-135">Response</span></span>
<span data-ttu-id="fedad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fedad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





