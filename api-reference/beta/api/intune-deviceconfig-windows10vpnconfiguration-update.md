---
title: 更新 windows10VpnConfiguration
description: 更新 windows10VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b960115db5145e087fda3b1e02a5110ac8987346
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792588"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="95478-103">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="95478-103">Update windows10VpnConfiguration</span></span>

<span data-ttu-id="95478-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95478-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95478-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95478-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95478-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95478-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95478-107">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95478-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95478-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="95478-108">Prerequisites</span></span>
<span data-ttu-id="95478-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="95478-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="95478-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95478-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95478-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="95478-111">Permission type</span></span>|<span data-ttu-id="95478-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95478-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95478-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95478-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95478-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95478-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95478-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95478-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95478-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="95478-116">Not supported.</span></span>|
|<span data-ttu-id="95478-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="95478-117">Application</span></span>|<span data-ttu-id="95478-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95478-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95478-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95478-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="95478-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="95478-120">Request headers</span></span>
|<span data-ttu-id="95478-121">标头</span><span class="sxs-lookup"><span data-stu-id="95478-121">Header</span></span>|<span data-ttu-id="95478-122">值</span><span class="sxs-lookup"><span data-stu-id="95478-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95478-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95478-123">Authorization</span></span>|<span data-ttu-id="95478-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95478-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95478-125">接受</span><span class="sxs-lookup"><span data-stu-id="95478-125">Accept</span></span>|<span data-ttu-id="95478-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95478-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95478-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95478-127">Request body</span></span>
<span data-ttu-id="95478-128">在请求正文中，提供[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95478-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="95478-129">下表显示创建[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95478-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="95478-130">属性</span><span class="sxs-lookup"><span data-stu-id="95478-130">Property</span></span>|<span data-ttu-id="95478-131">类型</span><span class="sxs-lookup"><span data-stu-id="95478-131">Type</span></span>|<span data-ttu-id="95478-132">说明</span><span class="sxs-lookup"><span data-stu-id="95478-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95478-133">id</span><span class="sxs-lookup"><span data-stu-id="95478-133">id</span></span>|<span data-ttu-id="95478-134">字符串</span><span class="sxs-lookup"><span data-stu-id="95478-134">String</span></span>|<span data-ttu-id="95478-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="95478-135">Key of the entity.</span></span> <span data-ttu-id="95478-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95478-137">lastModifiedDateTime</span></span>|<span data-ttu-id="95478-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95478-138">DateTimeOffset</span></span>|<span data-ttu-id="95478-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95478-139">DateTime the object was last modified.</span></span> <span data-ttu-id="95478-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95478-141">roleScopeTagIds</span></span>|<span data-ttu-id="95478-142">String collection</span><span class="sxs-lookup"><span data-stu-id="95478-142">String collection</span></span>|<span data-ttu-id="95478-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="95478-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95478-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95478-145">supportsScopeTags</span></span>|<span data-ttu-id="95478-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-146">Boolean</span></span>|<span data-ttu-id="95478-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="95478-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95478-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="95478-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95478-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="95478-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95478-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="95478-150">This property is read-only.</span></span> <span data-ttu-id="95478-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95478-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="95478-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95478-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="95478-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="95478-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="95478-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95478-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="95478-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95478-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="95478-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="95478-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="95478-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="95478-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="95478-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="95478-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="95478-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="95478-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="95478-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95478-164">createdDateTime</span></span>|<span data-ttu-id="95478-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95478-165">DateTimeOffset</span></span>|<span data-ttu-id="95478-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95478-166">DateTime the object was created.</span></span> <span data-ttu-id="95478-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-168">说明</span><span class="sxs-lookup"><span data-stu-id="95478-168">description</span></span>|<span data-ttu-id="95478-169">String</span><span class="sxs-lookup"><span data-stu-id="95478-169">String</span></span>|<span data-ttu-id="95478-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="95478-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95478-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-172">displayName</span><span class="sxs-lookup"><span data-stu-id="95478-172">displayName</span></span>|<span data-ttu-id="95478-173">String</span><span class="sxs-lookup"><span data-stu-id="95478-173">String</span></span>|<span data-ttu-id="95478-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="95478-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95478-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-176">version</span><span class="sxs-lookup"><span data-stu-id="95478-176">version</span></span>|<span data-ttu-id="95478-177">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-177">Int32</span></span>|<span data-ttu-id="95478-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="95478-178">Version of the device configuration.</span></span> <span data-ttu-id="95478-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="95478-180">connectionName</span></span>|<span data-ttu-id="95478-181">String</span><span class="sxs-lookup"><span data-stu-id="95478-181">String</span></span>|<span data-ttu-id="95478-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="95478-182">Connection name displayed to the user.</span></span> <span data-ttu-id="95478-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="95478-184">台</span><span class="sxs-lookup"><span data-stu-id="95478-184">servers</span></span>|<span data-ttu-id="95478-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="95478-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="95478-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="95478-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="95478-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="95478-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="95478-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="95478-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="95478-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="95478-190">customXml</span><span class="sxs-lookup"><span data-stu-id="95478-190">customXml</span></span>|<span data-ttu-id="95478-191">Binary</span><span class="sxs-lookup"><span data-stu-id="95478-191">Binary</span></span>|<span data-ttu-id="95478-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="95478-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="95478-193">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="95478-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="95478-194">profileTarget</span></span>|[<span data-ttu-id="95478-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="95478-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="95478-196">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="95478-196">Profile target type.</span></span> <span data-ttu-id="95478-197">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="95478-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="95478-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="95478-198">connectionType</span></span>|[<span data-ttu-id="95478-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="95478-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="95478-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="95478-200">Connection type.</span></span> <span data-ttu-id="95478-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="95478-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="95478-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="95478-202">enableSplitTunneling</span></span>|<span data-ttu-id="95478-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-203">Boolean</span></span>|<span data-ttu-id="95478-204">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="95478-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="95478-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="95478-205">enableAlwaysOn</span></span>|<span data-ttu-id="95478-206">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-206">Boolean</span></span>|<span data-ttu-id="95478-207">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="95478-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="95478-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="95478-208">enableDeviceTunnel</span></span>|<span data-ttu-id="95478-209">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-209">Boolean</span></span>|<span data-ttu-id="95478-210">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="95478-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="95478-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="95478-211">enableDnsRegistration</span></span>|<span data-ttu-id="95478-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-212">Boolean</span></span>|<span data-ttu-id="95478-213">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="95478-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="95478-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="95478-214">dnsSuffixes</span></span>|<span data-ttu-id="95478-215">String collection</span><span class="sxs-lookup"><span data-stu-id="95478-215">String collection</span></span>|<span data-ttu-id="95478-216">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="95478-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="95478-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="95478-217">authenticationMethod</span></span>|[<span data-ttu-id="95478-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="95478-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="95478-219">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="95478-219">Authentication method.</span></span> <span data-ttu-id="95478-220">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="95478-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="95478-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="95478-221">rememberUserCredentials</span></span>|<span data-ttu-id="95478-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-222">Boolean</span></span>|<span data-ttu-id="95478-223">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="95478-223">Remember user credentials.</span></span>|
|<span data-ttu-id="95478-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="95478-224">enableConditionalAccess</span></span>|<span data-ttu-id="95478-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-225">Boolean</span></span>|<span data-ttu-id="95478-226">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="95478-226">Enable conditional access.</span></span>|
|<span data-ttu-id="95478-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="95478-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="95478-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-228">Boolean</span></span>|<span data-ttu-id="95478-229">启用具有备用证书的单一登录（SSO）。</span><span class="sxs-lookup"><span data-stu-id="95478-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="95478-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="95478-230">singleSignOnEku</span></span>|[<span data-ttu-id="95478-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="95478-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="95478-232">单一登录扩展密钥用法（EKU）。</span><span class="sxs-lookup"><span data-stu-id="95478-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="95478-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="95478-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="95478-234">String</span><span class="sxs-lookup"><span data-stu-id="95478-234">String</span></span>|<span data-ttu-id="95478-235">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="95478-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="95478-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="95478-236">eapXml</span></span>|<span data-ttu-id="95478-237">Binary</span><span class="sxs-lookup"><span data-stu-id="95478-237">Binary</span></span>|<span data-ttu-id="95478-238">可扩展的身份验证协议（EAP） XML。</span><span class="sxs-lookup"><span data-stu-id="95478-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="95478-239">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="95478-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="95478-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="95478-240">proxyServer</span></span>|[<span data-ttu-id="95478-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="95478-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="95478-242">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="95478-242">Proxy Server.</span></span>|
|<span data-ttu-id="95478-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="95478-243">associatedApps</span></span>|<span data-ttu-id="95478-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="95478-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="95478-245">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="95478-245">Associated Apps.</span></span> <span data-ttu-id="95478-246">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="95478-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="95478-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="95478-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="95478-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="95478-248">Boolean</span></span>|<span data-ttu-id="95478-249">仅关联的应用程序可以使用连接（每个应用 VPN）。</span><span class="sxs-lookup"><span data-stu-id="95478-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="95478-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="95478-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="95478-251">String</span><span class="sxs-lookup"><span data-stu-id="95478-251">String</span></span>|<span data-ttu-id="95478-252">与此连接关联的 Windows 信息保护（WIP）域。</span><span class="sxs-lookup"><span data-stu-id="95478-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="95478-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="95478-253">trafficRules</span></span>|<span data-ttu-id="95478-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="95478-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="95478-255">流量规则。</span><span class="sxs-lookup"><span data-stu-id="95478-255">Traffic rules.</span></span> <span data-ttu-id="95478-256">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="95478-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="95478-257">航线</span><span class="sxs-lookup"><span data-stu-id="95478-257">routes</span></span>|<span data-ttu-id="95478-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="95478-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="95478-259">路由（可选用于第三方提供程序）。</span><span class="sxs-lookup"><span data-stu-id="95478-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="95478-260">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="95478-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="95478-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="95478-261">dnsRules</span></span>|<span data-ttu-id="95478-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="95478-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="95478-263">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="95478-263">DNS rules.</span></span> <span data-ttu-id="95478-264">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="95478-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="95478-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="95478-265">trustedNetworkDomains</span></span>|<span data-ttu-id="95478-266">String collection</span><span class="sxs-lookup"><span data-stu-id="95478-266">String collection</span></span>|<span data-ttu-id="95478-267">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="95478-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="95478-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="95478-268">cryptographySuite</span></span>|[<span data-ttu-id="95478-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="95478-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="95478-270">Windows10 及更高版本中 IKEv2 VPN 的加密套件安全设置</span><span class="sxs-lookup"><span data-stu-id="95478-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="95478-271">响应</span><span class="sxs-lookup"><span data-stu-id="95478-271">Response</span></span>
<span data-ttu-id="95478-272">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95478-272">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95478-273">示例</span><span class="sxs-lookup"><span data-stu-id="95478-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="95478-274">请求</span><span class="sxs-lookup"><span data-stu-id="95478-274">Request</span></span>
<span data-ttu-id="95478-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95478-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4463

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```

### <a name="response"></a><span data-ttu-id="95478-276">响应</span><span class="sxs-lookup"><span data-stu-id="95478-276">Response</span></span>
<span data-ttu-id="95478-277">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="95478-277">Here is an example of the response.</span></span> <span data-ttu-id="95478-278">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="95478-278">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="95478-279">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="95478-279">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4635

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```



