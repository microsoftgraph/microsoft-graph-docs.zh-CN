---
title: 列出 windowsUpdateForBusinessConfigurations
description: 列出 windowsUpdateForBusinessConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88a27d29ec61e70c239ebdf17c993fdd91aaf1d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153261"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="9e9db-103">列出 windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="9e9db-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="9e9db-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e9db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e9db-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e9db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e9db-106">列出 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e9db-106">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e9db-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e9db-107">Prerequisites</span></span>
<span data-ttu-id="9e9db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9e9db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e9db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e9db-110">Permission type</span></span>|<span data-ttu-id="9e9db-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e9db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e9db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e9db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e9db-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e9db-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e9db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e9db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e9db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e9db-115">Not supported.</span></span>|
|<span data-ttu-id="9e9db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e9db-116">Application</span></span>|<span data-ttu-id="9e9db-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e9db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e9db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e9db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e9db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e9db-119">Request headers</span></span>
|<span data-ttu-id="9e9db-120">标头</span><span class="sxs-lookup"><span data-stu-id="9e9db-120">Header</span></span>|<span data-ttu-id="9e9db-121">值</span><span class="sxs-lookup"><span data-stu-id="9e9db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e9db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e9db-122">Authorization</span></span>|<span data-ttu-id="9e9db-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e9db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e9db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9e9db-124">Accept</span></span>|<span data-ttu-id="9e9db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e9db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e9db-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e9db-126">Request body</span></span>
<span data-ttu-id="9e9db-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e9db-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e9db-128">响应</span><span class="sxs-lookup"><span data-stu-id="9e9db-128">Response</span></span>
<span data-ttu-id="9e9db-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9e9db-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e9db-130">示例</span><span class="sxs-lookup"><span data-stu-id="9e9db-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e9db-131">请求</span><span class="sxs-lookup"><span data-stu-id="9e9db-131">Request</span></span>
<span data-ttu-id="9e9db-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e9db-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9e9db-133">响应</span><span class="sxs-lookup"><span data-stu-id="9e9db-133">Response</span></span>
<span data-ttu-id="9e9db-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e9db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2185

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
      "businessReadyUpdatesOnly": "all",
      "skipChecksBeforeRestart": true,
      "updateWeeks": "firstWeek",
      "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
      "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
      "featureUpdatesRollbackWindowInDays": 2,
      "qualityUpdatesWillBeRolledBack": true,
      "featureUpdatesWillBeRolledBack": true,
      "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
      "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
      "engagedRestartDeadlineInDays": 12,
      "engagedRestartSnoozeScheduleInDays": 2,
      "engagedRestartTransitionScheduleInDays": 6,
      "autoRestartNotificationDismissal": "automatic",
      "scheduleRestartWarningInHours": 13,
      "scheduleImminentRestartWarningInMinutes": 7,
      "userPauseAccess": "enabled"
    }
  ]
}
```




