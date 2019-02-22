---
title: 创建 macOSEnterpriseWiFiConfiguration
description: 创建新的 macOSEnterpriseWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e618ff2fbfaef8127c4b1d36dc2dbd45b473a74
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143286"
---
# <a name="create-macosenterprisewificonfiguration"></a><span data-ttu-id="0e12e-103">创建 macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e12e-103">Create macOSEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="0e12e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e12e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e12e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e12e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e12e-106">创建新的[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e12e-106">Create a new [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e12e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e12e-107">Prerequisites</span></span>
<span data-ttu-id="0e12e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0e12e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e12e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e12e-110">Permission type</span></span>|<span data-ttu-id="0e12e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e12e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e12e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e12e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e12e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e12e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e12e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e12e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e12e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e12e-115">Not supported.</span></span>|
|<span data-ttu-id="0e12e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e12e-116">Application</span></span>|<span data-ttu-id="0e12e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e12e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e12e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e12e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0e12e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e12e-119">Request headers</span></span>
|<span data-ttu-id="0e12e-120">标头</span><span class="sxs-lookup"><span data-stu-id="0e12e-120">Header</span></span>|<span data-ttu-id="0e12e-121">值</span><span class="sxs-lookup"><span data-stu-id="0e12e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e12e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e12e-122">Authorization</span></span>|<span data-ttu-id="0e12e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e12e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e12e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e12e-124">Accept</span></span>|<span data-ttu-id="0e12e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e12e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e12e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e12e-126">Request body</span></span>
<span data-ttu-id="0e12e-127">在请求正文中, 提供 macOSEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e12e-127">In the request body, supply a JSON representation for the macOSEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="0e12e-128">下表显示创建 macOSEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e12e-128">The following table shows the properties that are required when you create the macOSEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="0e12e-129">属性</span><span class="sxs-lookup"><span data-stu-id="0e12e-129">Property</span></span>|<span data-ttu-id="0e12e-130">类型</span><span class="sxs-lookup"><span data-stu-id="0e12e-130">Type</span></span>|<span data-ttu-id="0e12e-131">说明</span><span class="sxs-lookup"><span data-stu-id="0e12e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e12e-132">id</span><span class="sxs-lookup"><span data-stu-id="0e12e-132">id</span></span>|<span data-ttu-id="0e12e-133">String</span><span class="sxs-lookup"><span data-stu-id="0e12e-133">String</span></span>|<span data-ttu-id="0e12e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0e12e-134">Key of the entity.</span></span> <span data-ttu-id="0e12e-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e12e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0e12e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e12e-137">DateTimeOffset</span></span>|<span data-ttu-id="0e12e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0e12e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0e12e-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e12e-140">roleScopeTagIds</span></span>|<span data-ttu-id="0e12e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0e12e-141">String collection</span></span>|<span data-ttu-id="0e12e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0e12e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e12e-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0e12e-144">supportsScopeTags</span></span>|<span data-ttu-id="0e12e-145">布尔</span><span class="sxs-lookup"><span data-stu-id="0e12e-145">Boolean</span></span>|<span data-ttu-id="0e12e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0e12e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e12e-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0e12e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e12e-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0e12e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e12e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0e12e-149">This property is read-only.</span></span> <span data-ttu-id="0e12e-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e12e-151">createdDateTime</span></span>|<span data-ttu-id="0e12e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e12e-152">DateTimeOffset</span></span>|<span data-ttu-id="0e12e-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0e12e-153">DateTime the object was created.</span></span> <span data-ttu-id="0e12e-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-155">description</span><span class="sxs-lookup"><span data-stu-id="0e12e-155">description</span></span>|<span data-ttu-id="0e12e-156">String</span><span class="sxs-lookup"><span data-stu-id="0e12e-156">String</span></span>|<span data-ttu-id="0e12e-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0e12e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e12e-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0e12e-159">displayName</span></span>|<span data-ttu-id="0e12e-160">String</span><span class="sxs-lookup"><span data-stu-id="0e12e-160">String</span></span>|<span data-ttu-id="0e12e-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0e12e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e12e-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-163">version</span><span class="sxs-lookup"><span data-stu-id="0e12e-163">version</span></span>|<span data-ttu-id="0e12e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0e12e-164">Int32</span></span>|<span data-ttu-id="0e12e-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0e12e-165">Version of the device configuration.</span></span> <span data-ttu-id="0e12e-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-167">networkName</span><span class="sxs-lookup"><span data-stu-id="0e12e-167">networkName</span></span>|<span data-ttu-id="0e12e-168">字符串</span><span class="sxs-lookup"><span data-stu-id="0e12e-168">String</span></span>|<span data-ttu-id="0e12e-169">从[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="0e12e-169">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-170">ssid</span><span class="sxs-lookup"><span data-stu-id="0e12e-170">ssid</span></span>|<span data-ttu-id="0e12e-171">字符串</span><span class="sxs-lookup"><span data-stu-id="0e12e-171">String</span></span>|<span data-ttu-id="0e12e-172">这是广播到所有设备的 wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="0e12e-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="0e12e-173">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-173">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0e12e-174">connectAutomatically</span></span>|<span data-ttu-id="0e12e-175">布尔</span><span class="sxs-lookup"><span data-stu-id="0e12e-175">Boolean</span></span>|<span data-ttu-id="0e12e-176">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="0e12e-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0e12e-177">将此设置为 true 将跳过用户提示, 并自动将设备连接到 wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="0e12e-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="0e12e-178">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-178">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0e12e-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0e12e-180">布尔</span><span class="sxs-lookup"><span data-stu-id="0e12e-180">Boolean</span></span>|<span data-ttu-id="0e12e-181">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="0e12e-181">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="0e12e-182">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="0e12e-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="0e12e-183">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-183">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0e12e-184">wiFiSecurityType</span></span>|[<span data-ttu-id="0e12e-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0e12e-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="0e12e-186">指示 wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="0e12e-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0e12e-187">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0e12e-187">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="0e12e-188">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="0e12e-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="0e12e-189">proxySettings</span><span class="sxs-lookup"><span data-stu-id="0e12e-189">proxySettings</span></span>|[<span data-ttu-id="0e12e-190">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="0e12e-190">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="0e12e-191">从[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)继承的此 wi-fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="0e12e-191">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="0e12e-192">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="0e12e-192">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="0e12e-193">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="0e12e-193">proxyManualAddress</span></span>|<span data-ttu-id="0e12e-194">字符串</span><span class="sxs-lookup"><span data-stu-id="0e12e-194">String</span></span>|<span data-ttu-id="0e12e-195">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="0e12e-195">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="0e12e-196">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-196">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-197">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="0e12e-197">proxyManualPort</span></span>|<span data-ttu-id="0e12e-198">Int32</span><span class="sxs-lookup"><span data-stu-id="0e12e-198">Int32</span></span>|<span data-ttu-id="0e12e-199">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="0e12e-199">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="0e12e-200">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-200">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-201">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="0e12e-201">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="0e12e-202">字符串</span><span class="sxs-lookup"><span data-stu-id="0e12e-202">String</span></span>|<span data-ttu-id="0e12e-203">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="0e12e-203">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="0e12e-204">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="0e12e-204">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="0e12e-205">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-205">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-206">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0e12e-206">preSharedKey</span></span>|<span data-ttu-id="0e12e-207">字符串</span><span class="sxs-lookup"><span data-stu-id="0e12e-207">String</span></span>|<span data-ttu-id="0e12e-208">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="0e12e-208">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="0e12e-209">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e12e-209">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="0e12e-210">eapType</span><span class="sxs-lookup"><span data-stu-id="0e12e-210">eapType</span></span>|[<span data-ttu-id="0e12e-211">eapType</span><span class="sxs-lookup"><span data-stu-id="0e12e-211">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="0e12e-212">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="0e12e-212">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="0e12e-213">指示在 wlan 终结点 (路由器) 上设置的 EAP 协议的类型。</span><span class="sxs-lookup"><span data-stu-id="0e12e-213">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="0e12e-214">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="0e12e-214">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="0e12e-215">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e12e-215">eapFastConfiguration</span></span>|[<span data-ttu-id="0e12e-216">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e12e-216">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="0e12e-217">eap-fast 配置选项, 当 eap-fast 是所选的 eap 类型时。</span><span class="sxs-lookup"><span data-stu-id="0e12e-217">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="0e12e-218">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="0e12e-218">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="0e12e-219">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="0e12e-219">trustedServerCertificateNames</span></span>|<span data-ttu-id="0e12e-220">String collection</span><span class="sxs-lookup"><span data-stu-id="0e12e-220">String collection</span></span>|<span data-ttu-id="0e12e-221">将 eap 类型配置为 eap-tls/TTLS/FAST 或 PEAP 时受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="0e12e-221">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="0e12e-222">这是由受信任的证书颁发机构 (CA) 颁发的证书中使用的公用名称。</span><span class="sxs-lookup"><span data-stu-id="0e12e-222">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="0e12e-223">如果您提供此信息, 您可以绕过在最终用户设备连接到此 wi-fi 网络时显示的 "动态信任" 对话框。</span><span class="sxs-lookup"><span data-stu-id="0e12e-223">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="0e12e-224">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0e12e-224">authenticationMethod</span></span>|[<span data-ttu-id="0e12e-225">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0e12e-225">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="0e12e-226">EAP 类型配置为 PEAP 或 EAP-TTLS 时的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0e12e-226">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="0e12e-227">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="0e12e-227">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="0e12e-228">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="0e12e-228">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="0e12e-229">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="0e12e-229">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="0e12e-230">eap 类型为 eap 时, 用于身份验证的非 EAP 方法 (内部标识)-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="0e12e-230">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="0e12e-231">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="0e12e-231">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="0e12e-232">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="0e12e-232">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="0e12e-233">字符串</span><span class="sxs-lookup"><span data-stu-id="0e12e-233">String</span></span>|<span data-ttu-id="0e12e-234">将 eap 类型配置为 eap-TTLS、eap-fast 或 PEAP 时启用标识隐私 (外部标识)。</span><span class="sxs-lookup"><span data-stu-id="0e12e-234">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="0e12e-235">此属性使用您输入的文本屏蔽用户名。</span><span class="sxs-lookup"><span data-stu-id="0e12e-235">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="0e12e-236">例如, 如果使用 "匿名", 则使用其真实用户名通过此 wlan 连接进行身份验证的每个用户都将显示为 "匿名"。</span><span class="sxs-lookup"><span data-stu-id="0e12e-236">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="0e12e-237">响应</span><span class="sxs-lookup"><span data-stu-id="0e12e-237">Response</span></span>
<span data-ttu-id="0e12e-238">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e12e-238">If successful, this method returns a `201 Created` response code and a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e12e-239">示例</span><span class="sxs-lookup"><span data-stu-id="0e12e-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e12e-240">请求</span><span class="sxs-lookup"><span data-stu-id="0e12e-240">Request</span></span>
<span data-ttu-id="0e12e-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e12e-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1085

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="0e12e-242">响应</span><span class="sxs-lookup"><span data-stu-id="0e12e-242">Response</span></span>
<span data-ttu-id="0e12e-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e12e-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1257

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




