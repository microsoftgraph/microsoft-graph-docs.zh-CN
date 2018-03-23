# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="9bebf-101">列出 windows10EndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="9bebf-101">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="9bebf-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9bebf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bebf-103">列出 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9bebf-103">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9bebf-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="9bebf-104">Prerequisites</span></span>
<span data-ttu-id="9bebf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9bebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9bebf-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bebf-107">Permission type</span></span>|<span data-ttu-id="9bebf-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9bebf-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bebf-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bebf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9bebf-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bebf-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9bebf-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bebf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bebf-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bebf-112">Not supported.</span></span>|
|<span data-ttu-id="9bebf-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bebf-113">Application</span></span>|<span data-ttu-id="9bebf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bebf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bebf-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bebf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9bebf-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bebf-116">Request headers</span></span>
|<span data-ttu-id="9bebf-117">标头</span><span class="sxs-lookup"><span data-stu-id="9bebf-117">Header</span></span>|<span data-ttu-id="9bebf-118">值</span><span class="sxs-lookup"><span data-stu-id="9bebf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bebf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bebf-119">Authorization</span></span>|<span data-ttu-id="9bebf-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9bebf-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9bebf-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9bebf-121">Accept</span></span>|<span data-ttu-id="9bebf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9bebf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bebf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bebf-123">Request body</span></span>
<span data-ttu-id="9bebf-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9bebf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bebf-125">响应</span><span class="sxs-lookup"><span data-stu-id="9bebf-125">Response</span></span>
<span data-ttu-id="9bebf-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9bebf-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bebf-127">示例</span><span class="sxs-lookup"><span data-stu-id="9bebf-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bebf-128">请求</span><span class="sxs-lookup"><span data-stu-id="9bebf-128">Request</span></span>
<span data-ttu-id="9bebf-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bebf-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9bebf-130">响应</span><span class="sxs-lookup"><span data-stu-id="9bebf-130">Response</span></span>
<span data-ttu-id="9bebf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bebf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



