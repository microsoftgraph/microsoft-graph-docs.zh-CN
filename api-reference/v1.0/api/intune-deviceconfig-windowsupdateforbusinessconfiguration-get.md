---
title: 获取 windowsUpdateForBusinessConfiguration
description: 读取 windowsUpdateForBusinessConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a7e9344ae8550bcc1992ba24d24fd94dff3821c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991018"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="d5e30-103">获取 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5e30-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="d5e30-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d5e30-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5e30-105">读取 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5e30-105">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5e30-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5e30-106">Prerequisites</span></span>
<span data-ttu-id="d5e30-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d5e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5e30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5e30-109">Permission type</span></span>|<span data-ttu-id="d5e30-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5e30-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5e30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5e30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5e30-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5e30-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5e30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5e30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5e30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5e30-114">Not supported.</span></span>|
|<span data-ttu-id="d5e30-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5e30-115">Application</span></span>|<span data-ttu-id="d5e30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5e30-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5e30-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5e30-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5e30-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5e30-118">Optional query parameters</span></span>
<span data-ttu-id="d5e30-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5e30-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d5e30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5e30-120">Request headers</span></span>
|<span data-ttu-id="d5e30-121">标头</span><span class="sxs-lookup"><span data-stu-id="d5e30-121">Header</span></span>|<span data-ttu-id="d5e30-122">值</span><span class="sxs-lookup"><span data-stu-id="d5e30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5e30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5e30-123">Authorization</span></span>|<span data-ttu-id="d5e30-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5e30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5e30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5e30-125">Accept</span></span>|<span data-ttu-id="d5e30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5e30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5e30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5e30-127">Request body</span></span>
<span data-ttu-id="d5e30-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5e30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5e30-129">响应</span><span class="sxs-lookup"><span data-stu-id="d5e30-129">Response</span></span>
<span data-ttu-id="d5e30-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5e30-130">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5e30-131">示例</span><span class="sxs-lookup"><span data-stu-id="d5e30-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5e30-132">请求</span><span class="sxs-lookup"><span data-stu-id="d5e30-132">Request</span></span>
<span data-ttu-id="d5e30-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5e30-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d5e30-134">响应</span><span class="sxs-lookup"><span data-stu-id="d5e30-134">Response</span></span>
<span data-ttu-id="d5e30-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5e30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1149

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "deliveryOptimizationMode": "httpOnly",
    "prereleaseFeatures": "settingsOnly",
    "automaticUpdateMode": "notifyDownload",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
      "scheduledInstallDay": "everyday",
      "scheduledInstallTime": "11:59:31.3170000"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
    "businessReadyUpdatesOnly": "all"
  }
}
```



