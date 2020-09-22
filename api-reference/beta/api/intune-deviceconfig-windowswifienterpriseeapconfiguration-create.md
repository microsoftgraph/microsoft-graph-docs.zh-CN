---
title: 创建 windowsWifiEnterpriseEAPConfiguration
description: 创建新的 windowsWifiEnterpriseEAPConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b47e1ba1fffaf7e194c5ac287903f28d13bfdb57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990044"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="73b60-103">创建 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="73b60-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="73b60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73b60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73b60-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73b60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73b60-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73b60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73b60-107">创建新的 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73b60-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73b60-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="73b60-108">Prerequisites</span></span>
<span data-ttu-id="73b60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73b60-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="73b60-111">Permission type</span></span>|<span data-ttu-id="73b60-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73b60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73b60-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73b60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73b60-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b60-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73b60-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73b60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73b60-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73b60-116">Not supported.</span></span>|
|<span data-ttu-id="73b60-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="73b60-117">Application</span></span>|<span data-ttu-id="73b60-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b60-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73b60-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73b60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73b60-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73b60-120">Request headers</span></span>
|<span data-ttu-id="73b60-121">标头</span><span class="sxs-lookup"><span data-stu-id="73b60-121">Header</span></span>|<span data-ttu-id="73b60-122">值</span><span class="sxs-lookup"><span data-stu-id="73b60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73b60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73b60-123">Authorization</span></span>|<span data-ttu-id="73b60-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73b60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73b60-125">接受</span><span class="sxs-lookup"><span data-stu-id="73b60-125">Accept</span></span>|<span data-ttu-id="73b60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73b60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73b60-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73b60-127">Request body</span></span>
<span data-ttu-id="73b60-128">在请求正文中，提供 windowsWifiEnterpriseEAPConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73b60-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="73b60-129">下表显示创建 windowsWifiEnterpriseEAPConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73b60-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="73b60-130">属性</span><span class="sxs-lookup"><span data-stu-id="73b60-130">Property</span></span>|<span data-ttu-id="73b60-131">类型</span><span class="sxs-lookup"><span data-stu-id="73b60-131">Type</span></span>|<span data-ttu-id="73b60-132">说明</span><span class="sxs-lookup"><span data-stu-id="73b60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b60-133">id</span><span class="sxs-lookup"><span data-stu-id="73b60-133">id</span></span>|<span data-ttu-id="73b60-134">String</span><span class="sxs-lookup"><span data-stu-id="73b60-134">String</span></span>|<span data-ttu-id="73b60-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73b60-135">Key of the entity.</span></span> <span data-ttu-id="73b60-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73b60-137">lastModifiedDateTime</span></span>|<span data-ttu-id="73b60-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73b60-138">DateTimeOffset</span></span>|<span data-ttu-id="73b60-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73b60-139">DateTime the object was last modified.</span></span> <span data-ttu-id="73b60-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73b60-141">roleScopeTagIds</span></span>|<span data-ttu-id="73b60-142">String collection</span><span class="sxs-lookup"><span data-stu-id="73b60-142">String collection</span></span>|<span data-ttu-id="73b60-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="73b60-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73b60-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73b60-145">supportsScopeTags</span></span>|<span data-ttu-id="73b60-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-146">Boolean</span></span>|<span data-ttu-id="73b60-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="73b60-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73b60-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="73b60-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73b60-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="73b60-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73b60-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="73b60-150">This property is read-only.</span></span> <span data-ttu-id="73b60-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73b60-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="73b60-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73b60-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="73b60-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="73b60-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="73b60-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73b60-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="73b60-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73b60-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="73b60-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="73b60-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="73b60-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73b60-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="73b60-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73b60-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="73b60-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="73b60-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="73b60-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73b60-164">createdDateTime</span></span>|<span data-ttu-id="73b60-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73b60-165">DateTimeOffset</span></span>|<span data-ttu-id="73b60-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73b60-166">DateTime the object was created.</span></span> <span data-ttu-id="73b60-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-168">description</span><span class="sxs-lookup"><span data-stu-id="73b60-168">description</span></span>|<span data-ttu-id="73b60-169">String</span><span class="sxs-lookup"><span data-stu-id="73b60-169">String</span></span>|<span data-ttu-id="73b60-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="73b60-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73b60-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-172">displayName</span><span class="sxs-lookup"><span data-stu-id="73b60-172">displayName</span></span>|<span data-ttu-id="73b60-173">String</span><span class="sxs-lookup"><span data-stu-id="73b60-173">String</span></span>|<span data-ttu-id="73b60-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="73b60-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73b60-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-176">version</span><span class="sxs-lookup"><span data-stu-id="73b60-176">version</span></span>|<span data-ttu-id="73b60-177">Int32</span><span class="sxs-lookup"><span data-stu-id="73b60-177">Int32</span></span>|<span data-ttu-id="73b60-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="73b60-178">Version of the device configuration.</span></span> <span data-ttu-id="73b60-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73b60-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="73b60-180">preSharedKey</span></span>|<span data-ttu-id="73b60-181">String</span><span class="sxs-lookup"><span data-stu-id="73b60-181">String</span></span>|<span data-ttu-id="73b60-182">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="73b60-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="73b60-183">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="73b60-184">wifiSecurityType</span></span>|[<span data-ttu-id="73b60-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="73b60-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="73b60-186">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="73b60-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="73b60-187">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="73b60-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="73b60-188">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="73b60-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="73b60-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="73b60-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="73b60-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="73b60-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="73b60-191">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="73b60-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="73b60-192">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="73b60-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="73b60-193">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="73b60-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="73b60-194">ssid</span><span class="sxs-lookup"><span data-stu-id="73b60-194">ssid</span></span>|<span data-ttu-id="73b60-195">String</span><span class="sxs-lookup"><span data-stu-id="73b60-195">String</span></span>|<span data-ttu-id="73b60-196">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="73b60-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="73b60-197">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-198">networkName</span><span class="sxs-lookup"><span data-stu-id="73b60-198">networkName</span></span>|<span data-ttu-id="73b60-199">String</span><span class="sxs-lookup"><span data-stu-id="73b60-199">String</span></span>|<span data-ttu-id="73b60-200">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="73b60-200">Specify the network configuration name.</span></span> <span data-ttu-id="73b60-201">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="73b60-202">connectAutomatically</span></span>|<span data-ttu-id="73b60-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-203">Boolean</span></span>|<span data-ttu-id="73b60-204">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="73b60-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="73b60-205">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="73b60-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="73b60-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-207">Boolean</span></span>|<span data-ttu-id="73b60-208">指定 wifi 连接是否应连接到更多的首选网络（如果已连接到此连接的话）。</span><span class="sxs-lookup"><span data-stu-id="73b60-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="73b60-209">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="73b60-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="73b60-210">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="73b60-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="73b60-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-212">Boolean</span></span>|<span data-ttu-id="73b60-213">指定是否应自动连接 wifi 连接，即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="73b60-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="73b60-214">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="73b60-215">proxySetting</span></span>|[<span data-ttu-id="73b60-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="73b60-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="73b60-217">指定从 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)继承的 wi-fi 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="73b60-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="73b60-218">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="73b60-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="73b60-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="73b60-219">proxyManualAddress</span></span>|<span data-ttu-id="73b60-220">String</span><span class="sxs-lookup"><span data-stu-id="73b60-220">String</span></span>|<span data-ttu-id="73b60-221">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="73b60-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="73b60-222">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="73b60-223">proxyManualPort</span></span>|<span data-ttu-id="73b60-224">Int32</span><span class="sxs-lookup"><span data-stu-id="73b60-224">Int32</span></span>|<span data-ttu-id="73b60-225">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="73b60-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="73b60-226">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="73b60-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="73b60-228">String</span><span class="sxs-lookup"><span data-stu-id="73b60-228">String</span></span>|<span data-ttu-id="73b60-229">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="73b60-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="73b60-230">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="73b60-231">forceFIPSCompliance</span></span>|<span data-ttu-id="73b60-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-232">Boolean</span></span>|<span data-ttu-id="73b60-233">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="73b60-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="73b60-234">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73b60-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="73b60-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="73b60-235">networkSingleSignOn</span></span>|[<span data-ttu-id="73b60-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="73b60-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="73b60-237">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="73b60-237">Specify the network single sign on type.</span></span> <span data-ttu-id="73b60-238">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="73b60-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="73b60-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="73b60-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="73b60-240">Int32</span><span class="sxs-lookup"><span data-stu-id="73b60-240">Int32</span></span>|<span data-ttu-id="73b60-241">以秒为单位指定最大身份验证超时 () 。</span><span class="sxs-lookup"><span data-stu-id="73b60-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="73b60-242">有效范围：1-120</span><span class="sxs-lookup"><span data-stu-id="73b60-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="73b60-243">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="73b60-243">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="73b60-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-244">Boolean</span></span>|<span data-ttu-id="73b60-245">指定 wifi 连接是否应提示额外的身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="73b60-245">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="73b60-246">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="73b60-246">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="73b60-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-247">Boolean</span></span>|<span data-ttu-id="73b60-248">指定 wifi 连接是否应启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="73b60-248">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="73b60-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="73b60-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="73b60-250">Int32</span><span class="sxs-lookup"><span data-stu-id="73b60-250">Int32</span></span>|<span data-ttu-id="73b60-251">指定最大成对主密钥缓存时间 (以分钟) 为单位）。</span><span class="sxs-lookup"><span data-stu-id="73b60-251">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="73b60-252">有效范围：5-1440</span><span class="sxs-lookup"><span data-stu-id="73b60-252">Valid range: 5-1440</span></span>|
|<span data-ttu-id="73b60-253">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="73b60-253">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="73b60-254">Int32</span><span class="sxs-lookup"><span data-stu-id="73b60-254">Int32</span></span>|<span data-ttu-id="73b60-255">指定缓存中成对主密钥的最大数量。</span><span class="sxs-lookup"><span data-stu-id="73b60-255">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="73b60-256">有效范围：1-255</span><span class="sxs-lookup"><span data-stu-id="73b60-256">Valid range: 1-255</span></span>|
|<span data-ttu-id="73b60-257">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="73b60-257">enablePreAuthentication</span></span>|<span data-ttu-id="73b60-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-258">Boolean</span></span>|<span data-ttu-id="73b60-259">指定是否应启用预先身份验证。</span><span class="sxs-lookup"><span data-stu-id="73b60-259">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="73b60-260">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="73b60-260">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="73b60-261">Int32</span><span class="sxs-lookup"><span data-stu-id="73b60-261">Int32</span></span>|<span data-ttu-id="73b60-262">指定最大预先身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="73b60-262">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="73b60-263">有效范围：1-16</span><span class="sxs-lookup"><span data-stu-id="73b60-263">Valid range: 1-16</span></span>|
|<span data-ttu-id="73b60-264">eapType</span><span class="sxs-lookup"><span data-stu-id="73b60-264">eapType</span></span>|[<span data-ttu-id="73b60-265">eapType</span><span class="sxs-lookup"><span data-stu-id="73b60-265">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="73b60-266">可扩展的身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="73b60-266">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="73b60-267">指示 Wi-fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="73b60-267">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="73b60-268">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="73b60-268">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="73b60-269">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="73b60-269">trustedServerCertificateNames</span></span>|<span data-ttu-id="73b60-270">String collection</span><span class="sxs-lookup"><span data-stu-id="73b60-270">String collection</span></span>|<span data-ttu-id="73b60-271">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="73b60-271">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="73b60-272">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73b60-272">authenticationMethod</span></span>|[<span data-ttu-id="73b60-273">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73b60-273">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="73b60-274">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="73b60-274">Specify the authentication method.</span></span> <span data-ttu-id="73b60-275">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="73b60-275">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="73b60-276">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="73b60-276">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="73b60-277">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="73b60-277">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="73b60-278">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="73b60-278">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="73b60-279">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="73b60-279">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="73b60-280">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="73b60-280">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="73b60-281">String</span><span class="sxs-lookup"><span data-stu-id="73b60-281">String</span></span>|<span data-ttu-id="73b60-282">指定在使用 EAP TTLS 或 PEAP 时用于替换隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="73b60-282">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="73b60-283">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="73b60-283">requireCryptographicBinding</span></span>|<span data-ttu-id="73b60-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-284">Boolean</span></span>|<span data-ttu-id="73b60-285">指定在选择 EAP 类型作为 PEAP 时是否启用加密绑定。</span><span class="sxs-lookup"><span data-stu-id="73b60-285">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="73b60-286">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="73b60-286">performServerValidation</span></span>|<span data-ttu-id="73b60-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-287">Boolean</span></span>|<span data-ttu-id="73b60-288">通过在选择 EAP 类型作为 PEAP 时验证证书来指定是否启用对服务器标识的验证。</span><span class="sxs-lookup"><span data-stu-id="73b60-288">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="73b60-289">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="73b60-289">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="73b60-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="73b60-290">Boolean</span></span>|<span data-ttu-id="73b60-291">当选择 EAP 类型作为 PEAP 时，指定是否阻止提示用户为受信任的证书颁发机构授权新服务器。</span><span class="sxs-lookup"><span data-stu-id="73b60-291">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="73b60-292">响应</span><span class="sxs-lookup"><span data-stu-id="73b60-292">Response</span></span>
<span data-ttu-id="73b60-293">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73b60-293">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b60-294">示例</span><span class="sxs-lookup"><span data-stu-id="73b60-294">Example</span></span>

### <a name="request"></a><span data-ttu-id="73b60-295">请求</span><span class="sxs-lookup"><span data-stu-id="73b60-295">Request</span></span>
<span data-ttu-id="73b60-296">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73b60-296">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73b60-297">响应</span><span class="sxs-lookup"><span data-stu-id="73b60-297">Response</span></span>
<span data-ttu-id="73b60-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73b60-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






