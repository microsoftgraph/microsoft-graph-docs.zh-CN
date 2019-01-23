---
title: 更新 iosEnterpriseWiFiConfiguration
description: 更新 iosEnterpriseWiFiConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4b39513693c1531628989b25e679056aab6a5c0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402116"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="23d57-103">更新 iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="23d57-103">Update iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="23d57-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="23d57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23d57-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23d57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23d57-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23d57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23d57-107">更新[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23d57-107">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23d57-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="23d57-108">Prerequisites</span></span>
<span data-ttu-id="23d57-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="23d57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23d57-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="23d57-111">Permission type</span></span>|<span data-ttu-id="23d57-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="23d57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23d57-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23d57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23d57-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23d57-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23d57-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23d57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23d57-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="23d57-116">Not supported.</span></span>|
|<span data-ttu-id="23d57-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="23d57-117">Application</span></span>|<span data-ttu-id="23d57-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="23d57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23d57-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23d57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="23d57-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="23d57-120">Request headers</span></span>
|<span data-ttu-id="23d57-121">标头</span><span class="sxs-lookup"><span data-stu-id="23d57-121">Header</span></span>|<span data-ttu-id="23d57-122">值</span><span class="sxs-lookup"><span data-stu-id="23d57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23d57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23d57-123">Authorization</span></span>|<span data-ttu-id="23d57-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="23d57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23d57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23d57-125">Accept</span></span>|<span data-ttu-id="23d57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23d57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23d57-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="23d57-127">Request body</span></span>
<span data-ttu-id="23d57-128">在请求正文中，提供[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23d57-128">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="23d57-129">下表显示时创建[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="23d57-129">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="23d57-130">属性</span><span class="sxs-lookup"><span data-stu-id="23d57-130">Property</span></span>|<span data-ttu-id="23d57-131">类型</span><span class="sxs-lookup"><span data-stu-id="23d57-131">Type</span></span>|<span data-ttu-id="23d57-132">说明</span><span class="sxs-lookup"><span data-stu-id="23d57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23d57-133">id</span><span class="sxs-lookup"><span data-stu-id="23d57-133">id</span></span>|<span data-ttu-id="23d57-134">String</span><span class="sxs-lookup"><span data-stu-id="23d57-134">String</span></span>|<span data-ttu-id="23d57-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="23d57-135">Key of the entity.</span></span> <span data-ttu-id="23d57-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23d57-137">lastModifiedDateTime</span></span>|<span data-ttu-id="23d57-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d57-138">DateTimeOffset</span></span>|<span data-ttu-id="23d57-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="23d57-139">DateTime the object was last modified.</span></span> <span data-ttu-id="23d57-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23d57-141">roleScopeTagIds</span></span>|<span data-ttu-id="23d57-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="23d57-142">String collection</span></span>|<span data-ttu-id="23d57-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="23d57-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23d57-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23d57-145">supportsScopeTags</span></span>|<span data-ttu-id="23d57-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d57-146">Boolean</span></span>|<span data-ttu-id="23d57-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="23d57-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23d57-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="23d57-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23d57-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="23d57-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23d57-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="23d57-150">This property is read-only.</span></span> <span data-ttu-id="23d57-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23d57-152">createdDateTime</span></span>|<span data-ttu-id="23d57-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d57-153">DateTimeOffset</span></span>|<span data-ttu-id="23d57-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="23d57-154">DateTime the object was created.</span></span> <span data-ttu-id="23d57-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-156">description</span><span class="sxs-lookup"><span data-stu-id="23d57-156">description</span></span>|<span data-ttu-id="23d57-157">String</span><span class="sxs-lookup"><span data-stu-id="23d57-157">String</span></span>|<span data-ttu-id="23d57-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="23d57-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23d57-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-160">displayName</span><span class="sxs-lookup"><span data-stu-id="23d57-160">displayName</span></span>|<span data-ttu-id="23d57-161">String</span><span class="sxs-lookup"><span data-stu-id="23d57-161">String</span></span>|<span data-ttu-id="23d57-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="23d57-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23d57-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-164">version</span><span class="sxs-lookup"><span data-stu-id="23d57-164">version</span></span>|<span data-ttu-id="23d57-165">Int32</span><span class="sxs-lookup"><span data-stu-id="23d57-165">Int32</span></span>|<span data-ttu-id="23d57-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="23d57-166">Version of the device configuration.</span></span> <span data-ttu-id="23d57-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d57-168">networkName</span><span class="sxs-lookup"><span data-stu-id="23d57-168">networkName</span></span>|<span data-ttu-id="23d57-169">String</span><span class="sxs-lookup"><span data-stu-id="23d57-169">String</span></span>|<span data-ttu-id="23d57-170">网络名称继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-170">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-171">ssid</span><span class="sxs-lookup"><span data-stu-id="23d57-171">ssid</span></span>|<span data-ttu-id="23d57-172">String</span><span class="sxs-lookup"><span data-stu-id="23d57-172">String</span></span>|<span data-ttu-id="23d57-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="23d57-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="23d57-174">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-174">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="23d57-175">connectAutomatically</span></span>|<span data-ttu-id="23d57-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d57-176">Boolean</span></span>|<span data-ttu-id="23d57-177">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="23d57-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="23d57-178">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="23d57-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="23d57-179">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-179">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="23d57-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="23d57-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d57-181">Boolean</span></span>|<span data-ttu-id="23d57-182">网络未进行广播其名称 (SSID) 连接。</span><span class="sxs-lookup"><span data-stu-id="23d57-182">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="23d57-183">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="23d57-183">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="23d57-184">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-184">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="23d57-185">wiFiSecurityType</span></span>|[<span data-ttu-id="23d57-186">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="23d57-186">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="23d57-187">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="23d57-187">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="23d57-188">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="23d57-188">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="23d57-189">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="23d57-189">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="23d57-190">proxySettings</span><span class="sxs-lookup"><span data-stu-id="23d57-190">proxySettings</span></span>|[<span data-ttu-id="23d57-191">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="23d57-191">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="23d57-192">代理类型从[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)此 Wi-fi 连接继承的。</span><span class="sxs-lookup"><span data-stu-id="23d57-192">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="23d57-193">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="23d57-193">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="23d57-194">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="23d57-194">proxyManualAddress</span></span>|<span data-ttu-id="23d57-195">String</span><span class="sxs-lookup"><span data-stu-id="23d57-195">String</span></span>|<span data-ttu-id="23d57-196">选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="23d57-196">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="23d57-197">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-197">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-198">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="23d57-198">proxyManualPort</span></span>|<span data-ttu-id="23d57-199">Int32</span><span class="sxs-lookup"><span data-stu-id="23d57-199">Int32</span></span>|<span data-ttu-id="23d57-200">选择手动配置时的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="23d57-200">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="23d57-201">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-201">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-202">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="23d57-202">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="23d57-203">String</span><span class="sxs-lookup"><span data-stu-id="23d57-203">String</span></span>|<span data-ttu-id="23d57-204">代理服务器自动配置脚本时选择了自动配置的 URL。</span><span class="sxs-lookup"><span data-stu-id="23d57-204">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="23d57-205">此 URL 通常是 PAC （代理自动配置） 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="23d57-205">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="23d57-206">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-206">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-207">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="23d57-207">preSharedKey</span></span>|<span data-ttu-id="23d57-208">String</span><span class="sxs-lookup"><span data-stu-id="23d57-208">String</span></span>|<span data-ttu-id="23d57-209">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="23d57-209">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="23d57-210">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23d57-210">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="23d57-211">eapType</span><span class="sxs-lookup"><span data-stu-id="23d57-211">eapType</span></span>|[<span data-ttu-id="23d57-212">eapType</span><span class="sxs-lookup"><span data-stu-id="23d57-212">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="23d57-213">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="23d57-213">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="23d57-214">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="23d57-214">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="23d57-215">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="23d57-215">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="23d57-216">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="23d57-216">eapFastConfiguration</span></span>|[<span data-ttu-id="23d57-217">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="23d57-217">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="23d57-218">EAP FAST 配置选项时 EAP FAST 是所选的 EAP 类型。</span><span class="sxs-lookup"><span data-stu-id="23d57-218">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="23d57-219">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="23d57-219">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="23d57-220">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="23d57-220">trustedServerCertificateNames</span></span>|<span data-ttu-id="23d57-221">String 集合</span><span class="sxs-lookup"><span data-stu-id="23d57-221">String collection</span></span>|<span data-ttu-id="23d57-222">当 EAP 类型配置为 EAP-TLS/TTL/FAST 或 PEAP 受信任服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="23d57-222">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="23d57-223">这是您的受信任的证书颁发机构 (CA) 颁发的证书中使用的通用名称。</span><span class="sxs-lookup"><span data-stu-id="23d57-223">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="23d57-224">如果您提供此信息，您可以跳过它们连接到此 Wi-fi 网络时，最终用户的设备显示动态信任对话框。</span><span class="sxs-lookup"><span data-stu-id="23d57-224">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="23d57-225">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="23d57-225">authenticationMethod</span></span>|[<span data-ttu-id="23d57-226">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="23d57-226">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="23d57-227">当 EAP 类型配置为 PEAP 或 EAP TTL 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="23d57-227">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="23d57-228">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="23d57-228">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="23d57-229">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="23d57-229">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="23d57-230">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="23d57-230">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="23d57-231">用于身份验证 EAP TTL 并 Authenticationmethod EAP 类型时的非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="23d57-231">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="23d57-232">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="23d57-232">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="23d57-233">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="23d57-233">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="23d57-234">String</span><span class="sxs-lookup"><span data-stu-id="23d57-234">String</span></span>|<span data-ttu-id="23d57-235">时 EAP 类型配置为 EAP-TTL，EAP-启用标识隐私 （外部标识） FAST 或 PEAP。</span><span class="sxs-lookup"><span data-stu-id="23d57-235">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="23d57-236">此属性将屏蔽用户名与您输入的文本。</span><span class="sxs-lookup"><span data-stu-id="23d57-236">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="23d57-237">例如，如果您使用匿名，每个与使用其实际用户名此 Wi-fi 连接进行身份验证的用户显示为匿名。</span><span class="sxs-lookup"><span data-stu-id="23d57-237">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="23d57-238">响应</span><span class="sxs-lookup"><span data-stu-id="23d57-238">Response</span></span>
<span data-ttu-id="23d57-239">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23d57-239">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23d57-240">示例</span><span class="sxs-lookup"><span data-stu-id="23d57-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="23d57-241">请求</span><span class="sxs-lookup"><span data-stu-id="23d57-241">Request</span></span>
<span data-ttu-id="23d57-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23d57-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1083

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="23d57-243">响应</span><span class="sxs-lookup"><span data-stu-id="23d57-243">Response</span></span>
<span data-ttu-id="23d57-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23d57-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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




