---
title: 获取 windowsKioskConfiguration
description: 读取 windowsKioskConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c2984e881e616d1f404eaf843adf14b29ed845d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132343"
---
# <a name="get-windowskioskconfiguration"></a><span data-ttu-id="d1ba7-103">获取 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1ba7-103">Get windowsKioskConfiguration</span></span>

<span data-ttu-id="d1ba7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1ba7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1ba7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1ba7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1ba7-107">读取 [windowsKioskConfiguration 对象的属性和](../resources/intune-deviceconfig-windowskioskconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-107">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1ba7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1ba7-108">Prerequisites</span></span>
<span data-ttu-id="d1ba7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ba7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1ba7-111">Permission type</span></span>|<span data-ttu-id="d1ba7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1ba7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1ba7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1ba7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1ba7-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ba7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1ba7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1ba7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1ba7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-116">Not supported.</span></span>|
|<span data-ttu-id="d1ba7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1ba7-117">Application</span></span>|<span data-ttu-id="d1ba7-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ba7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1ba7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1ba7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1ba7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1ba7-120">Optional query parameters</span></span>
<span data-ttu-id="d1ba7-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1ba7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1ba7-122">Request headers</span></span>
|<span data-ttu-id="d1ba7-123">标头</span><span class="sxs-lookup"><span data-stu-id="d1ba7-123">Header</span></span>|<span data-ttu-id="d1ba7-124">值</span><span class="sxs-lookup"><span data-stu-id="d1ba7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1ba7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1ba7-125">Authorization</span></span>|<span data-ttu-id="d1ba7-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1ba7-127">接受</span><span class="sxs-lookup"><span data-stu-id="d1ba7-127">Accept</span></span>|<span data-ttu-id="d1ba7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d1ba7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1ba7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1ba7-129">Request body</span></span>
<span data-ttu-id="d1ba7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1ba7-131">响应</span><span class="sxs-lookup"><span data-stu-id="d1ba7-131">Response</span></span>
<span data-ttu-id="d1ba7-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-132">If successful, this method returns a `200 OK` response code and [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1ba7-133">示例</span><span class="sxs-lookup"><span data-stu-id="d1ba7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1ba7-134">请求</span><span class="sxs-lookup"><span data-stu-id="d1ba7-134">Request</span></span>
<span data-ttu-id="d1ba7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d1ba7-136">响应</span><span class="sxs-lookup"><span data-stu-id="d1ba7-136">Response</span></span>
<span data-ttu-id="d1ba7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1ba7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
    "id": "146a990b-990b-146a-0b99-6a140b996a14",
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
    "kioskProfiles": [
      {
        "@odata.type": "microsoft.graph.windowsKioskProfile",
        "profileId": "Profile Id value",
        "profileName": "Profile Name value",
        "appConfiguration": {
          "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
          "apps": [
            {
              "@odata.type": "microsoft.graph.windowsKioskUWPApp",
              "startLayoutTileSize": "small",
              "name": "Name value",
              "appType": "store",
              "autoLaunch": true,
              "appUserModelId": "App User Model Id value",
              "appId": "App Id value",
              "containedAppId": "Contained App Id value"
            }
          ],
          "showTaskBar": true,
          "allowAccessToDownloadsFolder": true,
          "disallowDesktopApps": true,
          "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
        },
        "userAccountsConfiguration": [
          {
            "@odata.type": "microsoft.graph.windowsKioskVisitor"
          }
        ]
      }
    ],
    "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
    "kioskBrowserEnableHomeButton": true,
    "kioskBrowserEnableNavigationButtons": true,
    "kioskBrowserEnableEndSessionButton": true,
    "kioskBrowserRestartOnIdleTimeInMinutes": 6,
    "kioskBrowserBlockedURLs": [
      "Kiosk Browser Blocked URLs value"
    ],
    "kioskBrowserBlockedUrlExceptions": [
      "Kiosk Browser Blocked Url Exceptions value"
    ],
    "edgeKioskEnablePublicBrowsing": true,
    "windowsKioskForceUpdateSchedule": {
      "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "recurrence": "daily",
      "dayofWeek": "monday",
      "dayofMonth": 10,
      "runImmediatelyIfAfterStartDateTime": true
    }
  }
}
```




