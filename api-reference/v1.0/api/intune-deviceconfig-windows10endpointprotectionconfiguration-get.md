---
title: 获取 windows10EndpointProtectionConfiguration
description: 读取 windows10EndpointProtectionConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cb138e10a85719d74e78b206ddb40f2d81830ba
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753823"
---
# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="fe344-103">获取 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe344-103">Get windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="fe344-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe344-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe344-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe344-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe344-106">读取 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe344-106">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe344-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe344-107">Prerequisites</span></span>
<span data-ttu-id="fe344-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe344-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe344-110">Permission type</span></span>|<span data-ttu-id="fe344-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe344-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe344-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe344-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe344-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe344-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe344-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe344-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe344-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe344-115">Not supported.</span></span>|
|<span data-ttu-id="fe344-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe344-116">Application</span></span>|<span data-ttu-id="fe344-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe344-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe344-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe344-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe344-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe344-119">Optional query parameters</span></span>
<span data-ttu-id="fe344-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe344-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe344-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe344-121">Request headers</span></span>
|<span data-ttu-id="fe344-122">标头</span><span class="sxs-lookup"><span data-stu-id="fe344-122">Header</span></span>|<span data-ttu-id="fe344-123">值</span><span class="sxs-lookup"><span data-stu-id="fe344-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe344-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe344-124">Authorization</span></span>|<span data-ttu-id="fe344-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe344-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe344-126">接受</span><span class="sxs-lookup"><span data-stu-id="fe344-126">Accept</span></span>|<span data-ttu-id="fe344-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fe344-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe344-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe344-128">Request body</span></span>
<span data-ttu-id="fe344-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe344-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe344-130">响应</span><span class="sxs-lookup"><span data-stu-id="fe344-130">Response</span></span>
<span data-ttu-id="fe344-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe344-131">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe344-132">示例</span><span class="sxs-lookup"><span data-stu-id="fe344-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe344-133">请求</span><span class="sxs-lookup"><span data-stu-id="fe344-133">Request</span></span>
<span data-ttu-id="fe344-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe344-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fe344-135">响应</span><span class="sxs-lookup"><span data-stu-id="fe344-135">Response</span></span>
<span data-ttu-id="fe344-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe344-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4628

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
    "id": "09709403-9403-0970-0394-700903947009",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "firewallBlockStatefulFTP": true,
    "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
    "firewallPreSharedKeyEncodingMethod": "none",
    "firewallIPSecExemptionsAllowNeighborDiscovery": true,
    "firewallIPSecExemptionsAllowICMP": true,
    "firewallIPSecExemptionsAllowRouterDiscovery": true,
    "firewallIPSecExemptionsAllowDHCP": true,
    "firewallCertificateRevocationListCheckMethod": "none",
    "firewallMergeKeyingModuleSettings": true,
    "firewallPacketQueueingMethod": "disabled",
    "firewallProfileDomain": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "firewallProfilePublic": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "firewallProfilePrivate": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "defenderAttackSurfaceReductionExcludedPaths": [
      "Defender Attack Surface Reduction Excluded Paths value"
    ],
    "defenderGuardedFoldersAllowedAppPaths": [
      "Defender Guarded Folders Allowed App Paths value"
    ],
    "defenderAdditionalGuardedFolders": [
      "Defender Additional Guarded Folders value"
    ],
    "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
    "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
    "defenderSecurityCenterBlockExploitProtectionOverride": true,
    "appLockerApplicationControl": "enforceComponentsAndStoreApps",
    "smartScreenEnableInShell": true,
    "smartScreenBlockOverrideForFiles": true,
    "applicationGuardEnabled": true,
    "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
    "applicationGuardBlockNonEnterpriseContent": true,
    "applicationGuardAllowPersistence": true,
    "applicationGuardForceAuditing": true,
    "applicationGuardBlockClipboardSharing": "blockBoth",
    "applicationGuardAllowPrintToPDF": true,
    "applicationGuardAllowPrintToXPS": true,
    "applicationGuardAllowPrintToLocalPrinters": true,
    "applicationGuardAllowPrintToNetworkPrinters": true,
    "bitLockerDisableWarningForOtherDiskEncryption": true,
    "bitLockerEnableStorageCardEncryptionOnMobile": true,
    "bitLockerEncryptDevice": true,
    "bitLockerRemovableDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "blockCrossOrganizationWriteAccess": true
    }
  }
}
```




