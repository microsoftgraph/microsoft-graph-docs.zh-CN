---
title: 获取 macOSEndpointProtectionConfiguration
description: 读取 macOSEndpointProtectionConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc07594a002b56ee6359f6b14db65d60b6fbe712
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734992"
---
# <a name="get-macosendpointprotectionconfiguration"></a><span data-ttu-id="204c3-103">获取 macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="204c3-103">Get macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="204c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="204c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="204c3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="204c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="204c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="204c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="204c3-107">读取 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="204c3-107">Read properties and relationships of the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="204c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="204c3-108">Prerequisites</span></span>
<span data-ttu-id="204c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="204c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="204c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="204c3-111">Permission type</span></span>|<span data-ttu-id="204c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="204c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="204c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="204c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="204c3-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="204c3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="204c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="204c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="204c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="204c3-116">Not supported.</span></span>|
|<span data-ttu-id="204c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="204c3-117">Application</span></span>|<span data-ttu-id="204c3-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="204c3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="204c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="204c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="204c3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="204c3-120">Optional query parameters</span></span>
<span data-ttu-id="204c3-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="204c3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="204c3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="204c3-122">Request headers</span></span>
|<span data-ttu-id="204c3-123">标头</span><span class="sxs-lookup"><span data-stu-id="204c3-123">Header</span></span>|<span data-ttu-id="204c3-124">值</span><span class="sxs-lookup"><span data-stu-id="204c3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="204c3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="204c3-125">Authorization</span></span>|<span data-ttu-id="204c3-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="204c3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="204c3-127">接受</span><span class="sxs-lookup"><span data-stu-id="204c3-127">Accept</span></span>|<span data-ttu-id="204c3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="204c3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="204c3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="204c3-129">Request body</span></span>
<span data-ttu-id="204c3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="204c3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="204c3-131">响应</span><span class="sxs-lookup"><span data-stu-id="204c3-131">Response</span></span>
<span data-ttu-id="204c3-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="204c3-132">If successful, this method returns a `200 OK` response code and [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="204c3-133">示例</span><span class="sxs-lookup"><span data-stu-id="204c3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="204c3-134">请求</span><span class="sxs-lookup"><span data-stu-id="204c3-134">Request</span></span>
<span data-ttu-id="204c3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="204c3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="204c3-136">响应</span><span class="sxs-lookup"><span data-stu-id="204c3-136">Response</span></span>
<span data-ttu-id="204c3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="204c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3117

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
    "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
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
    "gatekeeperAllowedAppSource": "macAppStore",
    "gatekeeperBlockOverride": true,
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true,
    "firewallApplications": [
      {
        "@odata.type": "microsoft.graph.macOSFirewallApplication",
        "bundleId": "Bundle Id value",
        "allowsIncomingConnections": true
      }
    ],
    "fileVaultEnabled": true,
    "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
    "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
    "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
    "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
    "fileVaultAllowDeferralUntilSignOut": true,
    "fileVaultNumberOfTimesUserCanIgnore": 3,
    "fileVaultDisablePromptAtSignOut": true,
    "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
    "fileVaultHidePersonalRecoveryKey": true,
    "advancedThreatProtectionRealTime": "enabled",
    "advancedThreatProtectionCloudDelivered": "enabled",
    "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
    "advancedThreatProtectionDiagnosticDataCollection": "enabled",
    "advancedThreatProtectionExcludedFolders": [
      "Advanced Threat Protection Excluded Folders value"
    ],
    "advancedThreatProtectionExcludedFiles": [
      "Advanced Threat Protection Excluded Files value"
    ],
    "advancedThreatProtectionExcludedExtensions": [
      "Advanced Threat Protection Excluded Extensions value"
    ],
    "advancedThreatProtectionExcludedProcesses": [
      "Advanced Threat Protection Excluded Processes value"
    ]
  }
}
```





