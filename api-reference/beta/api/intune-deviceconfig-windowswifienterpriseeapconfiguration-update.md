---
title: 更新 windowsWifiEnterpriseEAPConfiguration
description: 更新 windowsWifiEnterpriseEAPConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c2b99036978f7cff3da786104529157e06d935f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420043"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="b45df-103">更新 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="b45df-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="b45df-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b45df-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b45df-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b45df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b45df-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b45df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b45df-107">更新[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b45df-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b45df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b45df-108">Prerequisites</span></span>
<span data-ttu-id="b45df-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b45df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b45df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b45df-111">Permission type</span></span>|<span data-ttu-id="b45df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b45df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b45df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b45df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b45df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b45df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b45df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b45df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b45df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b45df-116">Not supported.</span></span>|
|<span data-ttu-id="b45df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b45df-117">Application</span></span>|<span data-ttu-id="b45df-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b45df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b45df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b45df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b45df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b45df-120">Request headers</span></span>
|<span data-ttu-id="b45df-121">标头</span><span class="sxs-lookup"><span data-stu-id="b45df-121">Header</span></span>|<span data-ttu-id="b45df-122">值</span><span class="sxs-lookup"><span data-stu-id="b45df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b45df-123">授权</span><span class="sxs-lookup"><span data-stu-id="b45df-123">Authorization</span></span>|<span data-ttu-id="b45df-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b45df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b45df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b45df-125">Accept</span></span>|<span data-ttu-id="b45df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b45df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b45df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b45df-127">Request body</span></span>
<span data-ttu-id="b45df-128">在请求正文中，提供[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b45df-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="b45df-129">下表显示时创建[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b45df-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="b45df-130">属性</span><span class="sxs-lookup"><span data-stu-id="b45df-130">Property</span></span>|<span data-ttu-id="b45df-131">类型</span><span class="sxs-lookup"><span data-stu-id="b45df-131">Type</span></span>|<span data-ttu-id="b45df-132">说明</span><span class="sxs-lookup"><span data-stu-id="b45df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b45df-133">id</span><span class="sxs-lookup"><span data-stu-id="b45df-133">id</span></span>|<span data-ttu-id="b45df-134">String</span><span class="sxs-lookup"><span data-stu-id="b45df-134">String</span></span>|<span data-ttu-id="b45df-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b45df-135">Key of the entity.</span></span> <span data-ttu-id="b45df-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b45df-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b45df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b45df-138">DateTimeOffset</span></span>|<span data-ttu-id="b45df-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b45df-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b45df-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b45df-141">roleScopeTagIds</span></span>|<span data-ttu-id="b45df-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b45df-142">String collection</span></span>|<span data-ttu-id="b45df-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="b45df-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b45df-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b45df-145">supportsScopeTags</span></span>|<span data-ttu-id="b45df-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-146">Boolean</span></span>|<span data-ttu-id="b45df-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="b45df-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b45df-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b45df-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b45df-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="b45df-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b45df-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b45df-150">This property is read-only.</span></span> <span data-ttu-id="b45df-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b45df-152">createdDateTime</span></span>|<span data-ttu-id="b45df-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b45df-153">DateTimeOffset</span></span>|<span data-ttu-id="b45df-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b45df-154">DateTime the object was created.</span></span> <span data-ttu-id="b45df-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-156">description</span><span class="sxs-lookup"><span data-stu-id="b45df-156">description</span></span>|<span data-ttu-id="b45df-157">String</span><span class="sxs-lookup"><span data-stu-id="b45df-157">String</span></span>|<span data-ttu-id="b45df-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b45df-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b45df-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b45df-160">displayName</span></span>|<span data-ttu-id="b45df-161">String</span><span class="sxs-lookup"><span data-stu-id="b45df-161">String</span></span>|<span data-ttu-id="b45df-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b45df-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b45df-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-164">version</span><span class="sxs-lookup"><span data-stu-id="b45df-164">version</span></span>|<span data-ttu-id="b45df-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b45df-165">Int32</span></span>|<span data-ttu-id="b45df-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b45df-166">Version of the device configuration.</span></span> <span data-ttu-id="b45df-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b45df-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b45df-168">preSharedKey</span></span>|<span data-ttu-id="b45df-169">String</span><span class="sxs-lookup"><span data-stu-id="b45df-169">String</span></span>|<span data-ttu-id="b45df-170">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="b45df-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="b45df-171">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-171">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-172">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b45df-172">wifiSecurityType</span></span>|[<span data-ttu-id="b45df-173">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b45df-173">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="b45df-174">指定的 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="b45df-174">Specify the Wifi Security Type.</span></span> <span data-ttu-id="b45df-175">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b45df-175">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="b45df-176">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="b45df-176">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="b45df-177">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="b45df-177">meteredConnectionLimit</span></span>|[<span data-ttu-id="b45df-178">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="b45df-178">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="b45df-179">指定 wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="b45df-179">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="b45df-180">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b45df-180">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="b45df-181">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="b45df-181">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="b45df-182">ssid</span><span class="sxs-lookup"><span data-stu-id="b45df-182">ssid</span></span>|<span data-ttu-id="b45df-183">String</span><span class="sxs-lookup"><span data-stu-id="b45df-183">String</span></span>|<span data-ttu-id="b45df-184">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="b45df-184">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="b45df-185">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-185">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-186">networkName</span><span class="sxs-lookup"><span data-stu-id="b45df-186">networkName</span></span>|<span data-ttu-id="b45df-187">String</span><span class="sxs-lookup"><span data-stu-id="b45df-187">String</span></span>|<span data-ttu-id="b45df-188">指定的网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="b45df-188">Specify the network configuration name.</span></span> <span data-ttu-id="b45df-189">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-189">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-190">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b45df-190">connectAutomatically</span></span>|<span data-ttu-id="b45df-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-191">Boolean</span></span>|<span data-ttu-id="b45df-192">指定应在范围中自动连接是否 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="b45df-192">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="b45df-193">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-193">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-194">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="b45df-194">connectToPreferredNetwork</span></span>|<span data-ttu-id="b45df-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-195">Boolean</span></span>|<span data-ttu-id="b45df-196">指定 wifi 连接是否应连接到时已连接到此的更多首选网络。</span><span class="sxs-lookup"><span data-stu-id="b45df-196">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="b45df-197">需要 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="b45df-197">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="b45df-198">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-198">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-199">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b45df-199">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b45df-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-200">Boolean</span></span>|<span data-ttu-id="b45df-201">指定是否 wifi 连接应自动连接即使时 SSID 未进行广播。</span><span class="sxs-lookup"><span data-stu-id="b45df-201">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="b45df-202">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-202">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-203">proxySetting</span><span class="sxs-lookup"><span data-stu-id="b45df-203">proxySetting</span></span>|[<span data-ttu-id="b45df-204">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="b45df-204">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="b45df-205">指定从[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)设置 Wi-fi 配置继承的代理。</span><span class="sxs-lookup"><span data-stu-id="b45df-205">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="b45df-206">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="b45df-206">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="b45df-207">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="b45df-207">proxyManualAddress</span></span>|<span data-ttu-id="b45df-208">String</span><span class="sxs-lookup"><span data-stu-id="b45df-208">String</span></span>|<span data-ttu-id="b45df-209">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b45df-209">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="b45df-210">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-211">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="b45df-211">proxyManualPort</span></span>|<span data-ttu-id="b45df-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b45df-212">Int32</span></span>|<span data-ttu-id="b45df-213">指定的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="b45df-213">Specify the port for the proxy server.</span></span> <span data-ttu-id="b45df-214">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-215">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b45df-215">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b45df-216">String</span><span class="sxs-lookup"><span data-stu-id="b45df-216">String</span></span>|<span data-ttu-id="b45df-217">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="b45df-217">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="b45df-218">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-218">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="b45df-219">forceFIPSCompliance</span></span>|<span data-ttu-id="b45df-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-220">Boolean</span></span>|<span data-ttu-id="b45df-221">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="b45df-221">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="b45df-222">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b45df-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="b45df-223">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="b45df-223">networkSingleSignOn</span></span>|[<span data-ttu-id="b45df-224">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="b45df-224">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="b45df-225">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="b45df-225">Specify the network single sign on type.</span></span> <span data-ttu-id="b45df-226">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="b45df-226">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="b45df-227">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b45df-227">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="b45df-228">Int32</span><span class="sxs-lookup"><span data-stu-id="b45df-228">Int32</span></span>|<span data-ttu-id="b45df-229">指定最大的身份验证超时 （以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b45df-229">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="b45df-230">有效的范围： 1-120</span><span class="sxs-lookup"><span data-stu-id="b45df-230">Valid range: 1-120</span></span>|
|<span data-ttu-id="b45df-231">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="b45df-231">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="b45df-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-232">Boolean</span></span>|<span data-ttu-id="b45df-233">指定 wifi 连接是否应提示其他身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="b45df-233">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="b45df-234">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="b45df-234">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="b45df-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-235">Boolean</span></span>|<span data-ttu-id="b45df-236">指定 wifi 连接是否应启用缓存成对的主密钥。</span><span class="sxs-lookup"><span data-stu-id="b45df-236">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="b45df-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="b45df-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="b45df-238">Int32</span><span class="sxs-lookup"><span data-stu-id="b45df-238">Int32</span></span>|<span data-ttu-id="b45df-239">指定最大成对主密钥缓存时间 （以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="b45df-239">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="b45df-240">有效的范围： 5 1440年</span><span class="sxs-lookup"><span data-stu-id="b45df-240">Valid range: 5-1440</span></span>|
|<span data-ttu-id="b45df-241">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="b45df-241">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="b45df-242">Int32</span><span class="sxs-lookup"><span data-stu-id="b45df-242">Int32</span></span>|<span data-ttu-id="b45df-243">在缓存中指定成对的主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="b45df-243">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="b45df-244">有效的范围： 1 到 255</span><span class="sxs-lookup"><span data-stu-id="b45df-244">Valid range: 1-255</span></span>|
|<span data-ttu-id="b45df-245">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="b45df-245">enablePreAuthentication</span></span>|<span data-ttu-id="b45df-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b45df-246">Boolean</span></span>|<span data-ttu-id="b45df-247">指定是否应启用预身份验证。</span><span class="sxs-lookup"><span data-stu-id="b45df-247">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="b45df-248">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="b45df-248">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="b45df-249">Int32</span><span class="sxs-lookup"><span data-stu-id="b45df-249">Int32</span></span>|<span data-ttu-id="b45df-250">指定最大预身份验证尝试。</span><span class="sxs-lookup"><span data-stu-id="b45df-250">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="b45df-251">有效的范围： 1-16</span><span class="sxs-lookup"><span data-stu-id="b45df-251">Valid range: 1-16</span></span>|
|<span data-ttu-id="b45df-252">eapType</span><span class="sxs-lookup"><span data-stu-id="b45df-252">eapType</span></span>|[<span data-ttu-id="b45df-253">eapType</span><span class="sxs-lookup"><span data-stu-id="b45df-253">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="b45df-254">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="b45df-254">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="b45df-255">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="b45df-255">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="b45df-256">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="b45df-256">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="b45df-257">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="b45df-257">trustedServerCertificateNames</span></span>|<span data-ttu-id="b45df-258">String 集合</span><span class="sxs-lookup"><span data-stu-id="b45df-258">String collection</span></span>|<span data-ttu-id="b45df-259">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="b45df-259">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="b45df-260">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b45df-260">authenticationMethod</span></span>|[<span data-ttu-id="b45df-261">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b45df-261">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="b45df-262">指定的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b45df-262">Specify the authentication method.</span></span> <span data-ttu-id="b45df-263">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="b45df-263">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b45df-264">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="b45df-264">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="b45df-265">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="b45df-265">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="b45df-266">指定 EAP TTL 内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="b45df-266">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="b45df-267">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="b45df-267">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b45df-268">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="b45df-268">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="b45df-269">String</span><span class="sxs-lookup"><span data-stu-id="b45df-269">String</span></span>|<span data-ttu-id="b45df-270">指定要使用 EAP TTL 或 PEAP 时替换为隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="b45df-270">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="b45df-271">响应</span><span class="sxs-lookup"><span data-stu-id="b45df-271">Response</span></span>
<span data-ttu-id="b45df-272">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b45df-272">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b45df-273">示例</span><span class="sxs-lookup"><span data-stu-id="b45df-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="b45df-274">请求</span><span class="sxs-lookup"><span data-stu-id="b45df-274">Request</span></span>
<span data-ttu-id="b45df-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b45df-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b45df-276">响应</span><span class="sxs-lookup"><span data-stu-id="b45df-276">Response</span></span>
<span data-ttu-id="b45df-p132">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b45df-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




