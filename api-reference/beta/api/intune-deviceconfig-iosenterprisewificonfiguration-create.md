---
title: 创建 iosEnterpriseWiFiConfiguration
description: 创建新的 iosEnterpriseWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79df6dba6a4058b66f97bb95f74feb88a1a2e7b4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151331"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="c5d83-103">创建 iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5d83-103">Create iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="c5d83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5d83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5d83-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5d83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5d83-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5d83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5d83-107">创建新的 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5d83-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5d83-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5d83-108">Prerequisites</span></span>
<span data-ttu-id="c5d83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5d83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5d83-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5d83-111">Permission type</span></span>|<span data-ttu-id="c5d83-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5d83-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5d83-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5d83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5d83-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5d83-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5d83-116">Not supported.</span></span>|
|<span data-ttu-id="c5d83-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5d83-117">Application</span></span>|<span data-ttu-id="c5d83-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d83-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5d83-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5d83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5d83-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5d83-120">Request headers</span></span>
|<span data-ttu-id="c5d83-121">标头</span><span class="sxs-lookup"><span data-stu-id="c5d83-121">Header</span></span>|<span data-ttu-id="c5d83-122">值</span><span class="sxs-lookup"><span data-stu-id="c5d83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5d83-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5d83-123">Authorization</span></span>|<span data-ttu-id="c5d83-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5d83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5d83-125">接受</span><span class="sxs-lookup"><span data-stu-id="c5d83-125">Accept</span></span>|<span data-ttu-id="c5d83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d83-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5d83-127">Request body</span></span>
<span data-ttu-id="c5d83-128">在请求正文中，提供 iosEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5d83-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="c5d83-129">下表显示创建 iosEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5d83-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="c5d83-130">属性</span><span class="sxs-lookup"><span data-stu-id="c5d83-130">Property</span></span>|<span data-ttu-id="c5d83-131">类型</span><span class="sxs-lookup"><span data-stu-id="c5d83-131">Type</span></span>|<span data-ttu-id="c5d83-132">说明</span><span class="sxs-lookup"><span data-stu-id="c5d83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d83-133">id</span><span class="sxs-lookup"><span data-stu-id="c5d83-133">id</span></span>|<span data-ttu-id="c5d83-134">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-134">String</span></span>|<span data-ttu-id="c5d83-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5d83-135">Key of the entity.</span></span> <span data-ttu-id="c5d83-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5d83-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c5d83-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5d83-138">DateTimeOffset</span></span>|<span data-ttu-id="c5d83-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5d83-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c5d83-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5d83-141">roleScopeTagIds</span></span>|<span data-ttu-id="c5d83-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c5d83-142">String collection</span></span>|<span data-ttu-id="c5d83-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c5d83-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5d83-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5d83-145">supportsScopeTags</span></span>|<span data-ttu-id="c5d83-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d83-146">Boolean</span></span>|<span data-ttu-id="c5d83-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c5d83-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5d83-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c5d83-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5d83-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c5d83-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5d83-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c5d83-150">This property is read-only.</span></span> <span data-ttu-id="c5d83-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5d83-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c5d83-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5d83-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c5d83-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c5d83-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c5d83-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5d83-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c5d83-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5d83-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c5d83-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c5d83-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c5d83-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c5d83-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c5d83-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c5d83-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c5d83-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c5d83-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c5d83-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5d83-164">createdDateTime</span></span>|<span data-ttu-id="c5d83-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5d83-165">DateTimeOffset</span></span>|<span data-ttu-id="c5d83-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5d83-166">DateTime the object was created.</span></span> <span data-ttu-id="c5d83-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-168">说明</span><span class="sxs-lookup"><span data-stu-id="c5d83-168">description</span></span>|<span data-ttu-id="c5d83-169">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-169">String</span></span>|<span data-ttu-id="c5d83-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c5d83-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5d83-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d83-172">displayName</span></span>|<span data-ttu-id="c5d83-173">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-173">String</span></span>|<span data-ttu-id="c5d83-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c5d83-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5d83-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-176">version</span><span class="sxs-lookup"><span data-stu-id="c5d83-176">version</span></span>|<span data-ttu-id="c5d83-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c5d83-177">Int32</span></span>|<span data-ttu-id="c5d83-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c5d83-178">Version of the device configuration.</span></span> <span data-ttu-id="c5d83-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-180">networkName</span><span class="sxs-lookup"><span data-stu-id="c5d83-180">networkName</span></span>|<span data-ttu-id="c5d83-181">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-181">String</span></span>|<span data-ttu-id="c5d83-182">网络名称 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-183">ssid</span><span class="sxs-lookup"><span data-stu-id="c5d83-183">ssid</span></span>|<span data-ttu-id="c5d83-184">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-184">String</span></span>|<span data-ttu-id="c5d83-185">这是广播到所有Wi-Fi网络的名称。</span><span class="sxs-lookup"><span data-stu-id="c5d83-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="c5d83-186">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="c5d83-187">connectAutomatically</span></span>|<span data-ttu-id="c5d83-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d83-188">Boolean</span></span>|<span data-ttu-id="c5d83-189">此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="c5d83-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="c5d83-190">如果设置为 true，将跳过用户提示，并自动将设备Wi-Fi网络。</span><span class="sxs-lookup"><span data-stu-id="c5d83-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="c5d83-191">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c5d83-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c5d83-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d83-193">Boolean</span></span>|<span data-ttu-id="c5d83-194">当网络未在 SSID 中广播其名称 (连接) 。</span><span class="sxs-lookup"><span data-stu-id="c5d83-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="c5d83-195">设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="c5d83-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="c5d83-196">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c5d83-197">wiFiSecurityType</span></span>|[<span data-ttu-id="c5d83-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c5d83-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c5d83-199">指示Wi-Fi是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="c5d83-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="c5d83-200">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c5d83-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="c5d83-201">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="c5d83-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c5d83-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="c5d83-202">proxySettings</span></span>|[<span data-ttu-id="c5d83-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="c5d83-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c5d83-204">此连接代理Wi-Fi继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c5d83-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="c5d83-205">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="c5d83-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c5d83-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="c5d83-206">proxyManualAddress</span></span>|<span data-ttu-id="c5d83-207">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-207">String</span></span>|<span data-ttu-id="c5d83-208">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="c5d83-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="c5d83-209">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="c5d83-210">proxyManualPort</span></span>|<span data-ttu-id="c5d83-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c5d83-211">Int32</span></span>|<span data-ttu-id="c5d83-212">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="c5d83-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="c5d83-213">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="c5d83-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c5d83-215">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-215">String</span></span>|<span data-ttu-id="c5d83-216">选择自动配置时代理服务器自动配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="c5d83-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="c5d83-217">此 URL 通常是 PAC 代理自动配置 (文件) 位置。</span><span class="sxs-lookup"><span data-stu-id="c5d83-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="c5d83-218">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-219">disableMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="c5d83-219">disableMacAddressRandomization</span></span>|<span data-ttu-id="c5d83-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d83-220">Boolean</span></span>|<span data-ttu-id="c5d83-221">如果设置为 true，则强制使用此 Wi-Fi 配置文件连接的设备显示其实际的 Wi-Fi MAC 地址，而不是随机 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="c5d83-221">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="c5d83-222">适用于 iOS 14 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c5d83-222">Applies to iOS 14 and later.</span></span> <span data-ttu-id="c5d83-223">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-223">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-224">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="c5d83-224">preSharedKey</span></span>|<span data-ttu-id="c5d83-225">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-225">String</span></span>|<span data-ttu-id="c5d83-226">这是 WPA 个人共享网络的预共享Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="c5d83-226">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="c5d83-227">继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d83-227">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="c5d83-228">eapType</span><span class="sxs-lookup"><span data-stu-id="c5d83-228">eapType</span></span>|[<span data-ttu-id="c5d83-229">eapType</span><span class="sxs-lookup"><span data-stu-id="c5d83-229">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="c5d83-230">可扩展身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="c5d83-230">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="c5d83-231">指示在 Wi-Fi 路由器 (上设置的 EAP) 。</span><span class="sxs-lookup"><span data-stu-id="c5d83-231">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c5d83-232">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="c5d83-232">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="c5d83-233">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5d83-233">eapFastConfiguration</span></span>|[<span data-ttu-id="c5d83-234">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5d83-234">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="c5d83-235">当 EAP-FAST 为所选的 EAP 类型时，EAP-FAST 配置选项。</span><span class="sxs-lookup"><span data-stu-id="c5d83-235">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="c5d83-236">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="c5d83-236">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="c5d83-237">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="c5d83-237">trustedServerCertificateNames</span></span>|<span data-ttu-id="c5d83-238">String collection</span><span class="sxs-lookup"><span data-stu-id="c5d83-238">String collection</span></span>|<span data-ttu-id="c5d83-239">将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="c5d83-239">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="c5d83-240">这是由受信任证书颁发机构颁发给 CA 证书颁发机构颁发的 (名) 。</span><span class="sxs-lookup"><span data-stu-id="c5d83-240">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="c5d83-241">如果提供此信息，则当最终用户连接到此连接网络时，可以绕过显示在最终用户设备上Wi-Fi对话框。</span><span class="sxs-lookup"><span data-stu-id="c5d83-241">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="c5d83-242">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c5d83-242">authenticationMethod</span></span>|[<span data-ttu-id="c5d83-243">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c5d83-243">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c5d83-244">当 EAP 类型配置为 PEAP 或 EAP-TTLS 时身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c5d83-244">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="c5d83-245">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="c5d83-245">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c5d83-246">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="c5d83-246">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="c5d83-247">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="c5d83-247">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c5d83-248">当 EAP 类型为 EAP-TTLS 且 Authentication 方法为 Username 和 Password 时，非 EAP 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c5d83-248">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="c5d83-249">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="c5d83-249">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c5d83-250">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c5d83-250">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c5d83-251">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-251">String</span></span>|<span data-ttu-id="c5d83-252">将 EAP (EAP 类型) EAP - TTLS、EAP - FAST 或 PEAP 时，启用标识隐私和外部标识。</span><span class="sxs-lookup"><span data-stu-id="c5d83-252">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="c5d83-253">此属性会屏蔽输入文本的用户名。</span><span class="sxs-lookup"><span data-stu-id="c5d83-253">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="c5d83-254">例如，如果使用"匿名"，则使用此身份验证的每个用户Wi-Fi其真实用户名进行身份验证的连接将显示为"匿名"。</span><span class="sxs-lookup"><span data-stu-id="c5d83-254">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="c5d83-255">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="c5d83-255">usernameFormatString</span></span>|<span data-ttu-id="c5d83-256">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-256">String</span></span>|<span data-ttu-id="c5d83-257">用于生成要连接到 wifi 的用户名的用户名格式字符串</span><span class="sxs-lookup"><span data-stu-id="c5d83-257">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="c5d83-258">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="c5d83-258">passwordFormatString</span></span>|<span data-ttu-id="c5d83-259">String</span><span class="sxs-lookup"><span data-stu-id="c5d83-259">String</span></span>|<span data-ttu-id="c5d83-260">用于生成用于连接到 wifi 的密码的密码格式字符串</span><span class="sxs-lookup"><span data-stu-id="c5d83-260">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="c5d83-261">响应</span><span class="sxs-lookup"><span data-stu-id="c5d83-261">Response</span></span>
<span data-ttu-id="c5d83-262">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5d83-262">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d83-263">示例</span><span class="sxs-lookup"><span data-stu-id="c5d83-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5d83-264">请求</span><span class="sxs-lookup"><span data-stu-id="c5d83-264">Request</span></span>
<span data-ttu-id="c5d83-265">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5d83-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2017

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="c5d83-266">响应</span><span class="sxs-lookup"><span data-stu-id="c5d83-266">Response</span></span>
<span data-ttu-id="c5d83-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5d83-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2189

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```




