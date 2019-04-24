---
title: 更新 windowsWifiEnterpriseEAPConfiguration
description: 更新 windowsWifiEnterpriseEAPConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a87a8e3d4d3668c5193c44925db163df14c4bce9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510869"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="f225f-103">更新 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="f225f-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="f225f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f225f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f225f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f225f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f225f-106">更新[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f225f-106">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f225f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f225f-107">Prerequisites</span></span>
<span data-ttu-id="f225f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f225f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f225f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f225f-110">Permission type</span></span>|<span data-ttu-id="f225f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f225f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f225f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f225f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f225f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f225f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f225f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f225f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f225f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f225f-115">Not supported.</span></span>|
|<span data-ttu-id="f225f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f225f-116">Application</span></span>|<span data-ttu-id="f225f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f225f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f225f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f225f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f225f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f225f-119">Request headers</span></span>
|<span data-ttu-id="f225f-120">标头</span><span class="sxs-lookup"><span data-stu-id="f225f-120">Header</span></span>|<span data-ttu-id="f225f-121">值</span><span class="sxs-lookup"><span data-stu-id="f225f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f225f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f225f-122">Authorization</span></span>|<span data-ttu-id="f225f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f225f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f225f-124">接受</span><span class="sxs-lookup"><span data-stu-id="f225f-124">Accept</span></span>|<span data-ttu-id="f225f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f225f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f225f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f225f-126">Request body</span></span>
<span data-ttu-id="f225f-127">在请求正文中, 提供[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f225f-127">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="f225f-128">下表显示创建[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f225f-128">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="f225f-129">属性</span><span class="sxs-lookup"><span data-stu-id="f225f-129">Property</span></span>|<span data-ttu-id="f225f-130">类型</span><span class="sxs-lookup"><span data-stu-id="f225f-130">Type</span></span>|<span data-ttu-id="f225f-131">说明</span><span class="sxs-lookup"><span data-stu-id="f225f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f225f-132">id</span><span class="sxs-lookup"><span data-stu-id="f225f-132">id</span></span>|<span data-ttu-id="f225f-133">String</span><span class="sxs-lookup"><span data-stu-id="f225f-133">String</span></span>|<span data-ttu-id="f225f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f225f-134">Key of the entity.</span></span> <span data-ttu-id="f225f-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f225f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f225f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f225f-137">DateTimeOffset</span></span>|<span data-ttu-id="f225f-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f225f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f225f-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f225f-140">roleScopeTagIds</span></span>|<span data-ttu-id="f225f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f225f-141">String collection</span></span>|<span data-ttu-id="f225f-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f225f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f225f-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f225f-144">supportsScopeTags</span></span>|<span data-ttu-id="f225f-145">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-145">Boolean</span></span>|<span data-ttu-id="f225f-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f225f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f225f-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f225f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f225f-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f225f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f225f-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f225f-149">This property is read-only.</span></span> <span data-ttu-id="f225f-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f225f-151">createdDateTime</span></span>|<span data-ttu-id="f225f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f225f-152">DateTimeOffset</span></span>|<span data-ttu-id="f225f-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f225f-153">DateTime the object was created.</span></span> <span data-ttu-id="f225f-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-155">description</span><span class="sxs-lookup"><span data-stu-id="f225f-155">description</span></span>|<span data-ttu-id="f225f-156">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-156">String</span></span>|<span data-ttu-id="f225f-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f225f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f225f-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f225f-159">displayName</span></span>|<span data-ttu-id="f225f-160">String</span><span class="sxs-lookup"><span data-stu-id="f225f-160">String</span></span>|<span data-ttu-id="f225f-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f225f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f225f-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-163">version</span><span class="sxs-lookup"><span data-stu-id="f225f-163">version</span></span>|<span data-ttu-id="f225f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f225f-164">Int32</span></span>|<span data-ttu-id="f225f-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f225f-165">Version of the device configuration.</span></span> <span data-ttu-id="f225f-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f225f-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f225f-167">preSharedKey</span></span>|<span data-ttu-id="f225f-168">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-168">String</span></span>|<span data-ttu-id="f225f-169">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="f225f-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="f225f-170">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-170">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f225f-171">wifiSecurityType</span></span>|[<span data-ttu-id="f225f-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f225f-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="f225f-173">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="f225f-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="f225f-174">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f225f-174">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="f225f-175">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="f225f-175">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f225f-176">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="f225f-176">meteredConnectionLimit</span></span>|[<span data-ttu-id="f225f-177">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="f225f-177">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="f225f-178">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="f225f-178">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="f225f-179">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f225f-179">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="f225f-180">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="f225f-180">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="f225f-181">ssid</span><span class="sxs-lookup"><span data-stu-id="f225f-181">ssid</span></span>|<span data-ttu-id="f225f-182">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-182">String</span></span>|<span data-ttu-id="f225f-183">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="f225f-183">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="f225f-184">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-184">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-185">networkName</span><span class="sxs-lookup"><span data-stu-id="f225f-185">networkName</span></span>|<span data-ttu-id="f225f-186">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-186">String</span></span>|<span data-ttu-id="f225f-187">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="f225f-187">Specify the network configuration name.</span></span> <span data-ttu-id="f225f-188">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-188">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-189">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f225f-189">connectAutomatically</span></span>|<span data-ttu-id="f225f-190">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-190">Boolean</span></span>|<span data-ttu-id="f225f-191">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="f225f-191">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="f225f-192">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-193">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="f225f-193">connectToPreferredNetwork</span></span>|<span data-ttu-id="f225f-194">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-194">Boolean</span></span>|<span data-ttu-id="f225f-195">指定 wifi 连接是否应连接到更多的首选网络 (如果已连接到此连接的话)。</span><span class="sxs-lookup"><span data-stu-id="f225f-195">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="f225f-196">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="f225f-196">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="f225f-197">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-198">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f225f-198">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f225f-199">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-199">Boolean</span></span>|<span data-ttu-id="f225f-200">指定是否应自动连接 wifi 连接, 即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="f225f-200">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="f225f-201">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-202">proxySetting</span><span class="sxs-lookup"><span data-stu-id="f225f-202">proxySetting</span></span>|[<span data-ttu-id="f225f-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="f225f-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f225f-204">指定从[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)继承的 wi-fi 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="f225f-204">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="f225f-205">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="f225f-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f225f-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="f225f-206">proxyManualAddress</span></span>|<span data-ttu-id="f225f-207">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-207">String</span></span>|<span data-ttu-id="f225f-208">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="f225f-208">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="f225f-209">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="f225f-210">proxyManualPort</span></span>|<span data-ttu-id="f225f-211">Int32</span><span class="sxs-lookup"><span data-stu-id="f225f-211">Int32</span></span>|<span data-ttu-id="f225f-212">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="f225f-212">Specify the port for the proxy server.</span></span> <span data-ttu-id="f225f-213">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="f225f-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f225f-215">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-215">String</span></span>|<span data-ttu-id="f225f-216">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="f225f-216">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="f225f-217">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-217">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-218">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="f225f-218">forceFIPSCompliance</span></span>|<span data-ttu-id="f225f-219">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-219">Boolean</span></span>|<span data-ttu-id="f225f-220">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="f225f-220">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="f225f-221">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f225f-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f225f-222">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="f225f-222">networkSingleSignOn</span></span>|[<span data-ttu-id="f225f-223">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="f225f-223">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="f225f-224">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="f225f-224">Specify the network single sign on type.</span></span> <span data-ttu-id="f225f-225">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="f225f-225">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="f225f-226">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="f225f-226">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="f225f-227">Int32</span><span class="sxs-lookup"><span data-stu-id="f225f-227">Int32</span></span>|<span data-ttu-id="f225f-228">指定最大身份验证超时 (以秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="f225f-228">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="f225f-229">有效范围: 1-120</span><span class="sxs-lookup"><span data-stu-id="f225f-229">Valid range: 1-120</span></span>|
|<span data-ttu-id="f225f-230">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="f225f-230">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="f225f-231">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-231">Boolean</span></span>|<span data-ttu-id="f225f-232">指定 wifi 连接是否应提示额外的身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="f225f-232">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="f225f-233">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="f225f-233">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="f225f-234">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-234">Boolean</span></span>|<span data-ttu-id="f225f-235">指定 wifi 连接是否应启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="f225f-235">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="f225f-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="f225f-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="f225f-237">Int32</span><span class="sxs-lookup"><span data-stu-id="f225f-237">Int32</span></span>|<span data-ttu-id="f225f-238">指定最大成对主密钥缓存时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="f225f-238">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="f225f-239">有效范围: 5-1440</span><span class="sxs-lookup"><span data-stu-id="f225f-239">Valid range: 5-1440</span></span>|
|<span data-ttu-id="f225f-240">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="f225f-240">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="f225f-241">Int32</span><span class="sxs-lookup"><span data-stu-id="f225f-241">Int32</span></span>|<span data-ttu-id="f225f-242">指定缓存中成对主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="f225f-242">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="f225f-243">有效范围: 1-255</span><span class="sxs-lookup"><span data-stu-id="f225f-243">Valid range: 1-255</span></span>|
|<span data-ttu-id="f225f-244">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="f225f-244">enablePreAuthentication</span></span>|<span data-ttu-id="f225f-245">布尔</span><span class="sxs-lookup"><span data-stu-id="f225f-245">Boolean</span></span>|<span data-ttu-id="f225f-246">指定是否应启用预先身份验证。</span><span class="sxs-lookup"><span data-stu-id="f225f-246">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="f225f-247">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="f225f-247">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="f225f-248">Int32</span><span class="sxs-lookup"><span data-stu-id="f225f-248">Int32</span></span>|<span data-ttu-id="f225f-249">指定最大预先身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="f225f-249">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="f225f-250">有效范围: 1-16</span><span class="sxs-lookup"><span data-stu-id="f225f-250">Valid range: 1-16</span></span>|
|<span data-ttu-id="f225f-251">eapType</span><span class="sxs-lookup"><span data-stu-id="f225f-251">eapType</span></span>|[<span data-ttu-id="f225f-252">eapType</span><span class="sxs-lookup"><span data-stu-id="f225f-252">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="f225f-253">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="f225f-253">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="f225f-254">指示在 wlan 终结点 (路由器) 上设置的 EAP 协议的类型。</span><span class="sxs-lookup"><span data-stu-id="f225f-254">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f225f-255">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="f225f-255">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="f225f-256">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="f225f-256">trustedServerCertificateNames</span></span>|<span data-ttu-id="f225f-257">String collection</span><span class="sxs-lookup"><span data-stu-id="f225f-257">String collection</span></span>|<span data-ttu-id="f225f-258">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="f225f-258">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="f225f-259">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f225f-259">authenticationMethod</span></span>|[<span data-ttu-id="f225f-260">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f225f-260">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f225f-261">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f225f-261">Specify the authentication method.</span></span> <span data-ttu-id="f225f-262">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="f225f-262">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f225f-263">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="f225f-263">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="f225f-264">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="f225f-264">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f225f-265">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="f225f-265">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="f225f-266">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="f225f-266">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f225f-267">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f225f-267">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f225f-268">字符串</span><span class="sxs-lookup"><span data-stu-id="f225f-268">String</span></span>|<span data-ttu-id="f225f-269">指定在使用 EAP TTLS 或 PEAP 时用于替换隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="f225f-269">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="f225f-270">响应</span><span class="sxs-lookup"><span data-stu-id="f225f-270">Response</span></span>
<span data-ttu-id="f225f-271">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f225f-271">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f225f-272">示例</span><span class="sxs-lookup"><span data-stu-id="f225f-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="f225f-273">请求</span><span class="sxs-lookup"><span data-stu-id="f225f-273">Request</span></span>
<span data-ttu-id="f225f-274">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f225f-274">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f225f-275">响应</span><span class="sxs-lookup"><span data-stu-id="f225f-275">Response</span></span>
<span data-ttu-id="f225f-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f225f-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





