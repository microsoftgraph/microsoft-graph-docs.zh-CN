---
title: 获取 windows81GeneralConfiguration
description: 读取 windows81GeneralConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7bf197363579dcf07e5c62252503f6358ccb81b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753802"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="a06d6-103">获取 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a06d6-103">Get windows81GeneralConfiguration</span></span>

<span data-ttu-id="a06d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a06d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a06d6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a06d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a06d6-106">读取 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a06d6-106">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a06d6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a06d6-107">Prerequisites</span></span>
<span data-ttu-id="a06d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a06d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a06d6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a06d6-110">Permission type</span></span>|<span data-ttu-id="a06d6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a06d6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a06d6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a06d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a06d6-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a06d6-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a06d6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a06d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a06d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a06d6-115">Not supported.</span></span>|
|<span data-ttu-id="a06d6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a06d6-116">Application</span></span>|<span data-ttu-id="a06d6-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a06d6-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a06d6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a06d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a06d6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a06d6-119">Optional query parameters</span></span>
<span data-ttu-id="a06d6-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a06d6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a06d6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a06d6-121">Request headers</span></span>
|<span data-ttu-id="a06d6-122">标头</span><span class="sxs-lookup"><span data-stu-id="a06d6-122">Header</span></span>|<span data-ttu-id="a06d6-123">值</span><span class="sxs-lookup"><span data-stu-id="a06d6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a06d6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a06d6-124">Authorization</span></span>|<span data-ttu-id="a06d6-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a06d6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a06d6-126">接受</span><span class="sxs-lookup"><span data-stu-id="a06d6-126">Accept</span></span>|<span data-ttu-id="a06d6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a06d6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a06d6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a06d6-128">Request body</span></span>
<span data-ttu-id="a06d6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a06d6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a06d6-130">响应</span><span class="sxs-lookup"><span data-stu-id="a06d6-130">Response</span></span>
<span data-ttu-id="a06d6-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a06d6-131">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a06d6-132">示例</span><span class="sxs-lookup"><span data-stu-id="a06d6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a06d6-133">请求</span><span class="sxs-lookup"><span data-stu-id="a06d6-133">Request</span></span>
<span data-ttu-id="a06d6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a06d6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a06d6-135">响应</span><span class="sxs-lookup"><span data-stu-id="a06d6-135">Response</span></span>
<span data-ttu-id="a06d6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a06d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
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
}
```




