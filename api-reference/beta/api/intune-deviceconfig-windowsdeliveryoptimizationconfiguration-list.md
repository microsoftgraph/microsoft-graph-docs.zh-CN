---
title: 列出 windowsDeliveryOptimizationConfigurations
description: 列出 windowsDeliveryOptimizationConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01fb15d2270b32d357b10346399e9254dc85b39a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917987"
---
# <a name="list-windowsdeliveryoptimizationconfigurations"></a><span data-ttu-id="a2552-103">列出 windowsDeliveryOptimizationConfigurations</span><span class="sxs-lookup"><span data-stu-id="a2552-103">List windowsDeliveryOptimizationConfigurations</span></span>

> <span data-ttu-id="a2552-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2552-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2552-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2552-106">列出[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2552-106">List properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2552-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2552-107">Prerequisites</span></span>
<span data-ttu-id="a2552-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2552-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2552-110">Permission type</span></span>|<span data-ttu-id="a2552-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2552-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2552-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2552-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2552-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2552-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2552-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2552-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2552-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2552-115">Not supported.</span></span>|
|<span data-ttu-id="a2552-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2552-116">Application</span></span>|<span data-ttu-id="a2552-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2552-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2552-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2552-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2552-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2552-119">Request headers</span></span>
|<span data-ttu-id="a2552-120">标头</span><span class="sxs-lookup"><span data-stu-id="a2552-120">Header</span></span>|<span data-ttu-id="a2552-121">值</span><span class="sxs-lookup"><span data-stu-id="a2552-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2552-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2552-122">Authorization</span></span>|<span data-ttu-id="a2552-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2552-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2552-124">接受</span><span class="sxs-lookup"><span data-stu-id="a2552-124">Accept</span></span>|<span data-ttu-id="a2552-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2552-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2552-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2552-126">Request body</span></span>
<span data-ttu-id="a2552-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2552-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2552-128">响应</span><span class="sxs-lookup"><span data-stu-id="a2552-128">Response</span></span>
<span data-ttu-id="a2552-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2552-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2552-130">示例</span><span class="sxs-lookup"><span data-stu-id="a2552-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2552-131">请求</span><span class="sxs-lookup"><span data-stu-id="a2552-131">Request</span></span>
<span data-ttu-id="a2552-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2552-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a2552-133">响应</span><span class="sxs-lookup"><span data-stu-id="a2552-133">Response</span></span>
<span data-ttu-id="a2552-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1389

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
      "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "deliveryOptimizationMode": "httpOnly",
      "restrictPeerSelectionBy": "subnetMask",
      "groupIdSource": {
        "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
      },
      "bandwidthMode": {
        "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
      },
      "backgroundDownloadFromHttpDelayInSeconds": 8,
      "foregroundDownloadFromHttpDelayInSeconds": 8,
      "minimumRamAllowedToPeerInGigabytes": 2,
      "minimumDiskSizeAllowedToPeerInGigabytes": 7,
      "minimumFileSizeToCacheInMegabytes": 1,
      "minimumBatteryPercentageAllowedToUpload": 7,
      "modifyCacheLocation": "Modify Cache Location value",
      "maximumCacheAgeInDays": 5,
      "maximumCacheSize": {
        "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
      },
      "vpnPeerCaching": "enabled"
    }
  ]
}
```




