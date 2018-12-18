---
title: 获取 windows81GeneralConfiguration
description: 读取 windows81GeneralConfiguration 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: fd35bee5e035317dd67b3eb2bb0ec20676e9a4d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354017"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="0904d-103">获取 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="0904d-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="0904d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0904d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0904d-105">读取 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0904d-105">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0904d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0904d-106">Prerequisites</span></span>
<span data-ttu-id="0904d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0904d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0904d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0904d-109">Permission type</span></span>|<span data-ttu-id="0904d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0904d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0904d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0904d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0904d-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0904d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0904d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0904d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0904d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0904d-114">Not supported.</span></span>|
|<span data-ttu-id="0904d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0904d-115">Application</span></span>|<span data-ttu-id="0904d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0904d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0904d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0904d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0904d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0904d-118">Optional query parameters</span></span>
<span data-ttu-id="0904d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0904d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0904d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0904d-120">Request headers</span></span>
|<span data-ttu-id="0904d-121">标头</span><span class="sxs-lookup"><span data-stu-id="0904d-121">Header</span></span>|<span data-ttu-id="0904d-122">值</span><span class="sxs-lookup"><span data-stu-id="0904d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0904d-123">授权</span><span class="sxs-lookup"><span data-stu-id="0904d-123">Authorization</span></span>|<span data-ttu-id="0904d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0904d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0904d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0904d-125">Accept</span></span>|<span data-ttu-id="0904d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0904d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0904d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0904d-127">Request body</span></span>
<span data-ttu-id="0904d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0904d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0904d-129">响应</span><span class="sxs-lookup"><span data-stu-id="0904d-129">Response</span></span>
<span data-ttu-id="0904d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0904d-130">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0904d-131">示例</span><span class="sxs-lookup"><span data-stu-id="0904d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0904d-132">请求</span><span class="sxs-lookup"><span data-stu-id="0904d-132">Request</span></span>
<span data-ttu-id="0904d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0904d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0904d-134">响应</span><span class="sxs-lookup"><span data-stu-id="0904d-134">Response</span></span>
<span data-ttu-id="0904d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0904d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



