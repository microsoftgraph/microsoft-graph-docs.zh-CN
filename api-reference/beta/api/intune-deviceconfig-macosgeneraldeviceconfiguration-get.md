---
title: 获取 macOSGeneralDeviceConfiguration
description: 读取 macOSGeneralDeviceConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2015ce6568bf0f58a29185ab56ea7c1facd6611
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981284"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="37ef3-103">获取 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="37ef3-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="37ef3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37ef3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37ef3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37ef3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37ef3-106">读取 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="37ef3-106">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37ef3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="37ef3-107">Prerequisites</span></span>
<span data-ttu-id="37ef3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37ef3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="37ef3-110">Permission type</span></span>|<span data-ttu-id="37ef3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37ef3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37ef3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37ef3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37ef3-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37ef3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="37ef3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37ef3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37ef3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="37ef3-115">Not supported.</span></span>|
|<span data-ttu-id="37ef3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="37ef3-116">Application</span></span>|<span data-ttu-id="37ef3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="37ef3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37ef3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37ef3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37ef3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="37ef3-119">Optional query parameters</span></span>
<span data-ttu-id="37ef3-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37ef3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37ef3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="37ef3-121">Request headers</span></span>
|<span data-ttu-id="37ef3-122">标头</span><span class="sxs-lookup"><span data-stu-id="37ef3-122">Header</span></span>|<span data-ttu-id="37ef3-123">值</span><span class="sxs-lookup"><span data-stu-id="37ef3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37ef3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="37ef3-124">Authorization</span></span>|<span data-ttu-id="37ef3-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37ef3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37ef3-126">接受</span><span class="sxs-lookup"><span data-stu-id="37ef3-126">Accept</span></span>|<span data-ttu-id="37ef3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="37ef3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37ef3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="37ef3-128">Request body</span></span>
<span data-ttu-id="37ef3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37ef3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37ef3-130">响应</span><span class="sxs-lookup"><span data-stu-id="37ef3-130">Response</span></span>
<span data-ttu-id="37ef3-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37ef3-131">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37ef3-132">示例</span><span class="sxs-lookup"><span data-stu-id="37ef3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="37ef3-133">请求</span><span class="sxs-lookup"><span data-stu-id="37ef3-133">Request</span></span>
<span data-ttu-id="37ef3-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37ef3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="37ef3-135">响应</span><span class="sxs-lookup"><span data-stu-id="37ef3-135">Response</span></span>
<span data-ttu-id="37ef3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37ef3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2301

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "contentCachingBlocked": true
  }
}
```




