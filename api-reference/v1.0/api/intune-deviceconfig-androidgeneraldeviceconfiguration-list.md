---
title: 列出 androidGeneralDeviceConfigurations
description: 列出 androidGeneralDeviceConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 005375eea786c946e3d871b0bfd2110db5692a6b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753984"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="a5f08-103">列出 androidGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="a5f08-103">List androidGeneralDeviceConfigurations</span></span>

<span data-ttu-id="a5f08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5f08-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5f08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f08-106">列出 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5f08-106">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5f08-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a5f08-107">Prerequisites</span></span>
<span data-ttu-id="a5f08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f08-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5f08-110">Permission type</span></span>|<span data-ttu-id="a5f08-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5f08-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5f08-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5f08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5f08-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f08-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5f08-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5f08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5f08-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5f08-115">Not supported.</span></span>|
|<span data-ttu-id="a5f08-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5f08-116">Application</span></span>|<span data-ttu-id="a5f08-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f08-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5f08-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5f08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a5f08-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5f08-119">Request headers</span></span>
|<span data-ttu-id="a5f08-120">标头</span><span class="sxs-lookup"><span data-stu-id="a5f08-120">Header</span></span>|<span data-ttu-id="a5f08-121">值</span><span class="sxs-lookup"><span data-stu-id="a5f08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5f08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f08-122">Authorization</span></span>|<span data-ttu-id="a5f08-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a5f08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5f08-124">接受</span><span class="sxs-lookup"><span data-stu-id="a5f08-124">Accept</span></span>|<span data-ttu-id="a5f08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5f08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5f08-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5f08-126">Request body</span></span>
<span data-ttu-id="a5f08-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5f08-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5f08-128">响应</span><span class="sxs-lookup"><span data-stu-id="a5f08-128">Response</span></span>
<span data-ttu-id="a5f08-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a5f08-129">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f08-130">示例</span><span class="sxs-lookup"><span data-stu-id="a5f08-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5f08-131">请求</span><span class="sxs-lookup"><span data-stu-id="a5f08-131">Request</span></span>
<span data-ttu-id="a5f08-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5f08-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a5f08-133">响应</span><span class="sxs-lookup"><span data-stu-id="a5f08-133">Response</span></span>
<span data-ttu-id="a5f08-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5f08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "appsBlockClipboardSharing": true,
      "appsBlockCopyPaste": true,
      "appsBlockYouTube": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockDataRoaming": true,
      "cellularBlockMessaging": true,
      "cellularBlockVoiceRoaming": true,
      "cellularBlockWiFiTethering": true,
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
      "diagnosticDataBlockSubmission": true,
      "locationServicesBlocked": true,
      "googleAccountBlockAutoSync": true,
      "googlePlayStoreBlocked": true,
      "kioskModeBlockSleepButton": true,
      "kioskModeBlockVolumeButtons": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "nfcBlocked": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphabetic",
      "passwordRequired": true,
      "powerOffBlocked": true,
      "factoryResetBlocked": true,
      "screenCaptureBlocked": true,
      "deviceSharingAllowed": true,
      "storageBlockGoogleBackup": true,
      "storageBlockRemovableStorage": true,
      "storageRequireDeviceEncryption": true,
      "storageRequireRemovableStorageEncryption": true,
      "voiceAssistantBlocked": true,
      "voiceDialingBlocked": true,
      "webBrowserBlockPopups": true,
      "webBrowserBlockAutofill": true,
      "webBrowserBlockJavaScript": true,
      "webBrowserBlocked": true,
      "webBrowserCookieSettings": "blockAlways",
      "wiFiBlocked": true,
      "appsInstallAllowList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsLaunchBlockList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsHideList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "securityRequireVerifyApps": true
    }
  ]
}
```




