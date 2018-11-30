---
title: 更新 macOSEnterpriseWiFiConfiguration
description: 更新 macOSEnterpriseWiFiConfiguration 对象的属性。
ms.openlocfilehash: becaa5ab8597621c2cb89a1bfc79112474ed3e75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046306"
---
# <a name="update-macosenterprisewificonfiguration"></a><span data-ttu-id="e75d4-103">更新 macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e75d4-103">Update macOSEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="e75d4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e75d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e75d4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e75d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e75d4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e75d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e75d4-107">更新[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e75d4-107">Update the properties of a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e75d4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e75d4-108">Prerequisites</span></span>
<span data-ttu-id="e75d4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e75d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e75d4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e75d4-111">Permission type</span></span>|<span data-ttu-id="e75d4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e75d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e75d4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e75d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e75d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e75d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e75d4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e75d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e75d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e75d4-116">Not supported.</span></span>|
|<span data-ttu-id="e75d4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e75d4-117">Application</span></span>|<span data-ttu-id="e75d4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e75d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e75d4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e75d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e75d4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e75d4-120">Request headers</span></span>
|<span data-ttu-id="e75d4-121">标头</span><span class="sxs-lookup"><span data-stu-id="e75d4-121">Header</span></span>|<span data-ttu-id="e75d4-122">值</span><span class="sxs-lookup"><span data-stu-id="e75d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e75d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e75d4-123">Authorization</span></span>|<span data-ttu-id="e75d4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e75d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e75d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e75d4-125">Accept</span></span>|<span data-ttu-id="e75d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e75d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e75d4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e75d4-127">Request body</span></span>
<span data-ttu-id="e75d4-128">在请求正文中，提供[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e75d4-128">In the request body, supply a JSON representation for the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="e75d4-129">下表显示时创建[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e75d4-129">The following table shows the properties that are required when you create the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="e75d4-130">属性</span><span class="sxs-lookup"><span data-stu-id="e75d4-130">Property</span></span>|<span data-ttu-id="e75d4-131">类型</span><span class="sxs-lookup"><span data-stu-id="e75d4-131">Type</span></span>|<span data-ttu-id="e75d4-132">说明</span><span class="sxs-lookup"><span data-stu-id="e75d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75d4-133">id</span><span class="sxs-lookup"><span data-stu-id="e75d4-133">id</span></span>|<span data-ttu-id="e75d4-134">String</span><span class="sxs-lookup"><span data-stu-id="e75d4-134">String</span></span>|<span data-ttu-id="e75d4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e75d4-135">Key of the entity.</span></span> <span data-ttu-id="e75d4-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e75d4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e75d4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e75d4-138">DateTimeOffset</span></span>|<span data-ttu-id="e75d4-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e75d4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e75d4-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e75d4-141">roleScopeTagIds</span></span>|<span data-ttu-id="e75d4-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e75d4-142">String collection</span></span>|<span data-ttu-id="e75d4-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="e75d4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e75d4-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e75d4-145">supportsScopeTags</span></span>|<span data-ttu-id="e75d4-146">布尔</span><span class="sxs-lookup"><span data-stu-id="e75d4-146">Boolean</span></span>|<span data-ttu-id="e75d4-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="e75d4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e75d4-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="e75d4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e75d4-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="e75d4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e75d4-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e75d4-150">This property is read-only.</span></span> <span data-ttu-id="e75d4-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e75d4-152">createdDateTime</span></span>|<span data-ttu-id="e75d4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e75d4-153">DateTimeOffset</span></span>|<span data-ttu-id="e75d4-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e75d4-154">DateTime the object was created.</span></span> <span data-ttu-id="e75d4-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-156">description</span><span class="sxs-lookup"><span data-stu-id="e75d4-156">description</span></span>|<span data-ttu-id="e75d4-157">String</span><span class="sxs-lookup"><span data-stu-id="e75d4-157">String</span></span>|<span data-ttu-id="e75d4-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e75d4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e75d4-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e75d4-160">displayName</span></span>|<span data-ttu-id="e75d4-161">String</span><span class="sxs-lookup"><span data-stu-id="e75d4-161">String</span></span>|<span data-ttu-id="e75d4-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e75d4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e75d4-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-164">version</span><span class="sxs-lookup"><span data-stu-id="e75d4-164">version</span></span>|<span data-ttu-id="e75d4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e75d4-165">Int32</span></span>|<span data-ttu-id="e75d4-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e75d4-166">Version of the device configuration.</span></span> <span data-ttu-id="e75d4-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-168">networkName</span><span class="sxs-lookup"><span data-stu-id="e75d4-168">networkName</span></span>|<span data-ttu-id="e75d4-169">字符串</span><span class="sxs-lookup"><span data-stu-id="e75d4-169">String</span></span>|<span data-ttu-id="e75d4-170">网络名称继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-170">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-171">ssid</span><span class="sxs-lookup"><span data-stu-id="e75d4-171">ssid</span></span>|<span data-ttu-id="e75d4-172">字符串</span><span class="sxs-lookup"><span data-stu-id="e75d4-172">String</span></span>|<span data-ttu-id="e75d4-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="e75d4-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="e75d4-174">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-174">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e75d4-175">connectAutomatically</span></span>|<span data-ttu-id="e75d4-176">布尔</span><span class="sxs-lookup"><span data-stu-id="e75d4-176">Boolean</span></span>|<span data-ttu-id="e75d4-177">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="e75d4-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="e75d4-178">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="e75d4-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="e75d4-179">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-179">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e75d4-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e75d4-181">布尔</span><span class="sxs-lookup"><span data-stu-id="e75d4-181">Boolean</span></span>|<span data-ttu-id="e75d4-182">网络未进行广播其名称 (SSID) 连接。</span><span class="sxs-lookup"><span data-stu-id="e75d4-182">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="e75d4-183">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="e75d4-183">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="e75d4-184">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-184">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e75d4-185">wiFiSecurityType</span></span>|[<span data-ttu-id="e75d4-186">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e75d4-186">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e75d4-187">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="e75d4-187">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="e75d4-188">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="e75d4-188">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="e75d4-189">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="e75d4-189">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e75d4-190">proxySettings</span><span class="sxs-lookup"><span data-stu-id="e75d4-190">proxySettings</span></span>|[<span data-ttu-id="e75d4-191">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e75d4-191">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e75d4-192">代理类型从[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)此 Wi-fi 连接继承的。</span><span class="sxs-lookup"><span data-stu-id="e75d4-192">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="e75d4-193">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="e75d4-193">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e75d4-194">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e75d4-194">proxyManualAddress</span></span>|<span data-ttu-id="e75d4-195">字符串</span><span class="sxs-lookup"><span data-stu-id="e75d4-195">String</span></span>|<span data-ttu-id="e75d4-196">选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="e75d4-196">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="e75d4-197">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-197">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-198">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e75d4-198">proxyManualPort</span></span>|<span data-ttu-id="e75d4-199">Int32</span><span class="sxs-lookup"><span data-stu-id="e75d4-199">Int32</span></span>|<span data-ttu-id="e75d4-200">选择手动配置时的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="e75d4-200">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="e75d4-201">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-201">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-202">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e75d4-202">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e75d4-203">字符串</span><span class="sxs-lookup"><span data-stu-id="e75d4-203">String</span></span>|<span data-ttu-id="e75d4-204">代理服务器自动配置脚本时选择了自动配置的 URL。</span><span class="sxs-lookup"><span data-stu-id="e75d4-204">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="e75d4-205">此 URL 通常是 PAC （代理自动配置） 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="e75d4-205">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="e75d4-206">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-206">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-207">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e75d4-207">preSharedKey</span></span>|<span data-ttu-id="e75d4-208">字符串</span><span class="sxs-lookup"><span data-stu-id="e75d4-208">String</span></span>|<span data-ttu-id="e75d4-209">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="e75d4-209">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="e75d4-210">继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e75d4-210">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="e75d4-211">eapType</span><span class="sxs-lookup"><span data-stu-id="e75d4-211">eapType</span></span>|[<span data-ttu-id="e75d4-212">eapType</span><span class="sxs-lookup"><span data-stu-id="e75d4-212">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="e75d4-213">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="e75d4-213">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="e75d4-214">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="e75d4-214">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="e75d4-215">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="e75d4-215">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="e75d4-216">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="e75d4-216">eapFastConfiguration</span></span>|[<span data-ttu-id="e75d4-217">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="e75d4-217">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="e75d4-218">EAP FAST 配置选项时 EAP FAST 是所选的 EAP 类型。</span><span class="sxs-lookup"><span data-stu-id="e75d4-218">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="e75d4-219">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="e75d4-219">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="e75d4-220">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="e75d4-220">trustedServerCertificateNames</span></span>|<span data-ttu-id="e75d4-221">String 集合</span><span class="sxs-lookup"><span data-stu-id="e75d4-221">String collection</span></span>|<span data-ttu-id="e75d4-222">当 EAP 类型配置为 EAP-TLS/TTL/FAST 或 PEAP 受信任服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="e75d4-222">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="e75d4-223">这是您的受信任的证书颁发机构 (CA) 颁发的证书中使用的通用名称。</span><span class="sxs-lookup"><span data-stu-id="e75d4-223">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="e75d4-224">如果您提供此信息，您可以跳过它们连接到此 Wi-fi 网络时，最终用户设备显示动态信任对话框。</span><span class="sxs-lookup"><span data-stu-id="e75d4-224">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="e75d4-225">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e75d4-225">authenticationMethod</span></span>|[<span data-ttu-id="e75d4-226">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e75d4-226">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="e75d4-227">当 EAP 类型配置为 PEAP 或 EAP TTL 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="e75d4-227">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="e75d4-228">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="e75d4-228">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="e75d4-229">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="e75d4-229">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="e75d4-230">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="e75d4-230">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="e75d4-231">身份验证 （内部标识） EAP 类型时 EAP TTL 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="e75d4-231">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="e75d4-232">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="e75d4-232">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="e75d4-233">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="e75d4-233">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="e75d4-234">字符串</span><span class="sxs-lookup"><span data-stu-id="e75d4-234">String</span></span>|<span data-ttu-id="e75d4-235">到 EAP TTL、 EAP FAST 或 PEAP 配置 EAP 类型时启用标识隐私 （外部标识）。</span><span class="sxs-lookup"><span data-stu-id="e75d4-235">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="e75d4-236">此属性将屏蔽用户名与您输入的文本。</span><span class="sxs-lookup"><span data-stu-id="e75d4-236">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="e75d4-237">例如，如果您使用匿名，每个与使用其实际用户名此 Wi-fi 连接进行身份验证的用户显示为匿名。</span><span class="sxs-lookup"><span data-stu-id="e75d4-237">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="e75d4-238">响应</span><span class="sxs-lookup"><span data-stu-id="e75d4-238">Response</span></span>
<span data-ttu-id="e75d4-239">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e75d4-239">If successful, this method returns a `200 OK` response code and an updated [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e75d4-240">示例</span><span class="sxs-lookup"><span data-stu-id="e75d4-240">Example</span></span>
### <a name="request"></a><span data-ttu-id="e75d4-241">请求</span><span class="sxs-lookup"><span data-stu-id="e75d4-241">Request</span></span>
<span data-ttu-id="e75d4-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e75d4-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1078

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e75d4-243">响应</span><span class="sxs-lookup"><span data-stu-id="e75d4-243">Response</span></span>
<span data-ttu-id="e75d4-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e75d4-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





