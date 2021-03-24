---
title: 更新 windowsWifiEnterpriseEAPConfiguration
description: 更新 windowsWifiEnterpriseEAPConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a6c89823f9b66a793302fd6d787ec369b4732fd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136900"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="bbbbd-103">更新 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="bbbbd-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="bbbbd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbbbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbbbd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbbbd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbbbd-107">更新 [windowsWifiEnterpriseEAPConfiguration 对象](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbbbd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbbbd-108">Prerequisites</span></span>
<span data-ttu-id="bbbbd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbbbd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbbbd-111">Permission type</span></span>|<span data-ttu-id="bbbbd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbbbd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbbbd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbbbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbbbd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbbd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbbbd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbbbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbbbd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-116">Not supported.</span></span>|
|<span data-ttu-id="bbbbd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbbbd-117">Application</span></span>|<span data-ttu-id="bbbbd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbbd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbbbd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbbbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bbbbd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbbbd-120">Request headers</span></span>
|<span data-ttu-id="bbbbd-121">标头</span><span class="sxs-lookup"><span data-stu-id="bbbbd-121">Header</span></span>|<span data-ttu-id="bbbbd-122">值</span><span class="sxs-lookup"><span data-stu-id="bbbbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbbbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbbbd-123">Authorization</span></span>|<span data-ttu-id="bbbbd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbbbd-125">接受</span><span class="sxs-lookup"><span data-stu-id="bbbbd-125">Accept</span></span>|<span data-ttu-id="bbbbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbbbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbbbd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbbbd-127">Request body</span></span>
<span data-ttu-id="bbbbd-128">在请求正文中，提供 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="bbbbd-129">下表显示创建 [windowsWifiEnterpriseEAPConfiguration 时所需的属性](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="bbbbd-130">属性</span><span class="sxs-lookup"><span data-stu-id="bbbbd-130">Property</span></span>|<span data-ttu-id="bbbbd-131">类型</span><span class="sxs-lookup"><span data-stu-id="bbbbd-131">Type</span></span>|<span data-ttu-id="bbbbd-132">说明</span><span class="sxs-lookup"><span data-stu-id="bbbbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbbbd-133">id</span><span class="sxs-lookup"><span data-stu-id="bbbbd-133">id</span></span>|<span data-ttu-id="bbbbd-134">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-134">String</span></span>|<span data-ttu-id="bbbbd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-135">Key of the entity.</span></span> <span data-ttu-id="bbbbd-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbbbd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bbbbd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbbbd-138">DateTimeOffset</span></span>|<span data-ttu-id="bbbbd-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bbbbd-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bbbbd-141">roleScopeTagIds</span></span>|<span data-ttu-id="bbbbd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bbbbd-142">String collection</span></span>|<span data-ttu-id="bbbbd-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bbbbd-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bbbbd-145">supportsScopeTags</span></span>|<span data-ttu-id="bbbbd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-146">Boolean</span></span>|<span data-ttu-id="bbbbd-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bbbbd-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bbbbd-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bbbbd-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-150">This property is read-only.</span></span> <span data-ttu-id="bbbbd-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bbbbd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bbbbd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bbbbd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bbbbd-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bbbbd-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bbbbd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bbbbd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bbbbd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bbbbd-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bbbbd-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bbbbd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bbbbd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bbbbd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bbbbd-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bbbbd-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbbbd-164">createdDateTime</span></span>|<span data-ttu-id="bbbbd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbbbd-165">DateTimeOffset</span></span>|<span data-ttu-id="bbbbd-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-166">DateTime the object was created.</span></span> <span data-ttu-id="bbbbd-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-168">说明</span><span class="sxs-lookup"><span data-stu-id="bbbbd-168">description</span></span>|<span data-ttu-id="bbbbd-169">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-169">String</span></span>|<span data-ttu-id="bbbbd-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bbbbd-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bbbbd-172">displayName</span></span>|<span data-ttu-id="bbbbd-173">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-173">String</span></span>|<span data-ttu-id="bbbbd-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bbbbd-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-176">version</span><span class="sxs-lookup"><span data-stu-id="bbbbd-176">version</span></span>|<span data-ttu-id="bbbbd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-177">Int32</span></span>|<span data-ttu-id="bbbbd-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-178">Version of the device configuration.</span></span> <span data-ttu-id="bbbbd-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="bbbbd-180">preSharedKey</span></span>|<span data-ttu-id="bbbbd-181">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-181">String</span></span>|<span data-ttu-id="bbbbd-182">这是 WPA 个人共享网络的预共享Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="bbbbd-183">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-184">wifiSecurityType</span></span>|[<span data-ttu-id="bbbbd-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="bbbbd-186">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="bbbbd-187">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="bbbbd-188">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="bbbbd-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="bbbbd-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="bbbbd-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="bbbbd-191">指定 wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="bbbbd-192">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="bbbbd-193">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="bbbbd-194">ssid</span><span class="sxs-lookup"><span data-stu-id="bbbbd-194">ssid</span></span>|<span data-ttu-id="bbbbd-195">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-195">String</span></span>|<span data-ttu-id="bbbbd-196">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="bbbbd-197">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-198">networkName</span><span class="sxs-lookup"><span data-stu-id="bbbbd-198">networkName</span></span>|<span data-ttu-id="bbbbd-199">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-199">String</span></span>|<span data-ttu-id="bbbbd-200">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-200">Specify the network configuration name.</span></span> <span data-ttu-id="bbbbd-201">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="bbbbd-202">connectAutomatically</span></span>|<span data-ttu-id="bbbbd-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-203">Boolean</span></span>|<span data-ttu-id="bbbbd-204">指定 wifi 连接是否在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="bbbbd-205">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="bbbbd-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="bbbbd-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-207">Boolean</span></span>|<span data-ttu-id="bbbbd-208">指定 wifi 连接在已连接到此网络时是否应该连接到更首选的网络。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="bbbbd-209">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="bbbbd-210">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="bbbbd-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="bbbbd-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-212">Boolean</span></span>|<span data-ttu-id="bbbbd-213">指定即使在 SSID 未广播时 wifi 连接是否应该自动连接。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="bbbbd-214">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="bbbbd-215">proxySetting</span></span>|[<span data-ttu-id="bbbbd-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="bbbbd-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="bbbbd-217">为配置指定代理Wi-Fi继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="bbbbd-218">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="bbbbd-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="bbbbd-219">proxyManualAddress</span></span>|<span data-ttu-id="bbbbd-220">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-220">String</span></span>|<span data-ttu-id="bbbbd-221">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="bbbbd-222">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="bbbbd-223">proxyManualPort</span></span>|<span data-ttu-id="bbbbd-224">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-224">Int32</span></span>|<span data-ttu-id="bbbbd-225">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="bbbbd-226">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="bbbbd-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="bbbbd-228">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-228">String</span></span>|<span data-ttu-id="bbbbd-229">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="bbbbd-230">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="bbbbd-231">forceFIPSCompliance</span></span>|<span data-ttu-id="bbbbd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-232">Boolean</span></span>|<span data-ttu-id="bbbbd-233">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="bbbbd-234">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bbbbd-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="bbbbd-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="bbbbd-235">networkSingleSignOn</span></span>|[<span data-ttu-id="bbbbd-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="bbbbd-237">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-237">Specify the network single sign on type.</span></span> <span data-ttu-id="bbbbd-238">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="bbbbd-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="bbbbd-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="bbbbd-240">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-240">Int32</span></span>|<span data-ttu-id="bbbbd-241">指定最大身份验证超时 (秒数) 。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="bbbbd-242">有效范围：1-120</span><span class="sxs-lookup"><span data-stu-id="bbbbd-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="bbbbd-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="bbbbd-243">userBasedVirtualLan</span></span>|<span data-ttu-id="bbbbd-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-244">Boolean</span></span>|<span data-ttu-id="bbbbd-245">指定是否根据用户凭据更改设备使用的虚拟 LAN。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="bbbbd-246">当 NetworkSingleSignOnType 设置为 Disabled 时，不能使用。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="bbbbd-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="bbbbd-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="bbbbd-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-248">Boolean</span></span>|<span data-ttu-id="bbbbd-249">指定 wifi 连接是否应该提示输入其他身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="bbbbd-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="bbbbd-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="bbbbd-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-251">Boolean</span></span>|<span data-ttu-id="bbbbd-252">指定 wifi 连接是否应该启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="bbbbd-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="bbbbd-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="bbbbd-254">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-254">Int32</span></span>|<span data-ttu-id="bbbbd-255">指定最大成对主密钥缓存 (分钟数) 。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="bbbbd-256">有效范围：5-1440</span><span class="sxs-lookup"><span data-stu-id="bbbbd-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="bbbbd-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="bbbbd-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="bbbbd-258">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-258">Int32</span></span>|<span data-ttu-id="bbbbd-259">指定缓存中成对主键的最大数量。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="bbbbd-260">有效范围：1-255</span><span class="sxs-lookup"><span data-stu-id="bbbbd-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="bbbbd-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="bbbbd-261">enablePreAuthentication</span></span>|<span data-ttu-id="bbbbd-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-262">Boolean</span></span>|<span data-ttu-id="bbbbd-263">指定是否应该启用预身份验证。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="bbbbd-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="bbbbd-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="bbbbd-265">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-265">Int32</span></span>|<span data-ttu-id="bbbbd-266">指定最大预身份验证尝试次数。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="bbbbd-267">有效范围：1-16</span><span class="sxs-lookup"><span data-stu-id="bbbbd-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="bbbbd-268">eapType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-268">eapType</span></span>|[<span data-ttu-id="bbbbd-269">eapType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="bbbbd-270">可扩展身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="bbbbd-271">指示在 Wi-Fi 路由器 (上设置的 EAP) 。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="bbbbd-272">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="bbbbd-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="bbbbd-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="bbbbd-274">String collection</span><span class="sxs-lookup"><span data-stu-id="bbbbd-274">String collection</span></span>|<span data-ttu-id="bbbbd-275">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="bbbbd-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bbbbd-276">authenticationMethod</span></span>|[<span data-ttu-id="bbbbd-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bbbbd-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="bbbbd-278">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-278">Specify the authentication method.</span></span> <span data-ttu-id="bbbbd-279">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="bbbbd-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="bbbbd-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="bbbbd-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="bbbbd-282">为 EAP TTLS 指定内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="bbbbd-283">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="bbbbd-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="bbbbd-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="bbbbd-285">String</span><span class="sxs-lookup"><span data-stu-id="bbbbd-285">String</span></span>|<span data-ttu-id="bbbbd-286">使用 EAP TTLS 或 PEAP 时，指定用于替换隐私用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="bbbbd-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="bbbbd-287">requireCryptographicBinding</span></span>|<span data-ttu-id="bbbbd-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-288">Boolean</span></span>|<span data-ttu-id="bbbbd-289">指定在选择 EAP 类型作为 PEAP 时是否启用加密绑定。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="bbbbd-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="bbbbd-290">performServerValidation</span></span>|<span data-ttu-id="bbbbd-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-291">Boolean</span></span>|<span data-ttu-id="bbbbd-292">指定在选择 EAP 类型作为 PEAP 时是否通过验证证书来启用服务器身份验证。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="bbbbd-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="bbbbd-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="bbbbd-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-294">Boolean</span></span>|<span data-ttu-id="bbbbd-295">指定在选择 EAP 类型作为 PEAP 时是否提示用户为受信任的证书颁发机构授权新服务器。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="bbbbd-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="bbbbd-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="bbbbd-297">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-297">Int32</span></span>|<span data-ttu-id="bbbbd-298">指定客户端在身份验证尝试失败之前等待的秒数。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="bbbbd-299">有效范围为 1-3600。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="bbbbd-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="bbbbd-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="bbbbd-301">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-301">Int32</span></span>|<span data-ttu-id="bbbbd-302">指定失败的身份验证和下一次身份验证尝试之间的秒数。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="bbbbd-303">有效范围为 1-3600。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="bbbbd-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="bbbbd-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="bbbbd-305">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-305">Int32</span></span>|<span data-ttu-id="bbbbd-306">指定在通过 LAN 发送 EAPOL (可扩展身份验证协议之前要等待的) 消息。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="bbbbd-307">有效范围为 1-3600。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="bbbbd-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="bbbbd-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="bbbbd-309">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-309">Int32</span></span>|<span data-ttu-id="bbbbd-310">指定在返回失败 (发送的通过 LAN 的 EAPOL) 可扩展身份验证协议的最大数量。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="bbbbd-311">有效范围为 1-100。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="bbbbd-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="bbbbd-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="bbbbd-313">Int32</span><span class="sxs-lookup"><span data-stu-id="bbbbd-313">Int32</span></span>|<span data-ttu-id="bbbbd-314">指定一组凭据允许的最大身份验证失败数。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="bbbbd-315">有效范围为 1-100。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="bbbbd-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="bbbbd-316">cacheCredentials</span></span>|<span data-ttu-id="bbbbd-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbbbd-317">Boolean</span></span>|<span data-ttu-id="bbbbd-318">指定是否在设备上缓存用户凭据，以便用户无需每次连接时都一直输入凭据。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="bbbbd-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-319">authenticationType</span></span>|[<span data-ttu-id="bbbbd-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="bbbbd-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="bbbbd-321">指定是对用户、设备进行身份验证，还是使用来宾身份验证， (身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="bbbbd-322">如果使用证书身份验证，请确保证书类型与身份验证类型匹配。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="bbbbd-323">可取值为：`none`、`user`、`machine`、`machineOrUser`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="bbbbd-324">响应</span><span class="sxs-lookup"><span data-stu-id="bbbbd-324">Response</span></span>
<span data-ttu-id="bbbbd-325">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbbbd-326">示例</span><span class="sxs-lookup"><span data-stu-id="bbbbd-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbbbd-327">请求</span><span class="sxs-lookup"><span data-stu-id="bbbbd-327">Request</span></span>
<span data-ttu-id="bbbbd-328">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2695

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
  "userBasedVirtualLan": true,
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
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```

### <a name="response"></a><span data-ttu-id="bbbbd-329">响应</span><span class="sxs-lookup"><span data-stu-id="bbbbd-329">Response</span></span>
<span data-ttu-id="bbbbd-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbbbd-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2867

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
  "userBasedVirtualLan": true,
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
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```




