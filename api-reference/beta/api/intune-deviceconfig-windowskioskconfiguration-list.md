---
title: 列出 windowsKioskConfigurations
description: 列出 windowsKioskConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 213d1435cf6268381627a61c7252cce49382d371
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722002"
---
# <a name="list-windowskioskconfigurations"></a><span data-ttu-id="f43d7-103">列出 windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="f43d7-103">List windowsKioskConfigurations</span></span>

> <span data-ttu-id="f43d7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f43d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f43d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f43d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f43d7-106">列出[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f43d7-106">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f43d7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f43d7-107">Prerequisites</span></span>
<span data-ttu-id="f43d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f43d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f43d7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f43d7-110">Permission type</span></span>|<span data-ttu-id="f43d7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f43d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f43d7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f43d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f43d7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f43d7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f43d7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f43d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f43d7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f43d7-115">Not supported.</span></span>|
|<span data-ttu-id="f43d7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f43d7-116">Application</span></span>|<span data-ttu-id="f43d7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f43d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f43d7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f43d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f43d7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f43d7-119">Request headers</span></span>
|<span data-ttu-id="f43d7-120">标头</span><span class="sxs-lookup"><span data-stu-id="f43d7-120">Header</span></span>|<span data-ttu-id="f43d7-121">值</span><span class="sxs-lookup"><span data-stu-id="f43d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f43d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f43d7-122">Authorization</span></span>|<span data-ttu-id="f43d7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f43d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f43d7-124">接受</span><span class="sxs-lookup"><span data-stu-id="f43d7-124">Accept</span></span>|<span data-ttu-id="f43d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f43d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f43d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f43d7-126">Request body</span></span>
<span data-ttu-id="f43d7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f43d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f43d7-128">响应</span><span class="sxs-lookup"><span data-stu-id="f43d7-128">Response</span></span>
<span data-ttu-id="f43d7-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f43d7-129">If successful, this method returns a `200 OK` response code and a collection of [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f43d7-130">示例</span><span class="sxs-lookup"><span data-stu-id="f43d7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f43d7-131">请求</span><span class="sxs-lookup"><span data-stu-id="f43d7-131">Request</span></span>
<span data-ttu-id="f43d7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f43d7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f43d7-133">响应</span><span class="sxs-lookup"><span data-stu-id="f43d7-133">Response</span></span>
<span data-ttu-id="f43d7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f43d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3366

{
  "value": [
    {
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
  ]
}
```





