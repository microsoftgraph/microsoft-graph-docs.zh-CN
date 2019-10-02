---
title: 列出 windowsUpdateForBusinessConfigurations
description: 列出 windowsUpdateForBusinessConfiguration 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa81636535a0754409a242b3868ddd7bf4301427
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364667"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="abcb3-103">列出 windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="abcb3-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="abcb3-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abcb3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abcb3-105">列出 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="abcb3-105">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abcb3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="abcb3-106">Prerequisites</span></span>
<span data-ttu-id="abcb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abcb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abcb3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="abcb3-109">Permission type</span></span>|<span data-ttu-id="abcb3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="abcb3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abcb3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abcb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="abcb3-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="abcb3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="abcb3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abcb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abcb3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="abcb3-114">Not supported.</span></span>|
|<span data-ttu-id="abcb3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="abcb3-115">Application</span></span>|<span data-ttu-id="abcb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="abcb3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abcb3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abcb3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="abcb3-118">请求头</span><span class="sxs-lookup"><span data-stu-id="abcb3-118">Request headers</span></span>
|<span data-ttu-id="abcb3-119">标头</span><span class="sxs-lookup"><span data-stu-id="abcb3-119">Header</span></span>|<span data-ttu-id="abcb3-120">值</span><span class="sxs-lookup"><span data-stu-id="abcb3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abcb3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abcb3-121">Authorization</span></span>|<span data-ttu-id="abcb3-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="abcb3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abcb3-123">接受</span><span class="sxs-lookup"><span data-stu-id="abcb3-123">Accept</span></span>|<span data-ttu-id="abcb3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="abcb3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abcb3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="abcb3-125">Request body</span></span>
<span data-ttu-id="abcb3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="abcb3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abcb3-127">响应</span><span class="sxs-lookup"><span data-stu-id="abcb3-127">Response</span></span>
<span data-ttu-id="abcb3-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="abcb3-128">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abcb3-129">示例</span><span class="sxs-lookup"><span data-stu-id="abcb3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="abcb3-130">请求</span><span class="sxs-lookup"><span data-stu-id="abcb3-130">Request</span></span>
<span data-ttu-id="abcb3-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abcb3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="abcb3-132">响应</span><span class="sxs-lookup"><span data-stu-id="abcb3-132">Response</span></span>
<span data-ttu-id="abcb3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="abcb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "value": [
    {
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
  ]
}
```




