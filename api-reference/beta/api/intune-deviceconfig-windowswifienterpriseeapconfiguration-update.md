---
title: 更新 windowsWifiEnterpriseEAPConfiguration
description: 更新 windowsWifiEnterpriseEAPConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb62512c28d87a2c0707dc6dd9b1f326c5ce53ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344047"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="00803-103">更新 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="00803-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="00803-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00803-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00803-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00803-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00803-106">更新[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00803-106">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00803-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="00803-107">Prerequisites</span></span>
<span data-ttu-id="00803-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00803-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="00803-110">Permission type</span></span>|<span data-ttu-id="00803-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="00803-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00803-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00803-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00803-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00803-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00803-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00803-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00803-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00803-115">Not supported.</span></span>|
|<span data-ttu-id="00803-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="00803-116">Application</span></span>|<span data-ttu-id="00803-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00803-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00803-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00803-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="00803-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="00803-119">Request headers</span></span>
|<span data-ttu-id="00803-120">标头</span><span class="sxs-lookup"><span data-stu-id="00803-120">Header</span></span>|<span data-ttu-id="00803-121">值</span><span class="sxs-lookup"><span data-stu-id="00803-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00803-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00803-122">Authorization</span></span>|<span data-ttu-id="00803-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00803-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00803-124">接受</span><span class="sxs-lookup"><span data-stu-id="00803-124">Accept</span></span>|<span data-ttu-id="00803-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00803-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00803-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="00803-126">Request body</span></span>
<span data-ttu-id="00803-127">在请求正文中, 提供[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00803-127">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="00803-128">下表显示创建[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="00803-128">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="00803-129">属性</span><span class="sxs-lookup"><span data-stu-id="00803-129">Property</span></span>|<span data-ttu-id="00803-130">类型</span><span class="sxs-lookup"><span data-stu-id="00803-130">Type</span></span>|<span data-ttu-id="00803-131">说明</span><span class="sxs-lookup"><span data-stu-id="00803-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00803-132">id</span><span class="sxs-lookup"><span data-stu-id="00803-132">id</span></span>|<span data-ttu-id="00803-133">字符串</span><span class="sxs-lookup"><span data-stu-id="00803-133">String</span></span>|<span data-ttu-id="00803-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="00803-134">Key of the entity.</span></span> <span data-ttu-id="00803-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00803-136">lastModifiedDateTime</span></span>|<span data-ttu-id="00803-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00803-137">DateTimeOffset</span></span>|<span data-ttu-id="00803-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="00803-138">DateTime the object was last modified.</span></span> <span data-ttu-id="00803-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00803-140">roleScopeTagIds</span></span>|<span data-ttu-id="00803-141">String collection</span><span class="sxs-lookup"><span data-stu-id="00803-141">String collection</span></span>|<span data-ttu-id="00803-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="00803-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00803-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="00803-144">supportsScopeTags</span></span>|<span data-ttu-id="00803-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-145">Boolean</span></span>|<span data-ttu-id="00803-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="00803-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00803-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="00803-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00803-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="00803-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00803-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00803-149">This property is read-only.</span></span> <span data-ttu-id="00803-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="00803-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="00803-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="00803-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="00803-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="00803-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="00803-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="00803-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="00803-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="00803-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="00803-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="00803-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="00803-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="00803-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="00803-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="00803-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="00803-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="00803-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="00803-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00803-163">createdDateTime</span></span>|<span data-ttu-id="00803-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00803-164">DateTimeOffset</span></span>|<span data-ttu-id="00803-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="00803-165">DateTime the object was created.</span></span> <span data-ttu-id="00803-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-167">说明</span><span class="sxs-lookup"><span data-stu-id="00803-167">description</span></span>|<span data-ttu-id="00803-168">String</span><span class="sxs-lookup"><span data-stu-id="00803-168">String</span></span>|<span data-ttu-id="00803-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="00803-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00803-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-171">displayName</span><span class="sxs-lookup"><span data-stu-id="00803-171">displayName</span></span>|<span data-ttu-id="00803-172">String</span><span class="sxs-lookup"><span data-stu-id="00803-172">String</span></span>|<span data-ttu-id="00803-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="00803-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00803-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-175">version</span><span class="sxs-lookup"><span data-stu-id="00803-175">version</span></span>|<span data-ttu-id="00803-176">Int32</span><span class="sxs-lookup"><span data-stu-id="00803-176">Int32</span></span>|<span data-ttu-id="00803-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="00803-177">Version of the device configuration.</span></span> <span data-ttu-id="00803-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00803-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="00803-179">preSharedKey</span></span>|<span data-ttu-id="00803-180">String</span><span class="sxs-lookup"><span data-stu-id="00803-180">String</span></span>|<span data-ttu-id="00803-181">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="00803-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="00803-182">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="00803-183">wifiSecurityType</span></span>|[<span data-ttu-id="00803-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="00803-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="00803-185">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="00803-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="00803-186">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="00803-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="00803-187">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="00803-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="00803-188">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="00803-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="00803-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="00803-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="00803-190">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="00803-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="00803-191">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="00803-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="00803-192">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="00803-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="00803-193">ssid</span><span class="sxs-lookup"><span data-stu-id="00803-193">ssid</span></span>|<span data-ttu-id="00803-194">String</span><span class="sxs-lookup"><span data-stu-id="00803-194">String</span></span>|<span data-ttu-id="00803-195">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="00803-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="00803-196">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-197">networkName</span><span class="sxs-lookup"><span data-stu-id="00803-197">networkName</span></span>|<span data-ttu-id="00803-198">String</span><span class="sxs-lookup"><span data-stu-id="00803-198">String</span></span>|<span data-ttu-id="00803-199">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="00803-199">Specify the network configuration name.</span></span> <span data-ttu-id="00803-200">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-201">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="00803-201">connectAutomatically</span></span>|<span data-ttu-id="00803-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-202">Boolean</span></span>|<span data-ttu-id="00803-203">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="00803-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="00803-204">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-205">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="00803-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="00803-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-206">Boolean</span></span>|<span data-ttu-id="00803-207">指定 wifi 连接是否应连接到更多的首选网络 (如果已连接到此连接的话)。</span><span class="sxs-lookup"><span data-stu-id="00803-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="00803-208">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="00803-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="00803-209">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-210">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="00803-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="00803-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-211">Boolean</span></span>|<span data-ttu-id="00803-212">指定是否应自动连接 wifi 连接, 即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="00803-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="00803-213">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-214">proxySetting</span><span class="sxs-lookup"><span data-stu-id="00803-214">proxySetting</span></span>|[<span data-ttu-id="00803-215">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="00803-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="00803-216">指定从[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)继承的 wi-fi 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="00803-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="00803-217">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="00803-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="00803-218">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="00803-218">proxyManualAddress</span></span>|<span data-ttu-id="00803-219">String</span><span class="sxs-lookup"><span data-stu-id="00803-219">String</span></span>|<span data-ttu-id="00803-220">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="00803-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="00803-221">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-222">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="00803-222">proxyManualPort</span></span>|<span data-ttu-id="00803-223">Int32</span><span class="sxs-lookup"><span data-stu-id="00803-223">Int32</span></span>|<span data-ttu-id="00803-224">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="00803-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="00803-225">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-226">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="00803-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="00803-227">String</span><span class="sxs-lookup"><span data-stu-id="00803-227">String</span></span>|<span data-ttu-id="00803-228">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="00803-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="00803-229">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-230">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="00803-230">forceFIPSCompliance</span></span>|<span data-ttu-id="00803-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-231">Boolean</span></span>|<span data-ttu-id="00803-232">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="00803-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="00803-233">继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00803-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="00803-234">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="00803-234">networkSingleSignOn</span></span>|[<span data-ttu-id="00803-235">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="00803-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="00803-236">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="00803-236">Specify the network single sign on type.</span></span> <span data-ttu-id="00803-237">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="00803-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="00803-238">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="00803-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="00803-239">Int32</span><span class="sxs-lookup"><span data-stu-id="00803-239">Int32</span></span>|<span data-ttu-id="00803-240">指定最大身份验证超时 (以秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="00803-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="00803-241">有效范围: 1-120</span><span class="sxs-lookup"><span data-stu-id="00803-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="00803-242">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="00803-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="00803-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-243">Boolean</span></span>|<span data-ttu-id="00803-244">指定 wifi 连接是否应提示额外的身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="00803-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="00803-245">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="00803-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="00803-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-246">Boolean</span></span>|<span data-ttu-id="00803-247">指定 wifi 连接是否应启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="00803-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="00803-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="00803-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="00803-249">Int32</span><span class="sxs-lookup"><span data-stu-id="00803-249">Int32</span></span>|<span data-ttu-id="00803-250">指定最大成对主密钥缓存时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="00803-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="00803-251">有效范围: 5-1440</span><span class="sxs-lookup"><span data-stu-id="00803-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="00803-252">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="00803-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="00803-253">Int32</span><span class="sxs-lookup"><span data-stu-id="00803-253">Int32</span></span>|<span data-ttu-id="00803-254">指定缓存中成对主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="00803-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="00803-255">有效范围: 1-255</span><span class="sxs-lookup"><span data-stu-id="00803-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="00803-256">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="00803-256">enablePreAuthentication</span></span>|<span data-ttu-id="00803-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="00803-257">Boolean</span></span>|<span data-ttu-id="00803-258">指定是否应启用预先身份验证。</span><span class="sxs-lookup"><span data-stu-id="00803-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="00803-259">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="00803-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="00803-260">Int32</span><span class="sxs-lookup"><span data-stu-id="00803-260">Int32</span></span>|<span data-ttu-id="00803-261">指定最大预先身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="00803-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="00803-262">有效范围: 1-16</span><span class="sxs-lookup"><span data-stu-id="00803-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="00803-263">eapType</span><span class="sxs-lookup"><span data-stu-id="00803-263">eapType</span></span>|[<span data-ttu-id="00803-264">eapType</span><span class="sxs-lookup"><span data-stu-id="00803-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="00803-265">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="00803-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="00803-266">指示 Wi-fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="00803-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="00803-267">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="00803-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="00803-268">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="00803-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="00803-269">String collection</span><span class="sxs-lookup"><span data-stu-id="00803-269">String collection</span></span>|<span data-ttu-id="00803-270">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="00803-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="00803-271">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="00803-271">authenticationMethod</span></span>|[<span data-ttu-id="00803-272">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="00803-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="00803-273">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="00803-273">Specify the authentication method.</span></span> <span data-ttu-id="00803-274">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="00803-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="00803-275">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="00803-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="00803-276">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="00803-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="00803-277">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="00803-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="00803-278">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="00803-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="00803-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="00803-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="00803-280">String</span><span class="sxs-lookup"><span data-stu-id="00803-280">String</span></span>|<span data-ttu-id="00803-281">指定在使用 EAP TTLS 或 PEAP 时用于替换隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="00803-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="00803-282">响应</span><span class="sxs-lookup"><span data-stu-id="00803-282">Response</span></span>
<span data-ttu-id="00803-283">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00803-283">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00803-284">示例</span><span class="sxs-lookup"><span data-stu-id="00803-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="00803-285">请求</span><span class="sxs-lookup"><span data-stu-id="00803-285">Request</span></span>
<span data-ttu-id="00803-286">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00803-286">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="00803-287">响应</span><span class="sxs-lookup"><span data-stu-id="00803-287">Response</span></span>
<span data-ttu-id="00803-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00803-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






