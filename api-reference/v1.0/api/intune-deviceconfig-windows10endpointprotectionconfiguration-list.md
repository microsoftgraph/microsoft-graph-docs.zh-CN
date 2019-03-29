---
title: 列出 windows10EndpointProtectionConfigurations
description: 列出 windows10EndpointProtectionConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75e2797027aa87854b5946b336115fae61b43b5d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978897"
---
# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="34859-103">列出 windows10EndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="34859-103">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="34859-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34859-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34859-105">列出 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34859-105">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34859-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="34859-106">Prerequisites</span></span>
<span data-ttu-id="34859-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34859-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="34859-109">Permission type</span></span>|<span data-ttu-id="34859-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34859-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34859-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34859-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34859-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34859-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34859-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34859-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34859-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="34859-114">Not supported.</span></span>|
|<span data-ttu-id="34859-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="34859-115">Application</span></span>|<span data-ttu-id="34859-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34859-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34859-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34859-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34859-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="34859-118">Request headers</span></span>
|<span data-ttu-id="34859-119">标头</span><span class="sxs-lookup"><span data-stu-id="34859-119">Header</span></span>|<span data-ttu-id="34859-120">值</span><span class="sxs-lookup"><span data-stu-id="34859-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34859-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34859-121">Authorization</span></span>|<span data-ttu-id="34859-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34859-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34859-123">接受</span><span class="sxs-lookup"><span data-stu-id="34859-123">Accept</span></span>|<span data-ttu-id="34859-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34859-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34859-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="34859-125">Request body</span></span>
<span data-ttu-id="34859-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34859-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34859-127">响应</span><span class="sxs-lookup"><span data-stu-id="34859-127">Response</span></span>
<span data-ttu-id="34859-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="34859-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34859-129">示例</span><span class="sxs-lookup"><span data-stu-id="34859-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="34859-130">请求</span><span class="sxs-lookup"><span data-stu-id="34859-130">Request</span></span>
<span data-ttu-id="34859-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34859-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="34859-132">响应</span><span class="sxs-lookup"><span data-stu-id="34859-132">Response</span></span>
<span data-ttu-id="34859-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34859-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4834

{
  "value": [
    {
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
  ]
}
```



