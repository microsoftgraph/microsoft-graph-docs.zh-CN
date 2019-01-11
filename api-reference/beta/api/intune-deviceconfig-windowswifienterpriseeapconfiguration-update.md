---
title: 更新 windowsWifiEnterpriseEAPConfiguration
description: 更新 windowsWifiEnterpriseEAPConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4daa930e47c20f4a330ed9a860c2bc2c9224e742
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832639"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="036a4-103">更新 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="036a4-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="036a4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="036a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="036a4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="036a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="036a4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="036a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="036a4-107">更新[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="036a4-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="036a4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="036a4-108">Prerequisites</span></span>
<span data-ttu-id="036a4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="036a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="036a4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="036a4-111">Permission type</span></span>|<span data-ttu-id="036a4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="036a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="036a4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="036a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="036a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="036a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="036a4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="036a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="036a4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="036a4-116">Not supported.</span></span>|
|<span data-ttu-id="036a4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="036a4-117">Application</span></span>|<span data-ttu-id="036a4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="036a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="036a4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="036a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="036a4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="036a4-120">Request headers</span></span>
|<span data-ttu-id="036a4-121">标头</span><span class="sxs-lookup"><span data-stu-id="036a4-121">Header</span></span>|<span data-ttu-id="036a4-122">值</span><span class="sxs-lookup"><span data-stu-id="036a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="036a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="036a4-123">Authorization</span></span>|<span data-ttu-id="036a4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="036a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="036a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="036a4-125">Accept</span></span>|<span data-ttu-id="036a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="036a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="036a4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="036a4-127">Request body</span></span>
<span data-ttu-id="036a4-128">在请求正文中，提供[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="036a4-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="036a4-129">下表显示时创建[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="036a4-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="036a4-130">属性</span><span class="sxs-lookup"><span data-stu-id="036a4-130">Property</span></span>|<span data-ttu-id="036a4-131">类型</span><span class="sxs-lookup"><span data-stu-id="036a4-131">Type</span></span>|<span data-ttu-id="036a4-132">说明</span><span class="sxs-lookup"><span data-stu-id="036a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="036a4-133">id</span><span class="sxs-lookup"><span data-stu-id="036a4-133">id</span></span>|<span data-ttu-id="036a4-134">String</span><span class="sxs-lookup"><span data-stu-id="036a4-134">String</span></span>|<span data-ttu-id="036a4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="036a4-135">Key of the entity.</span></span> <span data-ttu-id="036a4-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="036a4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="036a4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="036a4-138">DateTimeOffset</span></span>|<span data-ttu-id="036a4-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="036a4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="036a4-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="036a4-141">roleScopeTagIds</span></span>|<span data-ttu-id="036a4-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="036a4-142">String collection</span></span>|<span data-ttu-id="036a4-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="036a4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="036a4-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="036a4-145">supportsScopeTags</span></span>|<span data-ttu-id="036a4-146">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-146">Boolean</span></span>|<span data-ttu-id="036a4-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="036a4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="036a4-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="036a4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="036a4-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="036a4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="036a4-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="036a4-150">This property is read-only.</span></span> <span data-ttu-id="036a4-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="036a4-152">createdDateTime</span></span>|<span data-ttu-id="036a4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="036a4-153">DateTimeOffset</span></span>|<span data-ttu-id="036a4-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="036a4-154">DateTime the object was created.</span></span> <span data-ttu-id="036a4-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-156">description</span><span class="sxs-lookup"><span data-stu-id="036a4-156">description</span></span>|<span data-ttu-id="036a4-157">String</span><span class="sxs-lookup"><span data-stu-id="036a4-157">String</span></span>|<span data-ttu-id="036a4-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="036a4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="036a4-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="036a4-160">displayName</span></span>|<span data-ttu-id="036a4-161">String</span><span class="sxs-lookup"><span data-stu-id="036a4-161">String</span></span>|<span data-ttu-id="036a4-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="036a4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="036a4-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-164">version</span><span class="sxs-lookup"><span data-stu-id="036a4-164">version</span></span>|<span data-ttu-id="036a4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="036a4-165">Int32</span></span>|<span data-ttu-id="036a4-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="036a4-166">Version of the device configuration.</span></span> <span data-ttu-id="036a4-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="036a4-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="036a4-168">preSharedKey</span></span>|<span data-ttu-id="036a4-169">字符串</span><span class="sxs-lookup"><span data-stu-id="036a4-169">String</span></span>|<span data-ttu-id="036a4-170">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="036a4-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="036a4-171">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-171">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-172">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="036a4-172">wifiSecurityType</span></span>|[<span data-ttu-id="036a4-173">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="036a4-173">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="036a4-174">指定的 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="036a4-174">Specify the Wifi Security Type.</span></span> <span data-ttu-id="036a4-175">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="036a4-175">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="036a4-176">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="036a4-176">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="036a4-177">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="036a4-177">meteredConnectionLimit</span></span>|[<span data-ttu-id="036a4-178">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="036a4-178">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="036a4-179">指定 wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="036a4-179">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="036a4-180">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="036a4-180">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="036a4-181">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="036a4-181">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="036a4-182">ssid</span><span class="sxs-lookup"><span data-stu-id="036a4-182">ssid</span></span>|<span data-ttu-id="036a4-183">字符串</span><span class="sxs-lookup"><span data-stu-id="036a4-183">String</span></span>|<span data-ttu-id="036a4-184">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="036a4-184">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="036a4-185">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-185">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-186">networkName</span><span class="sxs-lookup"><span data-stu-id="036a4-186">networkName</span></span>|<span data-ttu-id="036a4-187">字符串</span><span class="sxs-lookup"><span data-stu-id="036a4-187">String</span></span>|<span data-ttu-id="036a4-188">指定的网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="036a4-188">Specify the network configuration name.</span></span> <span data-ttu-id="036a4-189">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-189">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-190">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="036a4-190">connectAutomatically</span></span>|<span data-ttu-id="036a4-191">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-191">Boolean</span></span>|<span data-ttu-id="036a4-192">指定应在范围中自动连接是否 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="036a4-192">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="036a4-193">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-193">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-194">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="036a4-194">connectToPreferredNetwork</span></span>|<span data-ttu-id="036a4-195">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-195">Boolean</span></span>|<span data-ttu-id="036a4-196">指定 wifi 连接是否应连接到时已连接到此的更多首选网络。</span><span class="sxs-lookup"><span data-stu-id="036a4-196">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="036a4-197">需要 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="036a4-197">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="036a4-198">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-198">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-199">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="036a4-199">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="036a4-200">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-200">Boolean</span></span>|<span data-ttu-id="036a4-201">指定是否 wifi 连接应自动连接即使时 SSID 未进行广播。</span><span class="sxs-lookup"><span data-stu-id="036a4-201">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="036a4-202">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-202">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-203">proxySetting</span><span class="sxs-lookup"><span data-stu-id="036a4-203">proxySetting</span></span>|[<span data-ttu-id="036a4-204">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="036a4-204">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="036a4-205">指定从[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)设置 Wi-fi 配置继承的代理。</span><span class="sxs-lookup"><span data-stu-id="036a4-205">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="036a4-206">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="036a4-206">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="036a4-207">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="036a4-207">proxyManualAddress</span></span>|<span data-ttu-id="036a4-208">字符串</span><span class="sxs-lookup"><span data-stu-id="036a4-208">String</span></span>|<span data-ttu-id="036a4-209">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="036a4-209">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="036a4-210">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-211">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="036a4-211">proxyManualPort</span></span>|<span data-ttu-id="036a4-212">Int32</span><span class="sxs-lookup"><span data-stu-id="036a4-212">Int32</span></span>|<span data-ttu-id="036a4-213">指定的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="036a4-213">Specify the port for the proxy server.</span></span> <span data-ttu-id="036a4-214">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-215">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="036a4-215">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="036a4-216">字符串</span><span class="sxs-lookup"><span data-stu-id="036a4-216">String</span></span>|<span data-ttu-id="036a4-217">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="036a4-217">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="036a4-218">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-218">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="036a4-219">forceFIPSCompliance</span></span>|<span data-ttu-id="036a4-220">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-220">Boolean</span></span>|<span data-ttu-id="036a4-221">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="036a4-221">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="036a4-222">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="036a4-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="036a4-223">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="036a4-223">networkSingleSignOn</span></span>|[<span data-ttu-id="036a4-224">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="036a4-224">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="036a4-225">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="036a4-225">Specify the network single sign on type.</span></span> <span data-ttu-id="036a4-226">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="036a4-226">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="036a4-227">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="036a4-227">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="036a4-228">Int32</span><span class="sxs-lookup"><span data-stu-id="036a4-228">Int32</span></span>|<span data-ttu-id="036a4-229">指定最大的身份验证超时 （以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="036a4-229">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="036a4-230">有效的范围： 1-120</span><span class="sxs-lookup"><span data-stu-id="036a4-230">Valid range: 1-120</span></span>|
|<span data-ttu-id="036a4-231">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="036a4-231">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="036a4-232">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-232">Boolean</span></span>|<span data-ttu-id="036a4-233">指定 wifi 连接是否应提示其他身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="036a4-233">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="036a4-234">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="036a4-234">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="036a4-235">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-235">Boolean</span></span>|<span data-ttu-id="036a4-236">指定 wifi 连接是否应启用缓存成对的主密钥。</span><span class="sxs-lookup"><span data-stu-id="036a4-236">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="036a4-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="036a4-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="036a4-238">Int32</span><span class="sxs-lookup"><span data-stu-id="036a4-238">Int32</span></span>|<span data-ttu-id="036a4-239">指定最大成对主密钥缓存时间 （以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="036a4-239">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="036a4-240">有效的范围： 5 1440年</span><span class="sxs-lookup"><span data-stu-id="036a4-240">Valid range: 5-1440</span></span>|
|<span data-ttu-id="036a4-241">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="036a4-241">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="036a4-242">Int32</span><span class="sxs-lookup"><span data-stu-id="036a4-242">Int32</span></span>|<span data-ttu-id="036a4-243">在缓存中指定成对的主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="036a4-243">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="036a4-244">有效的范围： 1 到 255</span><span class="sxs-lookup"><span data-stu-id="036a4-244">Valid range: 1-255</span></span>|
|<span data-ttu-id="036a4-245">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="036a4-245">enablePreAuthentication</span></span>|<span data-ttu-id="036a4-246">布尔</span><span class="sxs-lookup"><span data-stu-id="036a4-246">Boolean</span></span>|<span data-ttu-id="036a4-247">指定是否应启用预身份验证。</span><span class="sxs-lookup"><span data-stu-id="036a4-247">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="036a4-248">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="036a4-248">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="036a4-249">Int32</span><span class="sxs-lookup"><span data-stu-id="036a4-249">Int32</span></span>|<span data-ttu-id="036a4-250">指定最大预身份验证尝试。</span><span class="sxs-lookup"><span data-stu-id="036a4-250">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="036a4-251">有效的范围： 1-16</span><span class="sxs-lookup"><span data-stu-id="036a4-251">Valid range: 1-16</span></span>|
|<span data-ttu-id="036a4-252">eapType</span><span class="sxs-lookup"><span data-stu-id="036a4-252">eapType</span></span>|[<span data-ttu-id="036a4-253">eapType</span><span class="sxs-lookup"><span data-stu-id="036a4-253">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="036a4-254">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="036a4-254">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="036a4-255">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="036a4-255">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="036a4-256">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="036a4-256">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="036a4-257">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="036a4-257">trustedServerCertificateNames</span></span>|<span data-ttu-id="036a4-258">String 集合</span><span class="sxs-lookup"><span data-stu-id="036a4-258">String collection</span></span>|<span data-ttu-id="036a4-259">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="036a4-259">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="036a4-260">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="036a4-260">authenticationMethod</span></span>|[<span data-ttu-id="036a4-261">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="036a4-261">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="036a4-262">指定的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="036a4-262">Specify the authentication method.</span></span> <span data-ttu-id="036a4-263">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="036a4-263">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="036a4-264">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="036a4-264">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="036a4-265">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="036a4-265">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="036a4-266">指定 EAP TTL 内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="036a4-266">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="036a4-267">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="036a4-267">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="036a4-268">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="036a4-268">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="036a4-269">字符串</span><span class="sxs-lookup"><span data-stu-id="036a4-269">String</span></span>|<span data-ttu-id="036a4-270">指定要使用 EAP TTL 或 PEAP 时替换为隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="036a4-270">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="036a4-271">响应</span><span class="sxs-lookup"><span data-stu-id="036a4-271">Response</span></span>
<span data-ttu-id="036a4-272">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="036a4-272">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="036a4-273">示例</span><span class="sxs-lookup"><span data-stu-id="036a4-273">Example</span></span>
### <a name="request"></a><span data-ttu-id="036a4-274">请求</span><span class="sxs-lookup"><span data-stu-id="036a4-274">Request</span></span>
<span data-ttu-id="036a4-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="036a4-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1492

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="036a4-276">响应</span><span class="sxs-lookup"><span data-stu-id="036a4-276">Response</span></span>
<span data-ttu-id="036a4-p132">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="036a4-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





