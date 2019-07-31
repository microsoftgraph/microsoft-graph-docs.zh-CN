---
title: 创建 windowsWifiEnterpriseEAPConfiguration
description: 创建新的 windowsWifiEnterpriseEAPConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3f832c62adddfabadb1f9f749269d396a8c1a51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981820"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="c4153-103">创建 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4153-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="c4153-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4153-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4153-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4153-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4153-106">创建新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c4153-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4153-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c4153-107">Prerequisites</span></span>
<span data-ttu-id="c4153-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4153-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4153-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4153-110">Permission type</span></span>|<span data-ttu-id="c4153-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c4153-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4153-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4153-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4153-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4153-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4153-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4153-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4153-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4153-115">Not supported.</span></span>|
|<span data-ttu-id="c4153-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4153-116">Application</span></span>|<span data-ttu-id="c4153-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4153-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4153-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4153-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c4153-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4153-119">Request headers</span></span>
|<span data-ttu-id="c4153-120">标头</span><span class="sxs-lookup"><span data-stu-id="c4153-120">Header</span></span>|<span data-ttu-id="c4153-121">值</span><span class="sxs-lookup"><span data-stu-id="c4153-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4153-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4153-122">Authorization</span></span>|<span data-ttu-id="c4153-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c4153-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4153-124">接受</span><span class="sxs-lookup"><span data-stu-id="c4153-124">Accept</span></span>|<span data-ttu-id="c4153-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4153-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4153-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4153-126">Request body</span></span>
<span data-ttu-id="c4153-127">在请求正文中, 提供 windowsWifiEnterpriseEAPConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4153-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="c4153-128">下表显示创建 windowsWifiEnterpriseEAPConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c4153-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="c4153-129">属性</span><span class="sxs-lookup"><span data-stu-id="c4153-129">Property</span></span>|<span data-ttu-id="c4153-130">类型</span><span class="sxs-lookup"><span data-stu-id="c4153-130">Type</span></span>|<span data-ttu-id="c4153-131">说明</span><span class="sxs-lookup"><span data-stu-id="c4153-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4153-132">id</span><span class="sxs-lookup"><span data-stu-id="c4153-132">id</span></span>|<span data-ttu-id="c4153-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c4153-133">String</span></span>|<span data-ttu-id="c4153-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c4153-134">Key of the entity.</span></span> <span data-ttu-id="c4153-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4153-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c4153-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4153-137">DateTimeOffset</span></span>|<span data-ttu-id="c4153-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c4153-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c4153-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4153-140">roleScopeTagIds</span></span>|<span data-ttu-id="c4153-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c4153-141">String collection</span></span>|<span data-ttu-id="c4153-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c4153-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4153-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4153-144">supportsScopeTags</span></span>|<span data-ttu-id="c4153-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-145">Boolean</span></span>|<span data-ttu-id="c4153-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c4153-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4153-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c4153-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4153-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c4153-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4153-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c4153-149">This property is read-only.</span></span> <span data-ttu-id="c4153-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4153-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c4153-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4153-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c4153-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c4153-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c4153-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4153-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c4153-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4153-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c4153-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c4153-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c4153-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4153-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c4153-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4153-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c4153-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c4153-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c4153-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4153-163">createdDateTime</span></span>|<span data-ttu-id="c4153-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4153-164">DateTimeOffset</span></span>|<span data-ttu-id="c4153-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c4153-165">DateTime the object was created.</span></span> <span data-ttu-id="c4153-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-167">说明</span><span class="sxs-lookup"><span data-stu-id="c4153-167">description</span></span>|<span data-ttu-id="c4153-168">String</span><span class="sxs-lookup"><span data-stu-id="c4153-168">String</span></span>|<span data-ttu-id="c4153-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c4153-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4153-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c4153-171">displayName</span></span>|<span data-ttu-id="c4153-172">String</span><span class="sxs-lookup"><span data-stu-id="c4153-172">String</span></span>|<span data-ttu-id="c4153-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c4153-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4153-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-175">version</span><span class="sxs-lookup"><span data-stu-id="c4153-175">version</span></span>|<span data-ttu-id="c4153-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c4153-176">Int32</span></span>|<span data-ttu-id="c4153-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c4153-177">Version of the device configuration.</span></span> <span data-ttu-id="c4153-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4153-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="c4153-179">preSharedKey</span></span>|<span data-ttu-id="c4153-180">String</span><span class="sxs-lookup"><span data-stu-id="c4153-180">String</span></span>|<span data-ttu-id="c4153-181">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="c4153-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="c4153-182">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c4153-183">wifiSecurityType</span></span>|[<span data-ttu-id="c4153-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c4153-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c4153-185">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="c4153-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="c4153-186">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c4153-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c4153-187">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="c4153-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c4153-188">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="c4153-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="c4153-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="c4153-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="c4153-190">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="c4153-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="c4153-191">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c4153-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c4153-192">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="c4153-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="c4153-193">ssid</span><span class="sxs-lookup"><span data-stu-id="c4153-193">ssid</span></span>|<span data-ttu-id="c4153-194">String</span><span class="sxs-lookup"><span data-stu-id="c4153-194">String</span></span>|<span data-ttu-id="c4153-195">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="c4153-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="c4153-196">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-197">networkName</span><span class="sxs-lookup"><span data-stu-id="c4153-197">networkName</span></span>|<span data-ttu-id="c4153-198">String</span><span class="sxs-lookup"><span data-stu-id="c4153-198">String</span></span>|<span data-ttu-id="c4153-199">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="c4153-199">Specify the network configuration name.</span></span> <span data-ttu-id="c4153-200">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-201">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="c4153-201">connectAutomatically</span></span>|<span data-ttu-id="c4153-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-202">Boolean</span></span>|<span data-ttu-id="c4153-203">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="c4153-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="c4153-204">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-205">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="c4153-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="c4153-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-206">Boolean</span></span>|<span data-ttu-id="c4153-207">指定 wifi 连接是否应连接到更多的首选网络 (如果已连接到此连接的话)。</span><span class="sxs-lookup"><span data-stu-id="c4153-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="c4153-208">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="c4153-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="c4153-209">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-210">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c4153-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c4153-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-211">Boolean</span></span>|<span data-ttu-id="c4153-212">指定是否应自动连接 wifi 连接, 即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="c4153-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="c4153-213">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-214">proxySetting</span><span class="sxs-lookup"><span data-stu-id="c4153-214">proxySetting</span></span>|[<span data-ttu-id="c4153-215">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="c4153-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c4153-216">指定从[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)继承的 wi-fi 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="c4153-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c4153-217">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="c4153-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c4153-218">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="c4153-218">proxyManualAddress</span></span>|<span data-ttu-id="c4153-219">String</span><span class="sxs-lookup"><span data-stu-id="c4153-219">String</span></span>|<span data-ttu-id="c4153-220">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c4153-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="c4153-221">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-222">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="c4153-222">proxyManualPort</span></span>|<span data-ttu-id="c4153-223">Int32</span><span class="sxs-lookup"><span data-stu-id="c4153-223">Int32</span></span>|<span data-ttu-id="c4153-224">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="c4153-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="c4153-225">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-226">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="c4153-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c4153-227">String</span><span class="sxs-lookup"><span data-stu-id="c4153-227">String</span></span>|<span data-ttu-id="c4153-228">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="c4153-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="c4153-229">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-230">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="c4153-230">forceFIPSCompliance</span></span>|<span data-ttu-id="c4153-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-231">Boolean</span></span>|<span data-ttu-id="c4153-232">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="c4153-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="c4153-233">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4153-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c4153-234">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="c4153-234">networkSingleSignOn</span></span>|[<span data-ttu-id="c4153-235">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="c4153-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="c4153-236">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="c4153-236">Specify the network single sign on type.</span></span> <span data-ttu-id="c4153-237">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="c4153-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="c4153-238">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="c4153-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="c4153-239">Int32</span><span class="sxs-lookup"><span data-stu-id="c4153-239">Int32</span></span>|<span data-ttu-id="c4153-240">指定最大身份验证超时 (以秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="c4153-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="c4153-241">有效范围: 1-120</span><span class="sxs-lookup"><span data-stu-id="c4153-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="c4153-242">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="c4153-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="c4153-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-243">Boolean</span></span>|<span data-ttu-id="c4153-244">指定 wifi 连接是否应提示额外的身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="c4153-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="c4153-245">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="c4153-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="c4153-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-246">Boolean</span></span>|<span data-ttu-id="c4153-247">指定 wifi 连接是否应启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="c4153-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="c4153-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c4153-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="c4153-249">Int32</span><span class="sxs-lookup"><span data-stu-id="c4153-249">Int32</span></span>|<span data-ttu-id="c4153-250">指定最大成对主密钥缓存时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="c4153-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="c4153-251">有效范围: 5-1440</span><span class="sxs-lookup"><span data-stu-id="c4153-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="c4153-252">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="c4153-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="c4153-253">Int32</span><span class="sxs-lookup"><span data-stu-id="c4153-253">Int32</span></span>|<span data-ttu-id="c4153-254">指定缓存中成对主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="c4153-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="c4153-255">有效范围: 1-255</span><span class="sxs-lookup"><span data-stu-id="c4153-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="c4153-256">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="c4153-256">enablePreAuthentication</span></span>|<span data-ttu-id="c4153-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4153-257">Boolean</span></span>|<span data-ttu-id="c4153-258">指定是否应启用预先身份验证。</span><span class="sxs-lookup"><span data-stu-id="c4153-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="c4153-259">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="c4153-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="c4153-260">Int32</span><span class="sxs-lookup"><span data-stu-id="c4153-260">Int32</span></span>|<span data-ttu-id="c4153-261">指定最大预先身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="c4153-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="c4153-262">有效范围: 1-16</span><span class="sxs-lookup"><span data-stu-id="c4153-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="c4153-263">eapType</span><span class="sxs-lookup"><span data-stu-id="c4153-263">eapType</span></span>|[<span data-ttu-id="c4153-264">eapType</span><span class="sxs-lookup"><span data-stu-id="c4153-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="c4153-265">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="c4153-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="c4153-266">指示 Wi-fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="c4153-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c4153-267">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="c4153-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="c4153-268">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="c4153-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="c4153-269">String collection</span><span class="sxs-lookup"><span data-stu-id="c4153-269">String collection</span></span>|<span data-ttu-id="c4153-270">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="c4153-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="c4153-271">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c4153-271">authenticationMethod</span></span>|[<span data-ttu-id="c4153-272">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c4153-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c4153-273">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c4153-273">Specify the authentication method.</span></span> <span data-ttu-id="c4153-274">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="c4153-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c4153-275">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="c4153-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="c4153-276">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="c4153-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c4153-277">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="c4153-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="c4153-278">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="c4153-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c4153-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c4153-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c4153-280">String</span><span class="sxs-lookup"><span data-stu-id="c4153-280">String</span></span>|<span data-ttu-id="c4153-281">指定在使用 EAP TTLS 或 PEAP 时用于替换隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="c4153-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="c4153-282">响应</span><span class="sxs-lookup"><span data-stu-id="c4153-282">Response</span></span>
<span data-ttu-id="c4153-283">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c4153-283">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4153-284">示例</span><span class="sxs-lookup"><span data-stu-id="c4153-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4153-285">请求</span><span class="sxs-lookup"><span data-stu-id="c4153-285">Request</span></span>
<span data-ttu-id="c4153-286">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4153-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2277

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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

### <a name="response"></a><span data-ttu-id="c4153-287">响应</span><span class="sxs-lookup"><span data-stu-id="c4153-287">Response</span></span>
<span data-ttu-id="c4153-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4153-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2449

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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





