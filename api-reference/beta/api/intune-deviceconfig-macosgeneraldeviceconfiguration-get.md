---
title: 获取 macOSGeneralDeviceConfiguration
description: 读取 macOSGeneralDeviceConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c1badb9178e90c08e82fc9314d40ce78424f9d5e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938578"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="c1b41-103">获取 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1b41-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c1b41-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c1b41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1b41-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1b41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1b41-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c1b41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1b41-107">读取 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1b41-107">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1b41-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1b41-108">Prerequisites</span></span>
<span data-ttu-id="c1b41-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c1b41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b41-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1b41-111">Permission type</span></span>|<span data-ttu-id="c1b41-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1b41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b41-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1b41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b41-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1b41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c1b41-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1b41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1b41-116">Not supported.</span></span>|
|<span data-ttu-id="c1b41-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1b41-117">Application</span></span>|<span data-ttu-id="c1b41-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1b41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b41-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1b41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1b41-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1b41-120">Optional query parameters</span></span>
<span data-ttu-id="c1b41-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1b41-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c1b41-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1b41-122">Request headers</span></span>
|<span data-ttu-id="c1b41-123">标头</span><span class="sxs-lookup"><span data-stu-id="c1b41-123">Header</span></span>|<span data-ttu-id="c1b41-124">值</span><span class="sxs-lookup"><span data-stu-id="c1b41-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b41-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1b41-125">Authorization</span></span>|<span data-ttu-id="c1b41-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1b41-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b41-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c1b41-127">Accept</span></span>|<span data-ttu-id="c1b41-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b41-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b41-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1b41-129">Request body</span></span>
<span data-ttu-id="c1b41-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1b41-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1b41-131">响应</span><span class="sxs-lookup"><span data-stu-id="c1b41-131">Response</span></span>
<span data-ttu-id="c1b41-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1b41-132">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b41-133">示例</span><span class="sxs-lookup"><span data-stu-id="c1b41-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1b41-134">请求</span><span class="sxs-lookup"><span data-stu-id="c1b41-134">Request</span></span>
<span data-ttu-id="c1b41-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1b41-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c1b41-136">响应</span><span class="sxs-lookup"><span data-stu-id="c1b41-136">Response</span></span>
<span data-ttu-id="c1b41-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1b41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2054

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
    "passwordBlockFingerprintUnlock": true
  }
}
```





