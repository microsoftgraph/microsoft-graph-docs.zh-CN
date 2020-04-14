---
title: 获取 windowsDeliveryOptimizationConfiguration
description: 读取 windowsDeliveryOptimizationConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18bc1c7f38e8362d036e32433db4b42e808ba84a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43429699"
---
# <a name="get-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="69b63-103">获取 windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="69b63-103">Get windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="69b63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69b63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69b63-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69b63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69b63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69b63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69b63-107">读取[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69b63-107">Read properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69b63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69b63-108">Prerequisites</span></span>
<span data-ttu-id="69b63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69b63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69b63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69b63-111">Permission type</span></span>|<span data-ttu-id="69b63-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69b63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69b63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69b63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69b63-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69b63-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69b63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69b63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69b63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69b63-116">Not supported.</span></span>|
|<span data-ttu-id="69b63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69b63-117">Application</span></span>|<span data-ttu-id="69b63-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69b63-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69b63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69b63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69b63-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69b63-120">Optional query parameters</span></span>
<span data-ttu-id="69b63-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69b63-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69b63-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="69b63-122">Request headers</span></span>
|<span data-ttu-id="69b63-123">标头</span><span class="sxs-lookup"><span data-stu-id="69b63-123">Header</span></span>|<span data-ttu-id="69b63-124">值</span><span class="sxs-lookup"><span data-stu-id="69b63-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69b63-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="69b63-125">Authorization</span></span>|<span data-ttu-id="69b63-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69b63-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69b63-127">接受</span><span class="sxs-lookup"><span data-stu-id="69b63-127">Accept</span></span>|<span data-ttu-id="69b63-128">application/json</span><span class="sxs-lookup"><span data-stu-id="69b63-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69b63-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="69b63-129">Request body</span></span>
<span data-ttu-id="69b63-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69b63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69b63-131">响应</span><span class="sxs-lookup"><span data-stu-id="69b63-131">Response</span></span>
<span data-ttu-id="69b63-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69b63-132">If successful, this method returns a `200 OK` response code and [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69b63-133">示例</span><span class="sxs-lookup"><span data-stu-id="69b63-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="69b63-134">请求</span><span class="sxs-lookup"><span data-stu-id="69b63-134">Request</span></span>
<span data-ttu-id="69b63-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69b63-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="69b63-136">响应</span><span class="sxs-lookup"><span data-stu-id="69b63-136">Response</span></span>
<span data-ttu-id="69b63-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69b63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2344

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
    "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
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
    "vpnPeerCaching": "enabled",
    "cacheServerHostNames": [
      "Cache Server Host Names value"
    ],
    "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
    "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
  }
}
```



