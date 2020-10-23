---
title: 创建 windowsWifiEnterpriseEAPConfiguration
description: 创建新的 windowsWifiEnterpriseEAPConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7081a741aac0a4175167a8fe940732fea6e396d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732302"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="c2820-103">创建 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2820-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="c2820-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2820-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2820-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2820-107">创建新的 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2820-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2820-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2820-108">Prerequisites</span></span>
<span data-ttu-id="c2820-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2820-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2820-111">Permission type</span></span>|<span data-ttu-id="c2820-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c2820-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2820-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2820-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2820-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2820-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2820-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2820-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2820-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2820-116">Not supported.</span></span>|
|<span data-ttu-id="c2820-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2820-117">Application</span></span>|<span data-ttu-id="c2820-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2820-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2820-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2820-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2820-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2820-120">Request headers</span></span>
|<span data-ttu-id="c2820-121">标头</span><span class="sxs-lookup"><span data-stu-id="c2820-121">Header</span></span>|<span data-ttu-id="c2820-122">值</span><span class="sxs-lookup"><span data-stu-id="c2820-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2820-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2820-123">Authorization</span></span>|<span data-ttu-id="c2820-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2820-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2820-125">接受</span><span class="sxs-lookup"><span data-stu-id="c2820-125">Accept</span></span>|<span data-ttu-id="c2820-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2820-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2820-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2820-127">Request body</span></span>
<span data-ttu-id="c2820-128">在请求正文中，提供 windowsWifiEnterpriseEAPConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2820-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="c2820-129">下表显示创建 windowsWifiEnterpriseEAPConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c2820-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="c2820-130">属性</span><span class="sxs-lookup"><span data-stu-id="c2820-130">Property</span></span>|<span data-ttu-id="c2820-131">类型</span><span class="sxs-lookup"><span data-stu-id="c2820-131">Type</span></span>|<span data-ttu-id="c2820-132">说明</span><span class="sxs-lookup"><span data-stu-id="c2820-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2820-133">id</span><span class="sxs-lookup"><span data-stu-id="c2820-133">id</span></span>|<span data-ttu-id="c2820-134">String</span><span class="sxs-lookup"><span data-stu-id="c2820-134">String</span></span>|<span data-ttu-id="c2820-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c2820-135">Key of the entity.</span></span> <span data-ttu-id="c2820-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2820-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c2820-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2820-138">DateTimeOffset</span></span>|<span data-ttu-id="c2820-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c2820-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c2820-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2820-141">roleScopeTagIds</span></span>|<span data-ttu-id="c2820-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c2820-142">String collection</span></span>|<span data-ttu-id="c2820-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c2820-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2820-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2820-145">supportsScopeTags</span></span>|<span data-ttu-id="c2820-146">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-146">Boolean</span></span>|<span data-ttu-id="c2820-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c2820-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2820-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c2820-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2820-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c2820-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2820-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c2820-150">This property is read-only.</span></span> <span data-ttu-id="c2820-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c2820-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c2820-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c2820-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c2820-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c2820-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c2820-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c2820-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c2820-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c2820-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c2820-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c2820-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c2820-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c2820-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c2820-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c2820-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c2820-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c2820-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c2820-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2820-164">createdDateTime</span></span>|<span data-ttu-id="c2820-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2820-165">DateTimeOffset</span></span>|<span data-ttu-id="c2820-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c2820-166">DateTime the object was created.</span></span> <span data-ttu-id="c2820-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-168">说明</span><span class="sxs-lookup"><span data-stu-id="c2820-168">description</span></span>|<span data-ttu-id="c2820-169">String</span><span class="sxs-lookup"><span data-stu-id="c2820-169">String</span></span>|<span data-ttu-id="c2820-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c2820-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2820-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c2820-172">displayName</span></span>|<span data-ttu-id="c2820-173">String</span><span class="sxs-lookup"><span data-stu-id="c2820-173">String</span></span>|<span data-ttu-id="c2820-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c2820-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2820-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-176">version</span><span class="sxs-lookup"><span data-stu-id="c2820-176">version</span></span>|<span data-ttu-id="c2820-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c2820-177">Int32</span></span>|<span data-ttu-id="c2820-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c2820-178">Version of the device configuration.</span></span> <span data-ttu-id="c2820-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2820-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="c2820-180">preSharedKey</span></span>|<span data-ttu-id="c2820-181">String</span><span class="sxs-lookup"><span data-stu-id="c2820-181">String</span></span>|<span data-ttu-id="c2820-182">这是 WPA 个人 Wi-Fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="c2820-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="c2820-183">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c2820-184">wifiSecurityType</span></span>|[<span data-ttu-id="c2820-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c2820-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c2820-186">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="c2820-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="c2820-187">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2820-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c2820-188">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="c2820-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c2820-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="c2820-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="c2820-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="c2820-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="c2820-191">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="c2820-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="c2820-192">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2820-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c2820-193">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="c2820-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="c2820-194">ssid</span><span class="sxs-lookup"><span data-stu-id="c2820-194">ssid</span></span>|<span data-ttu-id="c2820-195">String</span><span class="sxs-lookup"><span data-stu-id="c2820-195">String</span></span>|<span data-ttu-id="c2820-196">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="c2820-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="c2820-197">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-198">networkName</span><span class="sxs-lookup"><span data-stu-id="c2820-198">networkName</span></span>|<span data-ttu-id="c2820-199">String</span><span class="sxs-lookup"><span data-stu-id="c2820-199">String</span></span>|<span data-ttu-id="c2820-200">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="c2820-200">Specify the network configuration name.</span></span> <span data-ttu-id="c2820-201">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="c2820-202">connectAutomatically</span></span>|<span data-ttu-id="c2820-203">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-203">Boolean</span></span>|<span data-ttu-id="c2820-204">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="c2820-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="c2820-205">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="c2820-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="c2820-207">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-207">Boolean</span></span>|<span data-ttu-id="c2820-208">指定 wifi 连接是否应连接到更多的首选网络（如果已连接到此连接的话）。</span><span class="sxs-lookup"><span data-stu-id="c2820-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="c2820-209">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="c2820-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="c2820-210">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c2820-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c2820-212">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-212">Boolean</span></span>|<span data-ttu-id="c2820-213">指定是否应自动连接 wifi 连接，即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="c2820-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="c2820-214">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="c2820-215">proxySetting</span></span>|[<span data-ttu-id="c2820-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="c2820-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c2820-217">指定从 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)继承的 Wi-Fi 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="c2820-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c2820-218">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="c2820-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c2820-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="c2820-219">proxyManualAddress</span></span>|<span data-ttu-id="c2820-220">String</span><span class="sxs-lookup"><span data-stu-id="c2820-220">String</span></span>|<span data-ttu-id="c2820-221">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c2820-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="c2820-222">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="c2820-223">proxyManualPort</span></span>|<span data-ttu-id="c2820-224">Int32</span><span class="sxs-lookup"><span data-stu-id="c2820-224">Int32</span></span>|<span data-ttu-id="c2820-225">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="c2820-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="c2820-226">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="c2820-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c2820-228">String</span><span class="sxs-lookup"><span data-stu-id="c2820-228">String</span></span>|<span data-ttu-id="c2820-229">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="c2820-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="c2820-230">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="c2820-231">forceFIPSCompliance</span></span>|<span data-ttu-id="c2820-232">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-232">Boolean</span></span>|<span data-ttu-id="c2820-233">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="c2820-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="c2820-234">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2820-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c2820-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="c2820-235">networkSingleSignOn</span></span>|[<span data-ttu-id="c2820-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="c2820-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="c2820-237">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="c2820-237">Specify the network single sign on type.</span></span> <span data-ttu-id="c2820-238">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="c2820-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="c2820-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="c2820-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="c2820-240">Int32</span><span class="sxs-lookup"><span data-stu-id="c2820-240">Int32</span></span>|<span data-ttu-id="c2820-241">以秒为单位指定最大身份验证超时 () 。</span><span class="sxs-lookup"><span data-stu-id="c2820-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="c2820-242">有效范围：1-120</span><span class="sxs-lookup"><span data-stu-id="c2820-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="c2820-243">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="c2820-243">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="c2820-244">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-244">Boolean</span></span>|<span data-ttu-id="c2820-245">指定 wifi 连接是否应提示额外的身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="c2820-245">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="c2820-246">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="c2820-246">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="c2820-247">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-247">Boolean</span></span>|<span data-ttu-id="c2820-248">指定 wifi 连接是否应启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="c2820-248">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="c2820-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c2820-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="c2820-250">Int32</span><span class="sxs-lookup"><span data-stu-id="c2820-250">Int32</span></span>|<span data-ttu-id="c2820-251">指定最大成对主密钥缓存时间 (以分钟) 为单位）。</span><span class="sxs-lookup"><span data-stu-id="c2820-251">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="c2820-252">有效范围：5-1440</span><span class="sxs-lookup"><span data-stu-id="c2820-252">Valid range: 5-1440</span></span>|
|<span data-ttu-id="c2820-253">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="c2820-253">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="c2820-254">Int32</span><span class="sxs-lookup"><span data-stu-id="c2820-254">Int32</span></span>|<span data-ttu-id="c2820-255">指定缓存中成对主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="c2820-255">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="c2820-256">有效范围：1-255</span><span class="sxs-lookup"><span data-stu-id="c2820-256">Valid range: 1-255</span></span>|
|<span data-ttu-id="c2820-257">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="c2820-257">enablePreAuthentication</span></span>|<span data-ttu-id="c2820-258">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-258">Boolean</span></span>|<span data-ttu-id="c2820-259">指定是否应启用预先身份验证。</span><span class="sxs-lookup"><span data-stu-id="c2820-259">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="c2820-260">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="c2820-260">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="c2820-261">Int32</span><span class="sxs-lookup"><span data-stu-id="c2820-261">Int32</span></span>|<span data-ttu-id="c2820-262">指定最大预先身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="c2820-262">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="c2820-263">有效范围：1-16</span><span class="sxs-lookup"><span data-stu-id="c2820-263">Valid range: 1-16</span></span>|
|<span data-ttu-id="c2820-264">eapType</span><span class="sxs-lookup"><span data-stu-id="c2820-264">eapType</span></span>|[<span data-ttu-id="c2820-265">eapType</span><span class="sxs-lookup"><span data-stu-id="c2820-265">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="c2820-266">可扩展的身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="c2820-266">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="c2820-267">指示 Wi-Fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="c2820-267">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c2820-268">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="c2820-268">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="c2820-269">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="c2820-269">trustedServerCertificateNames</span></span>|<span data-ttu-id="c2820-270">String collection</span><span class="sxs-lookup"><span data-stu-id="c2820-270">String collection</span></span>|<span data-ttu-id="c2820-271">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="c2820-271">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="c2820-272">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2820-272">authenticationMethod</span></span>|[<span data-ttu-id="c2820-273">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2820-273">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c2820-274">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c2820-274">Specify the authentication method.</span></span> <span data-ttu-id="c2820-275">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="c2820-275">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c2820-276">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="c2820-276">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="c2820-277">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="c2820-277">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c2820-278">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="c2820-278">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="c2820-279">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="c2820-279">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c2820-280">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c2820-280">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c2820-281">String</span><span class="sxs-lookup"><span data-stu-id="c2820-281">String</span></span>|<span data-ttu-id="c2820-282">指定在使用 EAP TTLS 或 PEAP 时用于替换隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="c2820-282">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="c2820-283">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="c2820-283">requireCryptographicBinding</span></span>|<span data-ttu-id="c2820-284">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-284">Boolean</span></span>|<span data-ttu-id="c2820-285">指定在选择 EAP 类型作为 PEAP 时是否启用加密绑定。</span><span class="sxs-lookup"><span data-stu-id="c2820-285">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="c2820-286">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="c2820-286">performServerValidation</span></span>|<span data-ttu-id="c2820-287">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-287">Boolean</span></span>|<span data-ttu-id="c2820-288">通过在选择 EAP 类型作为 PEAP 时验证证书来指定是否启用对服务器标识的验证。</span><span class="sxs-lookup"><span data-stu-id="c2820-288">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="c2820-289">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="c2820-289">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="c2820-290">布尔</span><span class="sxs-lookup"><span data-stu-id="c2820-290">Boolean</span></span>|<span data-ttu-id="c2820-291">当选择 EAP 类型作为 PEAP 时，指定是否阻止提示用户为受信任的证书颁发机构授权新服务器。</span><span class="sxs-lookup"><span data-stu-id="c2820-291">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="c2820-292">响应</span><span class="sxs-lookup"><span data-stu-id="c2820-292">Response</span></span>
<span data-ttu-id="c2820-293">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2820-293">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2820-294">示例</span><span class="sxs-lookup"><span data-stu-id="c2820-294">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2820-295">请求</span><span class="sxs-lookup"><span data-stu-id="c2820-295">Request</span></span>
<span data-ttu-id="c2820-296">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2820-296">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2402

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true
}
```

### <a name="response"></a><span data-ttu-id="c2820-297">响应</span><span class="sxs-lookup"><span data-stu-id="c2820-297">Response</span></span>
<span data-ttu-id="c2820-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2820-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2574

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true
}
```





