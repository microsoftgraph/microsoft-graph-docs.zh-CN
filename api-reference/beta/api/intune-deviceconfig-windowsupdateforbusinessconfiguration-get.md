---
title: 获取 windowsUpdateForBusinessConfiguration
description: 读取 windowsUpdateForBusinessConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e80519394842c2f5580f3c08385edbca6aab482b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338208"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="c3c07-103">获取 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3c07-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="c3c07-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3c07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3c07-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3c07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3c07-106">读取 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3c07-106">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3c07-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3c07-107">Prerequisites</span></span>
<span data-ttu-id="c3c07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3c07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3c07-110">Permission type</span></span>|<span data-ttu-id="c3c07-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3c07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3c07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c07-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3c07-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c3c07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3c07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3c07-115">Not supported.</span></span>|
|<span data-ttu-id="c3c07-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3c07-116">Application</span></span>|<span data-ttu-id="c3c07-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3c07-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3c07-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3c07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3c07-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c3c07-119">Optional query parameters</span></span>
<span data-ttu-id="c3c07-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c3c07-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3c07-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3c07-121">Request headers</span></span>
|<span data-ttu-id="c3c07-122">标头</span><span class="sxs-lookup"><span data-stu-id="c3c07-122">Header</span></span>|<span data-ttu-id="c3c07-123">值</span><span class="sxs-lookup"><span data-stu-id="c3c07-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3c07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3c07-124">Authorization</span></span>|<span data-ttu-id="c3c07-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3c07-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3c07-126">接受</span><span class="sxs-lookup"><span data-stu-id="c3c07-126">Accept</span></span>|<span data-ttu-id="c3c07-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3c07-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c07-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3c07-128">Request body</span></span>
<span data-ttu-id="c3c07-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3c07-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3c07-130">响应</span><span class="sxs-lookup"><span data-stu-id="c3c07-130">Response</span></span>
<span data-ttu-id="c3c07-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3c07-131">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3c07-132">示例</span><span class="sxs-lookup"><span data-stu-id="c3c07-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3c07-133">请求</span><span class="sxs-lookup"><span data-stu-id="c3c07-133">Request</span></span>
<span data-ttu-id="c3c07-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3c07-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c3c07-135">响应</span><span class="sxs-lookup"><span data-stu-id="c3c07-135">Response</span></span>
<span data-ttu-id="c3c07-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3c07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3173

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
    "deadlineForFeatureUpdatesInDays": 15,
    "deadlineForQualityUpdatesInDays": 15,
    "deadlineGracePeriodInDays": 9,
    "postponeRebootUntilAfterDeadline": true,
    "autoRestartNotificationDismissal": "automatic",
    "scheduleRestartWarningInHours": 13,
    "scheduleImminentRestartWarningInMinutes": 7,
    "userPauseAccess": "enabled",
    "userWindowsUpdateScanAccess": "enabled",
    "updateNotificationLevel": "defaultNotifications"
  }
}
```






