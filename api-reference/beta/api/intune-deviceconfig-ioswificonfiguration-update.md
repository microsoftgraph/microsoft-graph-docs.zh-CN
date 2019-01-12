---
title: 更新 iosWiFiConfiguration
description: 更新 iosWiFiConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1023601ee93b4419830bb3fc27f33b80d7386a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978443"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="0af5d-103">更新 iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0af5d-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="0af5d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0af5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0af5d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0af5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0af5d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0af5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0af5d-107">更新[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0af5d-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0af5d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0af5d-108">Prerequisites</span></span>
<span data-ttu-id="0af5d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0af5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af5d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0af5d-111">Permission type</span></span>|<span data-ttu-id="0af5d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0af5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0af5d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0af5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0af5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0af5d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0af5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0af5d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af5d-116">Not supported.</span></span>|
|<span data-ttu-id="0af5d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0af5d-117">Application</span></span>|<span data-ttu-id="0af5d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af5d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0af5d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0af5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0af5d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0af5d-120">Request headers</span></span>
|<span data-ttu-id="0af5d-121">标头</span><span class="sxs-lookup"><span data-stu-id="0af5d-121">Header</span></span>|<span data-ttu-id="0af5d-122">值</span><span class="sxs-lookup"><span data-stu-id="0af5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0af5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af5d-123">Authorization</span></span>|<span data-ttu-id="0af5d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0af5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0af5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0af5d-125">Accept</span></span>|<span data-ttu-id="0af5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0af5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af5d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0af5d-127">Request body</span></span>
<span data-ttu-id="0af5d-128">在请求正文中，提供[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0af5d-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="0af5d-129">下表显示时创建[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0af5d-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="0af5d-130">属性</span><span class="sxs-lookup"><span data-stu-id="0af5d-130">Property</span></span>|<span data-ttu-id="0af5d-131">类型</span><span class="sxs-lookup"><span data-stu-id="0af5d-131">Type</span></span>|<span data-ttu-id="0af5d-132">说明</span><span class="sxs-lookup"><span data-stu-id="0af5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af5d-133">id</span><span class="sxs-lookup"><span data-stu-id="0af5d-133">id</span></span>|<span data-ttu-id="0af5d-134">String</span><span class="sxs-lookup"><span data-stu-id="0af5d-134">String</span></span>|<span data-ttu-id="0af5d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0af5d-135">Key of the entity.</span></span> <span data-ttu-id="0af5d-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0af5d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0af5d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0af5d-138">DateTimeOffset</span></span>|<span data-ttu-id="0af5d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0af5d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0af5d-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0af5d-141">roleScopeTagIds</span></span>|<span data-ttu-id="0af5d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0af5d-142">String collection</span></span>|<span data-ttu-id="0af5d-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0af5d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0af5d-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0af5d-145">supportsScopeTags</span></span>|<span data-ttu-id="0af5d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0af5d-146">Boolean</span></span>|<span data-ttu-id="0af5d-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0af5d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0af5d-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0af5d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0af5d-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0af5d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0af5d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0af5d-150">This property is read-only.</span></span> <span data-ttu-id="0af5d-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0af5d-152">createdDateTime</span></span>|<span data-ttu-id="0af5d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0af5d-153">DateTimeOffset</span></span>|<span data-ttu-id="0af5d-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0af5d-154">DateTime the object was created.</span></span> <span data-ttu-id="0af5d-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-156">description</span><span class="sxs-lookup"><span data-stu-id="0af5d-156">description</span></span>|<span data-ttu-id="0af5d-157">String</span><span class="sxs-lookup"><span data-stu-id="0af5d-157">String</span></span>|<span data-ttu-id="0af5d-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0af5d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0af5d-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0af5d-160">displayName</span></span>|<span data-ttu-id="0af5d-161">String</span><span class="sxs-lookup"><span data-stu-id="0af5d-161">String</span></span>|<span data-ttu-id="0af5d-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0af5d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0af5d-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-164">version</span><span class="sxs-lookup"><span data-stu-id="0af5d-164">version</span></span>|<span data-ttu-id="0af5d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0af5d-165">Int32</span></span>|<span data-ttu-id="0af5d-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0af5d-166">Version of the device configuration.</span></span> <span data-ttu-id="0af5d-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0af5d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0af5d-168">networkName</span><span class="sxs-lookup"><span data-stu-id="0af5d-168">networkName</span></span>|<span data-ttu-id="0af5d-169">字符串</span><span class="sxs-lookup"><span data-stu-id="0af5d-169">String</span></span>|<span data-ttu-id="0af5d-170">网络名称</span><span class="sxs-lookup"><span data-stu-id="0af5d-170">Network Name</span></span>|
|<span data-ttu-id="0af5d-171">ssid</span><span class="sxs-lookup"><span data-stu-id="0af5d-171">ssid</span></span>|<span data-ttu-id="0af5d-172">字符串</span><span class="sxs-lookup"><span data-stu-id="0af5d-172">String</span></span>|<span data-ttu-id="0af5d-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="0af5d-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="0af5d-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0af5d-174">connectAutomatically</span></span>|<span data-ttu-id="0af5d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0af5d-175">Boolean</span></span>|<span data-ttu-id="0af5d-176">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="0af5d-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0af5d-177">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="0af5d-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="0af5d-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0af5d-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0af5d-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="0af5d-179">Boolean</span></span>|<span data-ttu-id="0af5d-180">网络未进行广播其名称 (SSID) 连接。</span><span class="sxs-lookup"><span data-stu-id="0af5d-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="0af5d-181">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="0af5d-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="0af5d-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0af5d-182">wiFiSecurityType</span></span>|[<span data-ttu-id="0af5d-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0af5d-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="0af5d-184">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="0af5d-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0af5d-185">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="0af5d-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="0af5d-186">proxySettings</span><span class="sxs-lookup"><span data-stu-id="0af5d-186">proxySettings</span></span>|[<span data-ttu-id="0af5d-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="0af5d-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="0af5d-188">此 Wi-fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="0af5d-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="0af5d-189">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="0af5d-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="0af5d-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="0af5d-190">proxyManualAddress</span></span>|<span data-ttu-id="0af5d-191">字符串</span><span class="sxs-lookup"><span data-stu-id="0af5d-191">String</span></span>|<span data-ttu-id="0af5d-192">选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="0af5d-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="0af5d-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="0af5d-193">proxyManualPort</span></span>|<span data-ttu-id="0af5d-194">Int32</span><span class="sxs-lookup"><span data-stu-id="0af5d-194">Int32</span></span>|<span data-ttu-id="0af5d-195">选择手动配置时的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="0af5d-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="0af5d-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="0af5d-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="0af5d-197">字符串</span><span class="sxs-lookup"><span data-stu-id="0af5d-197">String</span></span>|<span data-ttu-id="0af5d-198">代理服务器自动配置脚本时选择了自动配置的 URL。</span><span class="sxs-lookup"><span data-stu-id="0af5d-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="0af5d-199">此 URL 通常是 PAC （代理自动配置） 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="0af5d-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="0af5d-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0af5d-200">preSharedKey</span></span>|<span data-ttu-id="0af5d-201">字符串</span><span class="sxs-lookup"><span data-stu-id="0af5d-201">String</span></span>|<span data-ttu-id="0af5d-202">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="0af5d-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="0af5d-203">响应</span><span class="sxs-lookup"><span data-stu-id="0af5d-203">Response</span></span>
<span data-ttu-id="0af5d-204">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0af5d-204">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0af5d-205">示例</span><span class="sxs-lookup"><span data-stu-id="0af5d-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="0af5d-206">请求</span><span class="sxs-lookup"><span data-stu-id="0af5d-206">Request</span></span>
<span data-ttu-id="0af5d-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0af5d-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 680

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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="0af5d-208">响应</span><span class="sxs-lookup"><span data-stu-id="0af5d-208">Response</span></span>
<span data-ttu-id="0af5d-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0af5d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 847

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "preSharedKey": "Pre Shared Key value"
}
```





