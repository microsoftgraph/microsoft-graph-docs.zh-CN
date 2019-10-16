---
title: 获取 androidWorkProfileGeneralDeviceConfiguration
description: 读取 androidWorkProfileGeneralDeviceConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1326dc5d2e73b6de4782e98c6bbb4b89b4cec02c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534335"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="45b7c-103">获取 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="45b7c-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="45b7c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="45b7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45b7c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45b7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45b7c-106">读取[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="45b7c-106">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45b7c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="45b7c-107">Prerequisites</span></span>
<span data-ttu-id="45b7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45b7c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="45b7c-110">Permission type</span></span>|<span data-ttu-id="45b7c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45b7c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45b7c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45b7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45b7c-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45b7c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45b7c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45b7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45b7c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="45b7c-115">Not supported.</span></span>|
|<span data-ttu-id="45b7c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="45b7c-116">Application</span></span>|<span data-ttu-id="45b7c-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45b7c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45b7c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45b7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45b7c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="45b7c-119">Optional query parameters</span></span>
<span data-ttu-id="45b7c-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="45b7c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45b7c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="45b7c-121">Request headers</span></span>
|<span data-ttu-id="45b7c-122">标头</span><span class="sxs-lookup"><span data-stu-id="45b7c-122">Header</span></span>|<span data-ttu-id="45b7c-123">值</span><span class="sxs-lookup"><span data-stu-id="45b7c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45b7c-124">授权</span><span class="sxs-lookup"><span data-stu-id="45b7c-124">Authorization</span></span>|<span data-ttu-id="45b7c-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45b7c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45b7c-126">接受</span><span class="sxs-lookup"><span data-stu-id="45b7c-126">Accept</span></span>|<span data-ttu-id="45b7c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45b7c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b7c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="45b7c-128">Request body</span></span>
<span data-ttu-id="45b7c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45b7c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45b7c-130">响应</span><span class="sxs-lookup"><span data-stu-id="45b7c-130">Response</span></span>
<span data-ttu-id="45b7c-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="45b7c-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45b7c-132">示例</span><span class="sxs-lookup"><span data-stu-id="45b7c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="45b7c-133">请求</span><span class="sxs-lookup"><span data-stu-id="45b7c-133">Request</span></span>
<span data-ttu-id="45b7c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45b7c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="45b7c-135">响应</span><span class="sxs-lookup"><span data-stu-id="45b7c-135">Response</span></span>
<span data-ttu-id="45b7c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45b7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3248

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true,
    "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
    "vpnEnableAlwaysOnLockdownMode": true,
    "workProfileAllowWidgets": true,
    "workProfileBlockPersonalAppInstallsFromUnknownSources": true
  }
}
```






