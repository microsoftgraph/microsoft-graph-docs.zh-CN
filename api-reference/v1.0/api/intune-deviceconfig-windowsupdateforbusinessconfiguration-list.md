---
title: 列出 windowsUpdateForBusinessConfigurations
description: 列出 windowsUpdateForBusinessConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a9ce0a56d2491c331e7abd74bdbbbab58100f75
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753781"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="f34c2-103">列出 windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="f34c2-103">List windowsUpdateForBusinessConfigurations</span></span>

<span data-ttu-id="f34c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f34c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f34c2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f34c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f34c2-106">列出 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f34c2-106">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f34c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f34c2-107">Prerequisites</span></span>
<span data-ttu-id="f34c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f34c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f34c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f34c2-110">Permission type</span></span>|<span data-ttu-id="f34c2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f34c2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f34c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f34c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f34c2-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f34c2-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f34c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f34c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f34c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f34c2-115">Not supported.</span></span>|
|<span data-ttu-id="f34c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f34c2-116">Application</span></span>|<span data-ttu-id="f34c2-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f34c2-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f34c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f34c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f34c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f34c2-119">Request headers</span></span>
|<span data-ttu-id="f34c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="f34c2-120">Header</span></span>|<span data-ttu-id="f34c2-121">值</span><span class="sxs-lookup"><span data-stu-id="f34c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f34c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f34c2-122">Authorization</span></span>|<span data-ttu-id="f34c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f34c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f34c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="f34c2-124">Accept</span></span>|<span data-ttu-id="f34c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f34c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f34c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f34c2-126">Request body</span></span>
<span data-ttu-id="f34c2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f34c2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f34c2-128">响应</span><span class="sxs-lookup"><span data-stu-id="f34c2-128">Response</span></span>
<span data-ttu-id="f34c2-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f34c2-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f34c2-130">示例</span><span class="sxs-lookup"><span data-stu-id="f34c2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f34c2-131">请求</span><span class="sxs-lookup"><span data-stu-id="f34c2-131">Request</span></span>
<span data-ttu-id="f34c2-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f34c2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f34c2-133">响应</span><span class="sxs-lookup"><span data-stu-id="f34c2-133">Response</span></span>
<span data-ttu-id="f34c2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f34c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




