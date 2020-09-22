---
title: 列出 windows81GeneralConfigurations
description: 列出 windows81GeneralConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4cd83eef41ec8992136c1829ddf95844f26d96c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063231"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="0bb04-103">列出 windows81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="0bb04-103">List windows81GeneralConfigurations</span></span>

<span data-ttu-id="0bb04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bb04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bb04-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0bb04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bb04-106">列出 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0bb04-106">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bb04-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0bb04-107">Prerequisites</span></span>
<span data-ttu-id="0bb04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bb04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bb04-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bb04-110">Permission type</span></span>|<span data-ttu-id="0bb04-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0bb04-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bb04-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb04-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bb04-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bb04-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0bb04-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb04-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bb04-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb04-115">Not supported.</span></span>|
|<span data-ttu-id="0bb04-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bb04-116">Application</span></span>|<span data-ttu-id="0bb04-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb04-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bb04-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bb04-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0bb04-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bb04-119">Request headers</span></span>
|<span data-ttu-id="0bb04-120">标头</span><span class="sxs-lookup"><span data-stu-id="0bb04-120">Header</span></span>|<span data-ttu-id="0bb04-121">值</span><span class="sxs-lookup"><span data-stu-id="0bb04-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bb04-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bb04-122">Authorization</span></span>|<span data-ttu-id="0bb04-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0bb04-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bb04-124">接受</span><span class="sxs-lookup"><span data-stu-id="0bb04-124">Accept</span></span>|<span data-ttu-id="0bb04-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bb04-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bb04-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bb04-126">Request body</span></span>
<span data-ttu-id="0bb04-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0bb04-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bb04-128">响应</span><span class="sxs-lookup"><span data-stu-id="0bb04-128">Response</span></span>
<span data-ttu-id="0bb04-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0bb04-129">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bb04-130">示例</span><span class="sxs-lookup"><span data-stu-id="0bb04-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bb04-131">请求</span><span class="sxs-lookup"><span data-stu-id="0bb04-131">Request</span></span>
<span data-ttu-id="0bb04-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bb04-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0bb04-133">响应</span><span class="sxs-lookup"><span data-stu-id="0bb04-133">Response</span></span>
<span data-ttu-id="0bb04-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bb04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2058

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
      "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "applyOnlyToWindows81": true,
      "browserBlockAutofill": true,
      "browserBlockAutomaticDetectionOfIntranetSites": true,
      "browserBlockEnterpriseModeAccess": true,
      "browserBlockJavaScript": true,
      "browserBlockPlugins": true,
      "browserBlockPopups": true,
      "browserBlockSendingDoNotTrackHeader": true,
      "browserBlockSingleWordEntryOnIntranetSites": true,
      "browserRequireSmartScreen": true,
      "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
      "browserInternetSecurityLevel": "medium",
      "browserIntranetSecurityLevel": "low",
      "browserLoggingReportLocation": "Browser Logging Report Location value",
      "browserRequireHighSecurityForRestrictedSites": true,
      "browserRequireFirewall": true,
      "browserRequireFraudWarning": true,
      "browserTrustedSitesSecurityLevel": "low",
      "cellularBlockDataRoaming": true,
      "diagnosticsBlockDataSubmission": true,
      "passwordBlockPicturePasswordAndPin": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "storageRequireDeviceEncryption": true,
      "updatesRequireAutomaticUpdates": true,
      "userAccountControlSettings": "alwaysNotify",
      "workFoldersUrl": "https://example.com/workFoldersUrl/"
    }
  ]
}
```









