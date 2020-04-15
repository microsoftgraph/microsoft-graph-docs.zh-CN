---
title: 获取 androidGeneralDeviceConfiguration
description: 读取 androidGeneralDeviceConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a419d1698e3505f6e90908ba78d34b1a7aa5673e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474637"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="32293-103">获取 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="32293-103">Get androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="32293-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32293-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32293-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32293-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32293-106">读取 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="32293-106">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32293-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="32293-107">Prerequisites</span></span>
<span data-ttu-id="32293-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32293-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32293-110">Permission type</span></span>|<span data-ttu-id="32293-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32293-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32293-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32293-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32293-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="32293-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="32293-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32293-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32293-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32293-115">Not supported.</span></span>|
|<span data-ttu-id="32293-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32293-116">Application</span></span>|<span data-ttu-id="32293-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="32293-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32293-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32293-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32293-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="32293-119">Optional query parameters</span></span>
<span data-ttu-id="32293-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="32293-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32293-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="32293-121">Request headers</span></span>
|<span data-ttu-id="32293-122">标头</span><span class="sxs-lookup"><span data-stu-id="32293-122">Header</span></span>|<span data-ttu-id="32293-123">值</span><span class="sxs-lookup"><span data-stu-id="32293-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32293-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="32293-124">Authorization</span></span>|<span data-ttu-id="32293-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32293-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32293-126">接受</span><span class="sxs-lookup"><span data-stu-id="32293-126">Accept</span></span>|<span data-ttu-id="32293-127">application/json</span><span class="sxs-lookup"><span data-stu-id="32293-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32293-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="32293-128">Request body</span></span>
<span data-ttu-id="32293-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32293-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32293-130">响应</span><span class="sxs-lookup"><span data-stu-id="32293-130">Response</span></span>
<span data-ttu-id="32293-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32293-131">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32293-132">示例</span><span class="sxs-lookup"><span data-stu-id="32293-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="32293-133">请求</span><span class="sxs-lookup"><span data-stu-id="32293-133">Request</span></span>
<span data-ttu-id="32293-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32293-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="32293-135">响应</span><span class="sxs-lookup"><span data-stu-id="32293-135">Response</span></span>
<span data-ttu-id="32293-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32293-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3414

{
  "value": {
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
}
```






