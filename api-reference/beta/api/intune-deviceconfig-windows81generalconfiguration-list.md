---
title: 列出 windows81GeneralConfigurations
description: 列出 windows81GeneralConfiguration 对象的属性和关系。
ms.openlocfilehash: 09ebff265df940360eb6484be4da94949a975ae0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049020"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="04137-103">列出 windows81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="04137-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="04137-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04137-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04137-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04137-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04137-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04137-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04137-107">列出 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04137-107">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04137-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="04137-108">Prerequisites</span></span>
<span data-ttu-id="04137-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="04137-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04137-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="04137-111">Permission type</span></span>|<span data-ttu-id="04137-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04137-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04137-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04137-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04137-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04137-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="04137-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04137-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04137-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04137-116">Not supported.</span></span>|
|<span data-ttu-id="04137-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="04137-117">Application</span></span>|<span data-ttu-id="04137-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="04137-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04137-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04137-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="04137-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="04137-120">Request headers</span></span>
|<span data-ttu-id="04137-121">标头</span><span class="sxs-lookup"><span data-stu-id="04137-121">Header</span></span>|<span data-ttu-id="04137-122">值</span><span class="sxs-lookup"><span data-stu-id="04137-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04137-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04137-123">Authorization</span></span>|<span data-ttu-id="04137-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04137-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04137-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04137-125">Accept</span></span>|<span data-ttu-id="04137-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04137-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04137-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04137-127">Request body</span></span>
<span data-ttu-id="04137-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04137-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04137-129">响应</span><span class="sxs-lookup"><span data-stu-id="04137-129">Response</span></span>
<span data-ttu-id="04137-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="04137-130">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04137-131">示例</span><span class="sxs-lookup"><span data-stu-id="04137-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="04137-132">请求</span><span class="sxs-lookup"><span data-stu-id="04137-132">Request</span></span>
<span data-ttu-id="04137-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04137-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="04137-134">响应</span><span class="sxs-lookup"><span data-stu-id="04137-134">Response</span></span>
<span data-ttu-id="04137-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04137-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
      "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "minimumAutoInstallClassification": "recommendedAndImportant",
      "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
      "updatesRequireAutomaticUpdates": true,
      "userAccountControlSettings": "alwaysNotify",
      "workFoldersUrl": "https://example.com/workFoldersUrl/"
    }
  ]
}
```





