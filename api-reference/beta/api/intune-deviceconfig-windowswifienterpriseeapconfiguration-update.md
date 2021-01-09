---
title: 更新 windowsWifiEnterpriseEAPConfiguration
description: 更新 windowsWifiEnterpriseEAPConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d092d4fd5cec9edd1ac102a935c63d9a96501808
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790718"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="1a48e-103">更新 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a48e-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="1a48e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a48e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a48e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a48e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a48e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a48e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a48e-107">更新 [windowsWifiEnterpriseEAPConfiguration 对象](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1a48e-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a48e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a48e-108">Prerequisites</span></span>
<span data-ttu-id="1a48e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a48e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a48e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a48e-111">Permission type</span></span>|<span data-ttu-id="1a48e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a48e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a48e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a48e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a48e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a48e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a48e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a48e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a48e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a48e-116">Not supported.</span></span>|
|<span data-ttu-id="1a48e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a48e-117">Application</span></span>|<span data-ttu-id="1a48e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a48e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a48e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a48e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1a48e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a48e-120">Request headers</span></span>
|<span data-ttu-id="1a48e-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a48e-121">Header</span></span>|<span data-ttu-id="1a48e-122">值</span><span class="sxs-lookup"><span data-stu-id="1a48e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a48e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a48e-123">Authorization</span></span>|<span data-ttu-id="1a48e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a48e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a48e-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a48e-125">Accept</span></span>|<span data-ttu-id="1a48e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a48e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a48e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a48e-127">Request body</span></span>
<span data-ttu-id="1a48e-128">在请求正文中，提供 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a48e-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="1a48e-129">下表显示创建 [windowsWifiEnterpriseEAPConfiguration 时所需的属性](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1a48e-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="1a48e-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a48e-130">Property</span></span>|<span data-ttu-id="1a48e-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a48e-131">Type</span></span>|<span data-ttu-id="1a48e-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a48e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a48e-133">id</span><span class="sxs-lookup"><span data-stu-id="1a48e-133">id</span></span>|<span data-ttu-id="1a48e-134">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-134">String</span></span>|<span data-ttu-id="1a48e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a48e-135">Key of the entity.</span></span> <span data-ttu-id="1a48e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a48e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1a48e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a48e-138">DateTimeOffset</span></span>|<span data-ttu-id="1a48e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a48e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1a48e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a48e-141">roleScopeTagIds</span></span>|<span data-ttu-id="1a48e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="1a48e-142">String collection</span></span>|<span data-ttu-id="1a48e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1a48e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a48e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a48e-145">supportsScopeTags</span></span>|<span data-ttu-id="1a48e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-146">Boolean</span></span>|<span data-ttu-id="1a48e-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="1a48e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a48e-148">如果此值为 false 且实体对范围用户不可见，则不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1a48e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a48e-149">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="1a48e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a48e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1a48e-150">This property is read-only.</span></span> <span data-ttu-id="1a48e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1a48e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1a48e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1a48e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1a48e-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="1a48e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1a48e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1a48e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1a48e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1a48e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1a48e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1a48e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1a48e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1a48e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1a48e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1a48e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1a48e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1a48e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1a48e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a48e-164">createdDateTime</span></span>|<span data-ttu-id="1a48e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a48e-165">DateTimeOffset</span></span>|<span data-ttu-id="1a48e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a48e-166">DateTime the object was created.</span></span> <span data-ttu-id="1a48e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-168">description</span><span class="sxs-lookup"><span data-stu-id="1a48e-168">description</span></span>|<span data-ttu-id="1a48e-169">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-169">String</span></span>|<span data-ttu-id="1a48e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1a48e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a48e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1a48e-172">displayName</span></span>|<span data-ttu-id="1a48e-173">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-173">String</span></span>|<span data-ttu-id="1a48e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1a48e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a48e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-176">version</span><span class="sxs-lookup"><span data-stu-id="1a48e-176">version</span></span>|<span data-ttu-id="1a48e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-177">Int32</span></span>|<span data-ttu-id="1a48e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1a48e-178">Version of the device configuration.</span></span> <span data-ttu-id="1a48e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="1a48e-180">preSharedKey</span></span>|<span data-ttu-id="1a48e-181">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-181">String</span></span>|<span data-ttu-id="1a48e-182">这是 WPA 个人用户网络预Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="1a48e-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="1a48e-183">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="1a48e-184">wifiSecurityType</span></span>|[<span data-ttu-id="1a48e-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="1a48e-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="1a48e-186">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="1a48e-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="1a48e-187">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1a48e-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="1a48e-188">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="1a48e-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="1a48e-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="1a48e-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="1a48e-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="1a48e-191">指定 Wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="1a48e-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="1a48e-192">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1a48e-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="1a48e-193">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="1a48e-194">ssid</span><span class="sxs-lookup"><span data-stu-id="1a48e-194">ssid</span></span>|<span data-ttu-id="1a48e-195">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-195">String</span></span>|<span data-ttu-id="1a48e-196">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="1a48e-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="1a48e-197">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-198">networkName</span><span class="sxs-lookup"><span data-stu-id="1a48e-198">networkName</span></span>|<span data-ttu-id="1a48e-199">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-199">String</span></span>|<span data-ttu-id="1a48e-200">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="1a48e-200">Specify the network configuration name.</span></span> <span data-ttu-id="1a48e-201">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="1a48e-202">connectAutomatically</span></span>|<span data-ttu-id="1a48e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-203">Boolean</span></span>|<span data-ttu-id="1a48e-204">指定 wifi 连接在范围内时是否自动连接。</span><span class="sxs-lookup"><span data-stu-id="1a48e-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="1a48e-205">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="1a48e-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="1a48e-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-207">Boolean</span></span>|<span data-ttu-id="1a48e-208">指定 Wifi 连接在已连接到此网络时是否应连接到更多首选网络。</span><span class="sxs-lookup"><span data-stu-id="1a48e-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="1a48e-209">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="1a48e-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="1a48e-210">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="1a48e-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="1a48e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-212">Boolean</span></span>|<span data-ttu-id="1a48e-213">指定即使 SSID 未广播，wifi 连接也应自动连接。</span><span class="sxs-lookup"><span data-stu-id="1a48e-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="1a48e-214">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="1a48e-215">proxySetting</span></span>|[<span data-ttu-id="1a48e-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="1a48e-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="1a48e-217">指定客户端配置的代理Wi-Fi 继承自[windowsWifiConfiguration。](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="1a48e-218">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="1a48e-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="1a48e-219">proxyManualAddress</span></span>|<span data-ttu-id="1a48e-220">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-220">String</span></span>|<span data-ttu-id="1a48e-221">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="1a48e-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="1a48e-222">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="1a48e-223">proxyManualPort</span></span>|<span data-ttu-id="1a48e-224">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-224">Int32</span></span>|<span data-ttu-id="1a48e-225">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="1a48e-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="1a48e-226">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="1a48e-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="1a48e-228">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-228">String</span></span>|<span data-ttu-id="1a48e-229">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="1a48e-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="1a48e-230">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="1a48e-231">forceFIPSCompliance</span></span>|<span data-ttu-id="1a48e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-232">Boolean</span></span>|<span data-ttu-id="1a48e-233">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="1a48e-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="1a48e-234">继承自 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a48e-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1a48e-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="1a48e-235">networkSingleSignOn</span></span>|[<span data-ttu-id="1a48e-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="1a48e-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="1a48e-237">指定网络单一登录类型。</span><span class="sxs-lookup"><span data-stu-id="1a48e-237">Specify the network single sign on type.</span></span> <span data-ttu-id="1a48e-238">可取值为：`disabled`、`prelogon`、`postlogon`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="1a48e-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="1a48e-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="1a48e-240">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-240">Int32</span></span>|<span data-ttu-id="1a48e-241">指定最大身份验证超时 (秒数) 。</span><span class="sxs-lookup"><span data-stu-id="1a48e-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="1a48e-242">有效范围：1-120</span><span class="sxs-lookup"><span data-stu-id="1a48e-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="1a48e-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="1a48e-243">userBasedVirtualLan</span></span>|<span data-ttu-id="1a48e-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-244">Boolean</span></span>|<span data-ttu-id="1a48e-245">指定是否根据用户凭据更改设备使用的虚拟 LAN。</span><span class="sxs-lookup"><span data-stu-id="1a48e-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="1a48e-246">当 NetworkSingleSignOnType 设置为"已禁用"时，不能使用。</span><span class="sxs-lookup"><span data-stu-id="1a48e-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="1a48e-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="1a48e-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="1a48e-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-248">Boolean</span></span>|<span data-ttu-id="1a48e-249">指定 wifi 连接是否应该提示输入其他身份验证凭据。</span><span class="sxs-lookup"><span data-stu-id="1a48e-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="1a48e-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="1a48e-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="1a48e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-251">Boolean</span></span>|<span data-ttu-id="1a48e-252">指定 wifi 连接是否应该启用成对主密钥缓存。</span><span class="sxs-lookup"><span data-stu-id="1a48e-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="1a48e-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1a48e-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="1a48e-254">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-254">Int32</span></span>|<span data-ttu-id="1a48e-255">指定最大成对主密钥缓存 (分钟数) 。</span><span class="sxs-lookup"><span data-stu-id="1a48e-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="1a48e-256">有效范围：5-1440</span><span class="sxs-lookup"><span data-stu-id="1a48e-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="1a48e-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="1a48e-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="1a48e-258">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-258">Int32</span></span>|<span data-ttu-id="1a48e-259">指定缓存中成对主键的最大数量。</span><span class="sxs-lookup"><span data-stu-id="1a48e-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="1a48e-260">有效范围：1-255</span><span class="sxs-lookup"><span data-stu-id="1a48e-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="1a48e-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="1a48e-261">enablePreAuthentication</span></span>|<span data-ttu-id="1a48e-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-262">Boolean</span></span>|<span data-ttu-id="1a48e-263">指定是否应该启用预身份验证。</span><span class="sxs-lookup"><span data-stu-id="1a48e-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="1a48e-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="1a48e-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="1a48e-265">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-265">Int32</span></span>|<span data-ttu-id="1a48e-266">指定最大身份验证前尝试次数。</span><span class="sxs-lookup"><span data-stu-id="1a48e-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="1a48e-267">有效范围：1-16</span><span class="sxs-lookup"><span data-stu-id="1a48e-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="1a48e-268">eapType</span><span class="sxs-lookup"><span data-stu-id="1a48e-268">eapType</span></span>|[<span data-ttu-id="1a48e-269">eapType</span><span class="sxs-lookup"><span data-stu-id="1a48e-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="1a48e-270">可扩展身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="1a48e-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="1a48e-271">指示在路由器或路由器Wi-Fi上设置的 EAP () 。</span><span class="sxs-lookup"><span data-stu-id="1a48e-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="1a48e-272">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="1a48e-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="1a48e-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="1a48e-274">String collection</span><span class="sxs-lookup"><span data-stu-id="1a48e-274">String collection</span></span>|<span data-ttu-id="1a48e-275">指定受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="1a48e-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="1a48e-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1a48e-276">authenticationMethod</span></span>|[<span data-ttu-id="1a48e-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1a48e-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="1a48e-278">指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="1a48e-278">Specify the authentication method.</span></span> <span data-ttu-id="1a48e-279">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="1a48e-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="1a48e-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="1a48e-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="1a48e-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="1a48e-282">指定 EAP TTLS 的内部身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="1a48e-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="1a48e-283">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="1a48e-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="1a48e-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="1a48e-285">String</span><span class="sxs-lookup"><span data-stu-id="1a48e-285">String</span></span>|<span data-ttu-id="1a48e-286">指定在使用 EAP TTLS 或 PEAP 时替换用于隐私的用户名的字符串。</span><span class="sxs-lookup"><span data-stu-id="1a48e-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="1a48e-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="1a48e-287">requireCryptographicBinding</span></span>|<span data-ttu-id="1a48e-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-288">Boolean</span></span>|<span data-ttu-id="1a48e-289">指定在选择 EAP 类型作为 PEAP 时是否启用加密绑定。</span><span class="sxs-lookup"><span data-stu-id="1a48e-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="1a48e-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="1a48e-290">performServerValidation</span></span>|<span data-ttu-id="1a48e-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-291">Boolean</span></span>|<span data-ttu-id="1a48e-292">指定在选择 EAP 类型作为 PEAP 时，是否通过验证证书来启用对服务器标识的验证。</span><span class="sxs-lookup"><span data-stu-id="1a48e-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="1a48e-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="1a48e-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="1a48e-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-294">Boolean</span></span>|<span data-ttu-id="1a48e-295">指定在选择 EAP 类型作为 PEAP 时是否提示用户为受信任的证书颁发机构授权新服务器。</span><span class="sxs-lookup"><span data-stu-id="1a48e-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="1a48e-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="1a48e-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="1a48e-297">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-297">Int32</span></span>|<span data-ttu-id="1a48e-298">指定客户端在身份验证尝试失败之前等待的秒数。</span><span class="sxs-lookup"><span data-stu-id="1a48e-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="1a48e-299">有效范围为 1-3600。</span><span class="sxs-lookup"><span data-stu-id="1a48e-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="1a48e-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="1a48e-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="1a48e-301">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-301">Int32</span></span>|<span data-ttu-id="1a48e-302">指定身份验证失败和下一次身份验证尝试之间的秒数。</span><span class="sxs-lookup"><span data-stu-id="1a48e-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="1a48e-303">有效范围为 1-3600。</span><span class="sxs-lookup"><span data-stu-id="1a48e-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="1a48e-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="1a48e-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="1a48e-305">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-305">Int32</span></span>|<span data-ttu-id="1a48e-306">指定在通过 LAN 或"开始"消息发送 EAPOL (可扩展身份验证协议) 的秒数。</span><span class="sxs-lookup"><span data-stu-id="1a48e-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="1a48e-307">有效范围为 1-3600。</span><span class="sxs-lookup"><span data-stu-id="1a48e-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="1a48e-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="1a48e-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="1a48e-309">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-309">Int32</span></span>|<span data-ttu-id="1a48e-310">指定在返回失败之前 (发送的通过 LAN 的可扩展身份验证协议) EAPOL 协议的最大数量。</span><span class="sxs-lookup"><span data-stu-id="1a48e-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="1a48e-311">有效范围为 1-100。</span><span class="sxs-lookup"><span data-stu-id="1a48e-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="1a48e-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="1a48e-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="1a48e-313">Int32</span><span class="sxs-lookup"><span data-stu-id="1a48e-313">Int32</span></span>|<span data-ttu-id="1a48e-314">指定一组凭据允许的最大身份验证失败数。</span><span class="sxs-lookup"><span data-stu-id="1a48e-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="1a48e-315">有效范围为 1-100。</span><span class="sxs-lookup"><span data-stu-id="1a48e-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="1a48e-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="1a48e-316">cacheCredentials</span></span>|<span data-ttu-id="1a48e-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a48e-317">Boolean</span></span>|<span data-ttu-id="1a48e-318">指定是否在设备上缓存用户凭据，以便用户无需每次连接时都继续输入凭据。</span><span class="sxs-lookup"><span data-stu-id="1a48e-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="1a48e-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="1a48e-319">authenticationType</span></span>|[<span data-ttu-id="1a48e-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="1a48e-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="1a48e-321">指定是对用户、设备进行身份验证，还是使用来宾身份验证， (身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="1a48e-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="1a48e-322">如果使用的是证书身份验证，请确保证书类型与身份验证类型匹配。</span><span class="sxs-lookup"><span data-stu-id="1a48e-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="1a48e-323">可取值为：`none`、`user`、`machine`、`machineOrUser`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="1a48e-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="1a48e-324">响应</span><span class="sxs-lookup"><span data-stu-id="1a48e-324">Response</span></span>
<span data-ttu-id="1a48e-325">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a48e-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a48e-326">示例</span><span class="sxs-lookup"><span data-stu-id="1a48e-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a48e-327">请求</span><span class="sxs-lookup"><span data-stu-id="1a48e-327">Request</span></span>
<span data-ttu-id="1a48e-328">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a48e-328">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a48e-329">响应</span><span class="sxs-lookup"><span data-stu-id="1a48e-329">Response</span></span>
<span data-ttu-id="1a48e-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a48e-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




