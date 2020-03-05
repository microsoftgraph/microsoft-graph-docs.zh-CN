---
title: 列出 macOSGeneralDeviceConfigurations
description: 列出 macOSGeneralDeviceConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7aaa0dbb68c0cf46f67fd9340809e0c4855047b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448751"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="df114-103">列出 macOSGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="df114-103">List macOSGeneralDeviceConfigurations</span></span>

<span data-ttu-id="df114-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="df114-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df114-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df114-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df114-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df114-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df114-107">列出 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df114-107">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df114-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df114-108">Prerequisites</span></span>
<span data-ttu-id="df114-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df114-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df114-111">Permission type</span></span>|<span data-ttu-id="df114-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df114-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df114-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df114-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df114-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df114-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="df114-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df114-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df114-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df114-116">Not supported.</span></span>|
|<span data-ttu-id="df114-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df114-117">Application</span></span>|<span data-ttu-id="df114-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df114-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df114-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df114-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="df114-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df114-120">Request headers</span></span>
|<span data-ttu-id="df114-121">标头</span><span class="sxs-lookup"><span data-stu-id="df114-121">Header</span></span>|<span data-ttu-id="df114-122">值</span><span class="sxs-lookup"><span data-stu-id="df114-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df114-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df114-123">Authorization</span></span>|<span data-ttu-id="df114-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df114-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df114-125">接受</span><span class="sxs-lookup"><span data-stu-id="df114-125">Accept</span></span>|<span data-ttu-id="df114-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df114-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df114-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df114-127">Request body</span></span>
<span data-ttu-id="df114-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df114-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df114-129">响应</span><span class="sxs-lookup"><span data-stu-id="df114-129">Response</span></span>
<span data-ttu-id="df114-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="df114-130">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df114-131">示例</span><span class="sxs-lookup"><span data-stu-id="df114-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df114-132">请求</span><span class="sxs-lookup"><span data-stu-id="df114-132">Request</span></span>
<span data-ttu-id="df114-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df114-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="df114-134">响应</span><span class="sxs-lookup"><span data-stu-id="df114-134">Response</span></span>
<span data-ttu-id="df114-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df114-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3711

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumCharacterSetCount": 0,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "keychainBlockCloudSync": true,
      "airPrintBlocked": true,
      "airPrintForceTrustedTLS": true,
      "airPrintBlockiBeaconDiscovery": true,
      "safariBlockAutofill": true,
      "cameraBlocked": true,
      "iTunesBlockMusicService": true,
      "spotlightBlockInternetResults": true,
      "keyboardBlockDictation": true,
      "definitionLookupBlocked": true,
      "appleWatchBlockAutoUnlock": true,
      "iTunesBlockFileSharing": true,
      "iCloudBlockDocumentSync": true,
      "iCloudBlockMail": true,
      "iCloudBlockAddressBook": true,
      "iCloudBlockCalendar": true,
      "iCloudBlockReminders": true,
      "iCloudBlockBookmarks": true,
      "iCloudBlockNotes": true,
      "airDropBlocked": true,
      "passwordBlockModification": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockAutoFill": true,
      "passwordBlockProximityRequests": true,
      "passwordBlockAirDropSharing": true,
      "softwareUpdatesEnforcedDelayInDays": 2,
      "softwareUpdatesForceDelayed": true,
      "contentCachingBlocked": true,
      "iCloudBlockPhotoLibrary": true,
      "screenCaptureBlocked": true,
      "classroomAppBlockRemoteScreenObservation": true,
      "classroomAppForceUnpromptedScreenObservation": true,
      "classroomForceAutomaticallyJoinClasses": true,
      "classroomForceRequestPermissionToLeaveClasses": true,
      "classroomForceUnpromptedAppAndDeviceLock": true,
      "iCloudBlockActivityContinuation": true
    }
  ]
}
```





