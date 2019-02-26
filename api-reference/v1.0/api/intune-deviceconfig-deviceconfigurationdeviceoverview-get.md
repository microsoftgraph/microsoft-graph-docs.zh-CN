---
title: 获取 deviceConfigurationDeviceOverview
description: 读取 deviceConfigurationDeviceOverview 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 966187ff9815559d62a94f5baf64702116e88b5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258049"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="05aaa-103">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="05aaa-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="05aaa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05aaa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05aaa-105">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05aaa-105">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05aaa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="05aaa-106">Prerequisites</span></span>
<span data-ttu-id="05aaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="05aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05aaa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05aaa-109">Permission type</span></span>|<span data-ttu-id="05aaa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05aaa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05aaa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05aaa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05aaa-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05aaa-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="05aaa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05aaa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05aaa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05aaa-114">Not supported.</span></span>|
|<span data-ttu-id="05aaa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05aaa-115">Application</span></span>|<span data-ttu-id="05aaa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05aaa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05aaa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05aaa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05aaa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="05aaa-118">Optional query parameters</span></span>
<span data-ttu-id="05aaa-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="05aaa-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05aaa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05aaa-120">Request headers</span></span>
|<span data-ttu-id="05aaa-121">标头</span><span class="sxs-lookup"><span data-stu-id="05aaa-121">Header</span></span>|<span data-ttu-id="05aaa-122">值</span><span class="sxs-lookup"><span data-stu-id="05aaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05aaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05aaa-123">Authorization</span></span>|<span data-ttu-id="05aaa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05aaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05aaa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05aaa-125">Accept</span></span>|<span data-ttu-id="05aaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05aaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05aaa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05aaa-127">Request body</span></span>
<span data-ttu-id="05aaa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05aaa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05aaa-129">响应</span><span class="sxs-lookup"><span data-stu-id="05aaa-129">Response</span></span>
<span data-ttu-id="05aaa-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05aaa-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05aaa-131">示例</span><span class="sxs-lookup"><span data-stu-id="05aaa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="05aaa-132">请求</span><span class="sxs-lookup"><span data-stu-id="05aaa-132">Request</span></span>
<span data-ttu-id="05aaa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05aaa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="05aaa-134">响应</span><span class="sxs-lookup"><span data-stu-id="05aaa-134">Response</span></span>
<span data-ttu-id="05aaa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05aaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



