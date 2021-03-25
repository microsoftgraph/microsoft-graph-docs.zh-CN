---
title: 更新 iosWiFiConfiguration
description: 更新 iosWiFiConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 12b29ee1d8b3c8fc980ea8e4617daa3c20779493
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151233"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="e7f9d-103">更新 iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7f9d-103">Update iosWiFiConfiguration</span></span>

<span data-ttu-id="e7f9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7f9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7f9d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7f9d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7f9d-107">更新 [iosWiFiConfiguration 对象](../resources/intune-deviceconfig-ioswificonfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7f9d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7f9d-108">Prerequisites</span></span>
<span data-ttu-id="e7f9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7f9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7f9d-111">Permission type</span></span>|<span data-ttu-id="e7f9d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7f9d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7f9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7f9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7f9d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7f9d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7f9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7f9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7f9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-116">Not supported.</span></span>|
|<span data-ttu-id="e7f9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7f9d-117">Application</span></span>|<span data-ttu-id="e7f9d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7f9d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7f9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7f9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7f9d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7f9d-120">Request headers</span></span>
|<span data-ttu-id="e7f9d-121">标头</span><span class="sxs-lookup"><span data-stu-id="e7f9d-121">Header</span></span>|<span data-ttu-id="e7f9d-122">值</span><span class="sxs-lookup"><span data-stu-id="e7f9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7f9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7f9d-123">Authorization</span></span>|<span data-ttu-id="e7f9d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7f9d-125">接受</span><span class="sxs-lookup"><span data-stu-id="e7f9d-125">Accept</span></span>|<span data-ttu-id="e7f9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7f9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7f9d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7f9d-127">Request body</span></span>
<span data-ttu-id="e7f9d-128">在请求正文中，提供 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="e7f9d-129">下表显示创建 [iosWiFiConfiguration 时所需的属性](../resources/intune-deviceconfig-ioswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="e7f9d-130">属性</span><span class="sxs-lookup"><span data-stu-id="e7f9d-130">Property</span></span>|<span data-ttu-id="e7f9d-131">类型</span><span class="sxs-lookup"><span data-stu-id="e7f9d-131">Type</span></span>|<span data-ttu-id="e7f9d-132">说明</span><span class="sxs-lookup"><span data-stu-id="e7f9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7f9d-133">id</span><span class="sxs-lookup"><span data-stu-id="e7f9d-133">id</span></span>|<span data-ttu-id="e7f9d-134">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-134">String</span></span>|<span data-ttu-id="e7f9d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-135">Key of the entity.</span></span> <span data-ttu-id="e7f9d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7f9d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e7f9d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7f9d-138">DateTimeOffset</span></span>|<span data-ttu-id="e7f9d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e7f9d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7f9d-141">roleScopeTagIds</span></span>|<span data-ttu-id="e7f9d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e7f9d-142">String collection</span></span>|<span data-ttu-id="e7f9d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7f9d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7f9d-145">supportsScopeTags</span></span>|<span data-ttu-id="e7f9d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7f9d-146">Boolean</span></span>|<span data-ttu-id="e7f9d-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7f9d-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7f9d-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7f9d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-150">This property is read-only.</span></span> <span data-ttu-id="e7f9d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7f9d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e7f9d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7f9d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e7f9d-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e7f9d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7f9d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e7f9d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7f9d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e7f9d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e7f9d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e7f9d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e7f9d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e7f9d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e7f9d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e7f9d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7f9d-164">createdDateTime</span></span>|<span data-ttu-id="e7f9d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7f9d-165">DateTimeOffset</span></span>|<span data-ttu-id="e7f9d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-166">DateTime the object was created.</span></span> <span data-ttu-id="e7f9d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-168">说明</span><span class="sxs-lookup"><span data-stu-id="e7f9d-168">description</span></span>|<span data-ttu-id="e7f9d-169">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-169">String</span></span>|<span data-ttu-id="e7f9d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7f9d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e7f9d-172">displayName</span></span>|<span data-ttu-id="e7f9d-173">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-173">String</span></span>|<span data-ttu-id="e7f9d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7f9d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-176">version</span><span class="sxs-lookup"><span data-stu-id="e7f9d-176">version</span></span>|<span data-ttu-id="e7f9d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f9d-177">Int32</span></span>|<span data-ttu-id="e7f9d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-178">Version of the device configuration.</span></span> <span data-ttu-id="e7f9d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7f9d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7f9d-180">networkName</span><span class="sxs-lookup"><span data-stu-id="e7f9d-180">networkName</span></span>|<span data-ttu-id="e7f9d-181">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-181">String</span></span>|<span data-ttu-id="e7f9d-182">网络名称</span><span class="sxs-lookup"><span data-stu-id="e7f9d-182">Network Name</span></span>|
|<span data-ttu-id="e7f9d-183">ssid</span><span class="sxs-lookup"><span data-stu-id="e7f9d-183">ssid</span></span>|<span data-ttu-id="e7f9d-184">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-184">String</span></span>|<span data-ttu-id="e7f9d-185">这是广播到所有Wi-Fi网络的名称。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="e7f9d-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e7f9d-186">connectAutomatically</span></span>|<span data-ttu-id="e7f9d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7f9d-187">Boolean</span></span>|<span data-ttu-id="e7f9d-188">此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="e7f9d-189">如果设置为 true，将跳过用户提示，并自动将设备Wi-Fi网络。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="e7f9d-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e7f9d-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e7f9d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7f9d-191">Boolean</span></span>|<span data-ttu-id="e7f9d-192">当网络未在 SSID 中广播其名称 (连接) 。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="e7f9d-193">设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="e7f9d-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e7f9d-194">wiFiSecurityType</span></span>|[<span data-ttu-id="e7f9d-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e7f9d-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e7f9d-196">指示Wi-Fi是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="e7f9d-197">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e7f9d-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="e7f9d-198">proxySettings</span></span>|[<span data-ttu-id="e7f9d-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e7f9d-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e7f9d-200">此连接代理Wi-Fi类型。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="e7f9d-201">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e7f9d-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e7f9d-202">proxyManualAddress</span></span>|<span data-ttu-id="e7f9d-203">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-203">String</span></span>|<span data-ttu-id="e7f9d-204">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e7f9d-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e7f9d-205">proxyManualPort</span></span>|<span data-ttu-id="e7f9d-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f9d-206">Int32</span></span>|<span data-ttu-id="e7f9d-207">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e7f9d-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e7f9d-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e7f9d-209">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-209">String</span></span>|<span data-ttu-id="e7f9d-210">选择自动配置时代理服务器自动配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="e7f9d-211">此 URL 通常是 PAC 代理自动配置 (文件) 位置。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="e7f9d-212">disableMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="e7f9d-212">disableMacAddressRandomization</span></span>|<span data-ttu-id="e7f9d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7f9d-213">Boolean</span></span>|<span data-ttu-id="e7f9d-214">如果设置为 true，则强制使用此 Wi-Fi 配置文件连接的设备显示其实际的 Wi-Fi MAC 地址，而不是随机 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-214">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="e7f9d-215">适用于 iOS 14 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-215">Applies to iOS 14 and later.</span></span>|
|<span data-ttu-id="e7f9d-216">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e7f9d-216">preSharedKey</span></span>|<span data-ttu-id="e7f9d-217">String</span><span class="sxs-lookup"><span data-stu-id="e7f9d-217">String</span></span>|<span data-ttu-id="e7f9d-218">这是 WPA 个人共享网络的预共享Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-218">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="e7f9d-219">响应</span><span class="sxs-lookup"><span data-stu-id="e7f9d-219">Response</span></span>
<span data-ttu-id="e7f9d-220">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-220">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7f9d-221">示例</span><span class="sxs-lookup"><span data-stu-id="e7f9d-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7f9d-222">请求</span><span class="sxs-lookup"><span data-stu-id="e7f9d-222">Request</span></span>
<span data-ttu-id="e7f9d-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="e7f9d-224">响应</span><span class="sxs-lookup"><span data-stu-id="e7f9d-224">Response</span></span>
<span data-ttu-id="e7f9d-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7f9d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "preSharedKey": "Pre Shared Key value"
}
```




