---
title: 创建 windows10VpnConfiguration
description: 创建新的 windows10VpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05eb4933fa63e04010f65c563bc3265ac1a5b92f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122831"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="b44e7-103">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b44e7-103">Create windows10VpnConfiguration</span></span>

<span data-ttu-id="b44e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b44e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b44e7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b44e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b44e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b44e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b44e7-107">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b44e7-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b44e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b44e7-108">Prerequisites</span></span>
<span data-ttu-id="b44e7-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b44e7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b44e7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b44e7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b44e7-111">Permission type</span></span>|<span data-ttu-id="b44e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b44e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b44e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b44e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b44e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b44e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b44e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b44e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b44e7-116">Not supported.</span></span>|
|<span data-ttu-id="b44e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b44e7-117">Application</span></span>|<span data-ttu-id="b44e7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44e7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b44e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b44e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b44e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b44e7-120">Request headers</span></span>
|<span data-ttu-id="b44e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="b44e7-121">Header</span></span>|<span data-ttu-id="b44e7-122">值</span><span class="sxs-lookup"><span data-stu-id="b44e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b44e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b44e7-123">Authorization</span></span>|<span data-ttu-id="b44e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b44e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b44e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="b44e7-125">Accept</span></span>|<span data-ttu-id="b44e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b44e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b44e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b44e7-127">Request body</span></span>
<span data-ttu-id="b44e7-128">在请求正文中，提供 windows10VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b44e7-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="b44e7-129">下表显示创建 windows10VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b44e7-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="b44e7-130">属性</span><span class="sxs-lookup"><span data-stu-id="b44e7-130">Property</span></span>|<span data-ttu-id="b44e7-131">类型</span><span class="sxs-lookup"><span data-stu-id="b44e7-131">Type</span></span>|<span data-ttu-id="b44e7-132">说明</span><span class="sxs-lookup"><span data-stu-id="b44e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b44e7-133">id</span><span class="sxs-lookup"><span data-stu-id="b44e7-133">id</span></span>|<span data-ttu-id="b44e7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b44e7-134">String</span></span>|<span data-ttu-id="b44e7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b44e7-135">Key of the entity.</span></span> <span data-ttu-id="b44e7-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b44e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b44e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b44e7-138">DateTimeOffset</span></span>|<span data-ttu-id="b44e7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b44e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b44e7-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b44e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="b44e7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b44e7-142">String collection</span></span>|<span data-ttu-id="b44e7-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b44e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b44e7-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b44e7-145">supportsScopeTags</span></span>|<span data-ttu-id="b44e7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-146">Boolean</span></span>|<span data-ttu-id="b44e7-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b44e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b44e7-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b44e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b44e7-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b44e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b44e7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b44e7-150">This property is read-only.</span></span> <span data-ttu-id="b44e7-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b44e7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b44e7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b44e7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b44e7-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b44e7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b44e7-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b44e7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b44e7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b44e7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b44e7-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b44e7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b44e7-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b44e7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b44e7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b44e7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b44e7-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b44e7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b44e7-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b44e7-164">createdDateTime</span></span>|<span data-ttu-id="b44e7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b44e7-165">DateTimeOffset</span></span>|<span data-ttu-id="b44e7-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b44e7-166">DateTime the object was created.</span></span> <span data-ttu-id="b44e7-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-168">说明</span><span class="sxs-lookup"><span data-stu-id="b44e7-168">description</span></span>|<span data-ttu-id="b44e7-169">String</span><span class="sxs-lookup"><span data-stu-id="b44e7-169">String</span></span>|<span data-ttu-id="b44e7-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b44e7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b44e7-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b44e7-172">displayName</span></span>|<span data-ttu-id="b44e7-173">String</span><span class="sxs-lookup"><span data-stu-id="b44e7-173">String</span></span>|<span data-ttu-id="b44e7-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b44e7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b44e7-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-176">version</span><span class="sxs-lookup"><span data-stu-id="b44e7-176">version</span></span>|<span data-ttu-id="b44e7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b44e7-177">Int32</span></span>|<span data-ttu-id="b44e7-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b44e7-178">Version of the device configuration.</span></span> <span data-ttu-id="b44e7-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="b44e7-180">connectionName</span></span>|<span data-ttu-id="b44e7-181">String</span><span class="sxs-lookup"><span data-stu-id="b44e7-181">String</span></span>|<span data-ttu-id="b44e7-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="b44e7-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b44e7-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-184">台</span><span class="sxs-lookup"><span data-stu-id="b44e7-184">servers</span></span>|<span data-ttu-id="b44e7-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="b44e7-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b44e7-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="b44e7-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="b44e7-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="b44e7-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b44e7-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b44e7-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b44e7-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44e7-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-190">customXml</span><span class="sxs-lookup"><span data-stu-id="b44e7-190">customXml</span></span>|<span data-ttu-id="b44e7-191">Binary</span><span class="sxs-lookup"><span data-stu-id="b44e7-191">Binary</span></span>|<span data-ttu-id="b44e7-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="b44e7-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b44e7-193">从[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)继承的 (UTF8 编码的字节数组) </span><span class="sxs-lookup"><span data-stu-id="b44e7-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44e7-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="b44e7-194">profileTarget</span></span>|[<span data-ttu-id="b44e7-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="b44e7-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="b44e7-196">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="b44e7-196">Profile target type.</span></span> <span data-ttu-id="b44e7-197">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="b44e7-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="b44e7-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="b44e7-198">connectionType</span></span>|[<span data-ttu-id="b44e7-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b44e7-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="b44e7-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="b44e7-200">Connection type.</span></span> <span data-ttu-id="b44e7-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="b44e7-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="b44e7-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b44e7-202">enableSplitTunneling</span></span>|<span data-ttu-id="b44e7-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-203">Boolean</span></span>|<span data-ttu-id="b44e7-204">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="b44e7-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="b44e7-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="b44e7-205">enableAlwaysOn</span></span>|<span data-ttu-id="b44e7-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-206">Boolean</span></span>|<span data-ttu-id="b44e7-207">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="b44e7-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="b44e7-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="b44e7-208">enableDeviceTunnel</span></span>|<span data-ttu-id="b44e7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-209">Boolean</span></span>|<span data-ttu-id="b44e7-210">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="b44e7-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="b44e7-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="b44e7-211">enableDnsRegistration</span></span>|<span data-ttu-id="b44e7-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-212">Boolean</span></span>|<span data-ttu-id="b44e7-213">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="b44e7-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="b44e7-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="b44e7-214">dnsSuffixes</span></span>|<span data-ttu-id="b44e7-215">String collection</span><span class="sxs-lookup"><span data-stu-id="b44e7-215">String collection</span></span>|<span data-ttu-id="b44e7-216">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="b44e7-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="b44e7-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b44e7-217">authenticationMethod</span></span>|[<span data-ttu-id="b44e7-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b44e7-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="b44e7-219">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b44e7-219">Authentication method.</span></span> <span data-ttu-id="b44e7-220">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="b44e7-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b44e7-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="b44e7-221">rememberUserCredentials</span></span>|<span data-ttu-id="b44e7-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-222">Boolean</span></span>|<span data-ttu-id="b44e7-223">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="b44e7-223">Remember user credentials.</span></span>|
|<span data-ttu-id="b44e7-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b44e7-224">enableConditionalAccess</span></span>|<span data-ttu-id="b44e7-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-225">Boolean</span></span>|<span data-ttu-id="b44e7-226">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="b44e7-226">Enable conditional access.</span></span>|
|<span data-ttu-id="b44e7-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="b44e7-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="b44e7-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-228">Boolean</span></span>|<span data-ttu-id="b44e7-229">启用具有备用证书的单一登录 (SSO) 。</span><span class="sxs-lookup"><span data-stu-id="b44e7-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="b44e7-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="b44e7-230">singleSignOnEku</span></span>|[<span data-ttu-id="b44e7-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="b44e7-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="b44e7-232">单一登录扩展密钥用法 (EKU) 。</span><span class="sxs-lookup"><span data-stu-id="b44e7-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="b44e7-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="b44e7-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="b44e7-234">String</span><span class="sxs-lookup"><span data-stu-id="b44e7-234">String</span></span>|<span data-ttu-id="b44e7-235">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="b44e7-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="b44e7-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="b44e7-236">eapXml</span></span>|<span data-ttu-id="b44e7-237">Binary</span><span class="sxs-lookup"><span data-stu-id="b44e7-237">Binary</span></span>|<span data-ttu-id="b44e7-238">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="b44e7-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="b44e7-239">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="b44e7-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="b44e7-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b44e7-240">proxyServer</span></span>|[<span data-ttu-id="b44e7-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b44e7-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="b44e7-242">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="b44e7-242">Proxy Server.</span></span>|
|<span data-ttu-id="b44e7-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="b44e7-243">associatedApps</span></span>|<span data-ttu-id="b44e7-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="b44e7-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="b44e7-245">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="b44e7-245">Associated Apps.</span></span> <span data-ttu-id="b44e7-246">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b44e7-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b44e7-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="b44e7-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="b44e7-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44e7-248">Boolean</span></span>|<span data-ttu-id="b44e7-249">仅关联的应用程序可以使用 (每应用 VPN) 的连接。</span><span class="sxs-lookup"><span data-stu-id="b44e7-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="b44e7-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="b44e7-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="b44e7-251">String</span><span class="sxs-lookup"><span data-stu-id="b44e7-251">String</span></span>|<span data-ttu-id="b44e7-252">与此连接关联的 Windows 信息保护 (与此连接关联的 WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="b44e7-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="b44e7-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="b44e7-253">trafficRules</span></span>|<span data-ttu-id="b44e7-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="b44e7-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="b44e7-255">流量规则。</span><span class="sxs-lookup"><span data-stu-id="b44e7-255">Traffic rules.</span></span> <span data-ttu-id="b44e7-256">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b44e7-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b44e7-257">航线</span><span class="sxs-lookup"><span data-stu-id="b44e7-257">routes</span></span>|<span data-ttu-id="b44e7-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="b44e7-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="b44e7-259"> (第三方提供商) 的路由可选。</span><span class="sxs-lookup"><span data-stu-id="b44e7-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="b44e7-260">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b44e7-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b44e7-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="b44e7-261">dnsRules</span></span>|<span data-ttu-id="b44e7-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="b44e7-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="b44e7-263">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="b44e7-263">DNS rules.</span></span> <span data-ttu-id="b44e7-264">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b44e7-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b44e7-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="b44e7-265">trustedNetworkDomains</span></span>|<span data-ttu-id="b44e7-266">String collection</span><span class="sxs-lookup"><span data-stu-id="b44e7-266">String collection</span></span>|<span data-ttu-id="b44e7-267">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="b44e7-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="b44e7-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="b44e7-268">cryptographySuite</span></span>|[<span data-ttu-id="b44e7-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="b44e7-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="b44e7-270">Windows10 及更高版本中 IKEv2 VPN 的加密套件安全设置</span><span class="sxs-lookup"><span data-stu-id="b44e7-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="b44e7-271">响应</span><span class="sxs-lookup"><span data-stu-id="b44e7-271">Response</span></span>
<span data-ttu-id="b44e7-272">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b44e7-272">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b44e7-273">示例</span><span class="sxs-lookup"><span data-stu-id="b44e7-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="b44e7-274">请求</span><span class="sxs-lookup"><span data-stu-id="b44e7-274">Request</span></span>
<span data-ttu-id="b44e7-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b44e7-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="b44e7-276">响应</span><span class="sxs-lookup"><span data-stu-id="b44e7-276">Response</span></span>
<span data-ttu-id="b44e7-277">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b44e7-277">Here is an example of the response.</span></span> <span data-ttu-id="b44e7-278">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b44e7-278">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b44e7-279">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b44e7-279">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



