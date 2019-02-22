---
title: 创建 windowsWifiEnterpriseEAPConfiguration
description: 创建新的 windowsWifiEnterpriseEAPConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8df4ef22727b6bb56ccf759408f60ba22f0dc6dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146723"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="206a8-103">创建 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="206a8-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="206a8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="206a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="206a8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="206a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="206a8-106">创建新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="206a8-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="206a8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="206a8-107">Prerequisites</span></span>
<span data-ttu-id="206a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="206a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="206a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="206a8-110">Permission type</span></span>|<span data-ttu-id="206a8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="206a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="206a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="206a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="206a8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="206a8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="206a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="206a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="206a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="206a8-115">Not supported.</span></span>|
|<span data-ttu-id="206a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="206a8-116">Application</span></span>|<span data-ttu-id="206a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="206a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="206a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="206a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="206a8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="206a8-119">Request headers</span></span>
|<span data-ttu-id="206a8-120">标头</span><span class="sxs-lookup"><span data-stu-id="206a8-120">Header</span></span>|<span data-ttu-id="206a8-121">值</span><span class="sxs-lookup"><span data-stu-id="206a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="206a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="206a8-122">Authorization</span></span>|<span data-ttu-id="206a8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="206a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="206a8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="206a8-124">Accept</span></span>|<span data-ttu-id="206a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="206a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="206a8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="206a8-126">Request body</span></span>
<span data-ttu-id="206a8-127">在请求正文中, 提供 windowsWifiEnterpriseEAPConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="206a8-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="206a8-128">下表显示创建 windowsWifiEnterpriseEAPConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="206a8-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="206a8-129">属性</span><span class="sxs-lookup"><span data-stu-id="206a8-129">Property</span></span>|<span data-ttu-id="206a8-130">类型</span><span class="sxs-lookup"><span data-stu-id="206a8-130">Type</span></span>|<span data-ttu-id="206a8-131">说明</span><span class="sxs-lookup"><span data-stu-id="206a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="206a8-132">id</span><span class="sxs-lookup"><span data-stu-id="206a8-132">id</span></span>|<span data-ttu-id="206a8-133">String</span><span class="sxs-lookup"><span data-stu-id="206a8-133">String</span></span>|<span data-ttu-id="206a8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="206a8-134">Key of the entity.</span></span> <span data-ttu-id="206a8-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="206a8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="206a8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="206a8-137">DateTimeOffset</span></span>|<span data-ttu-id="206a8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="206a8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="206a8-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="206a8-140">roleScopeTagIds</span></span>|<span data-ttu-id="206a8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="206a8-141">String collection</span></span>|<span data-ttu-id="206a8-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="206a8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="206a8-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="206a8-144">supportsScopeTags</span></span>|<span data-ttu-id="206a8-145">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-145">Boolean</span></span>|<span data-ttu-id="206a8-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="206a8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="206a8-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="206a8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="206a8-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="206a8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="206a8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="206a8-149">This property is read-only.</span></span> <span data-ttu-id="206a8-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="206a8-151">createdDateTime</span></span>|<span data-ttu-id="206a8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="206a8-152">DateTimeOffset</span></span>|<span data-ttu-id="206a8-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="206a8-153">DateTime the object was created.</span></span> <span data-ttu-id="206a8-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-155">description</span><span class="sxs-lookup"><span data-stu-id="206a8-155">description</span></span>|<span data-ttu-id="206a8-156">String</span><span class="sxs-lookup"><span data-stu-id="206a8-156">String</span></span>|<span data-ttu-id="206a8-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="206a8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="206a8-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="206a8-159">displayName</span></span>|<span data-ttu-id="206a8-160">String</span><span class="sxs-lookup"><span data-stu-id="206a8-160">String</span></span>|<span data-ttu-id="206a8-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="206a8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="206a8-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-163">version</span><span class="sxs-lookup"><span data-stu-id="206a8-163">version</span></span>|<span data-ttu-id="206a8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="206a8-164">Int32</span></span>|<span data-ttu-id="206a8-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="206a8-165">Version of the device configuration.</span></span> <span data-ttu-id="206a8-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="206a8-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="206a8-167">preSharedKey</span></span>|<span data-ttu-id="206a8-168">字符串</span><span class="sxs-lookup"><span data-stu-id="206a8-168">String</span></span>|<span data-ttu-id="206a8-169">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="206a8-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="206a8-170">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-170">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="206a8-171">wifiSecurityType</span></span>|[<span data-ttu-id="206a8-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="206a8-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="206a8-173">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="206a8-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="206a8-174">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="206a8-174">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="206a8-175">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="206a8-175">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="206a8-176">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="206a8-176">meteredConnectionLimit</span></span>|[<span data-ttu-id="206a8-177">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="206a8-177">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="206a8-178">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="206a8-178">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="206a8-179">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="206a8-179">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="206a8-180">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="206a8-180">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="206a8-181">ssid</span><span class="sxs-lookup"><span data-stu-id="206a8-181">ssid</span></span>|<span data-ttu-id="206a8-182">字符串</span><span class="sxs-lookup"><span data-stu-id="206a8-182">String</span></span>|<span data-ttu-id="206a8-183">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="206a8-183">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="206a8-184">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-184">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-185">networkName</span><span class="sxs-lookup"><span data-stu-id="206a8-185">networkName</span></span>|<span data-ttu-id="206a8-186">字符串</span><span class="sxs-lookup"><span data-stu-id="206a8-186">String</span></span>|<span data-ttu-id="206a8-187">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="206a8-187">Specify the network configuration name.</span></span> <span data-ttu-id="206a8-188">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-188">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-189">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="206a8-189">connectAutomatically</span></span>|<span data-ttu-id="206a8-190">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-190">Boolean</span></span>|<span data-ttu-id="206a8-191">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="206a8-191">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="206a8-192">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-193">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="206a8-193">connectToPreferredNetwork</span></span>|<span data-ttu-id="206a8-194">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-194">Boolean</span></span>|<span data-ttu-id="206a8-195">指定 wifi 连接是否应连接到更多的首选网络 (如果已连接到此连接的话)。</span><span class="sxs-lookup"><span data-stu-id="206a8-195">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="206a8-196">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="206a8-196">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="206a8-197">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-198">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="206a8-198">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="206a8-199">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-199">Boolean</span></span>|<span data-ttu-id="206a8-200">指定是否应自动连接 wifi 连接, 即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="206a8-200">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="206a8-201">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-202">proxySetting</span><span class="sxs-lookup"><span data-stu-id="206a8-202">proxySetting</span></span>|[<span data-ttu-id="206a8-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="206a8-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="206a8-204">指定从[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)继承的 wi-fi 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="206a8-204">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="206a8-205">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="206a8-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="206a8-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="206a8-206">proxyManualAddress</span></span>|<span data-ttu-id="206a8-207">字符串</span><span class="sxs-lookup"><span data-stu-id="206a8-207">String</span></span>|<span data-ttu-id="206a8-208">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="206a8-208">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="206a8-209">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="206a8-210">proxyManualPort</span></span>|<span data-ttu-id="206a8-211">Int32</span><span class="sxs-lookup"><span data-stu-id="206a8-211">Int32</span></span>|<span data-ttu-id="206a8-212">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="206a8-212">Specify the port for the proxy server.</span></span> <span data-ttu-id="206a8-213">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="206a8-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="206a8-215">字符串</span><span class="sxs-lookup"><span data-stu-id="206a8-215">String</span></span>|<span data-ttu-id="206a8-216">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="206a8-216">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="206a8-217">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-217">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-218">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="206a8-218">forceFIPSCompliance</span></span>|<span data-ttu-id="206a8-219">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-219">Boolean</span></span>|<span data-ttu-id="206a8-220">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="206a8-220">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="206a8-221">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="206a8-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="206a8-222">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="206a8-222">networkSingleSignOn</span></span>|[<span data-ttu-id="206a8-223">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="206a8-223">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="206a8-224">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="206a8-224">Specify the network single sign on type.</span></span> <span data-ttu-id="206a8-225">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="206a8-225">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="206a8-226">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="206a8-226">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="206a8-227">Int32</span><span class="sxs-lookup"><span data-stu-id="206a8-227">Int32</span></span>|<span data-ttu-id="206a8-228">指定最大身份验证超时 (以秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="206a8-228">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="206a8-229">有效范围: 1-120</span><span class="sxs-lookup"><span data-stu-id="206a8-229">Valid range: 1-120</span></span>|
|<span data-ttu-id="206a8-230">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="206a8-230">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="206a8-231">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-231">Boolean</span></span>|<span data-ttu-id="206a8-232">指定 wifi 连接是否应提示额外的身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="206a8-232">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="206a8-233">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="206a8-233">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="206a8-234">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-234">Boolean</span></span>|<span data-ttu-id="206a8-235">指定 wifi 连接是否应启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="206a8-235">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="206a8-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="206a8-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="206a8-237">Int32</span><span class="sxs-lookup"><span data-stu-id="206a8-237">Int32</span></span>|<span data-ttu-id="206a8-238">指定最大成对主密钥缓存时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="206a8-238">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="206a8-239">有效范围: 5-1440</span><span class="sxs-lookup"><span data-stu-id="206a8-239">Valid range: 5-1440</span></span>|
|<span data-ttu-id="206a8-240">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="206a8-240">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="206a8-241">Int32</span><span class="sxs-lookup"><span data-stu-id="206a8-241">Int32</span></span>|<span data-ttu-id="206a8-242">指定缓存中成对主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="206a8-242">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="206a8-243">有效范围: 1-255</span><span class="sxs-lookup"><span data-stu-id="206a8-243">Valid range: 1-255</span></span>|
|<span data-ttu-id="206a8-244">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="206a8-244">enablePreAuthentication</span></span>|<span data-ttu-id="206a8-245">布尔</span><span class="sxs-lookup"><span data-stu-id="206a8-245">Boolean</span></span>|<span data-ttu-id="206a8-246">指定是否应启用预先身份验证。</span><span class="sxs-lookup"><span data-stu-id="206a8-246">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="206a8-247">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="206a8-247">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="206a8-248">Int32</span><span class="sxs-lookup"><span data-stu-id="206a8-248">Int32</span></span>|<span data-ttu-id="206a8-249">指定最大预先身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="206a8-249">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="206a8-250">有效范围: 1-16</span><span class="sxs-lookup"><span data-stu-id="206a8-250">Valid range: 1-16</span></span>|
|<span data-ttu-id="206a8-251">eapType</span><span class="sxs-lookup"><span data-stu-id="206a8-251">eapType</span></span>|[<span data-ttu-id="206a8-252">eapType</span><span class="sxs-lookup"><span data-stu-id="206a8-252">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="206a8-253">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="206a8-253">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="206a8-254">指示在 wlan 终结点 (路由器) 上设置的 EAP 协议的类型。</span><span class="sxs-lookup"><span data-stu-id="206a8-254">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="206a8-255">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="206a8-255">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="206a8-256">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="206a8-256">trustedServerCertificateNames</span></span>|<span data-ttu-id="206a8-257">String collection</span><span class="sxs-lookup"><span data-stu-id="206a8-257">String collection</span></span>|<span data-ttu-id="206a8-258">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="206a8-258">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="206a8-259">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="206a8-259">authenticationMethod</span></span>|[<span data-ttu-id="206a8-260">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="206a8-260">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="206a8-261">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="206a8-261">Specify the authentication method.</span></span> <span data-ttu-id="206a8-262">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="206a8-262">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="206a8-263">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="206a8-263">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="206a8-264">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="206a8-264">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="206a8-265">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="206a8-265">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="206a8-266">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="206a8-266">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="206a8-267">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="206a8-267">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="206a8-268">字符串</span><span class="sxs-lookup"><span data-stu-id="206a8-268">String</span></span>|<span data-ttu-id="206a8-269">指定在使用 EAP TTLS 或 PEAP 时用于替换隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="206a8-269">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="206a8-270">响应</span><span class="sxs-lookup"><span data-stu-id="206a8-270">Response</span></span>
<span data-ttu-id="206a8-271">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="206a8-271">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="206a8-272">示例</span><span class="sxs-lookup"><span data-stu-id="206a8-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="206a8-273">请求</span><span class="sxs-lookup"><span data-stu-id="206a8-273">Request</span></span>
<span data-ttu-id="206a8-274">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="206a8-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="206a8-275">响应</span><span class="sxs-lookup"><span data-stu-id="206a8-275">Response</span></span>
<span data-ttu-id="206a8-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="206a8-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




