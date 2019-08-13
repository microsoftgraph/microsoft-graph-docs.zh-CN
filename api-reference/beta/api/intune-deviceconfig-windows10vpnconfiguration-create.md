---
title: 创建 windows10VpnConfiguration
description: 创建新的 windows10VpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bdc0ae8261061fac4fd0e63dfb3bb2a4f3901f85
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314292"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="443c1-103">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="443c1-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="443c1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="443c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="443c1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="443c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="443c1-106">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="443c1-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="443c1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="443c1-107">Prerequisites</span></span>
<span data-ttu-id="443c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="443c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443c1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="443c1-110">Permission type</span></span>|<span data-ttu-id="443c1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="443c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="443c1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="443c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="443c1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443c1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="443c1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="443c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="443c1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="443c1-115">Not supported.</span></span>|
|<span data-ttu-id="443c1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="443c1-116">Application</span></span>|<span data-ttu-id="443c1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443c1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="443c1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="443c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="443c1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="443c1-119">Request headers</span></span>
|<span data-ttu-id="443c1-120">标头</span><span class="sxs-lookup"><span data-stu-id="443c1-120">Header</span></span>|<span data-ttu-id="443c1-121">值</span><span class="sxs-lookup"><span data-stu-id="443c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="443c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="443c1-122">Authorization</span></span>|<span data-ttu-id="443c1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="443c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="443c1-124">接受</span><span class="sxs-lookup"><span data-stu-id="443c1-124">Accept</span></span>|<span data-ttu-id="443c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="443c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="443c1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="443c1-126">Request body</span></span>
<span data-ttu-id="443c1-127">在请求正文中, 提供 windows10VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="443c1-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="443c1-128">下表显示创建 windows10VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="443c1-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="443c1-129">属性</span><span class="sxs-lookup"><span data-stu-id="443c1-129">Property</span></span>|<span data-ttu-id="443c1-130">类型</span><span class="sxs-lookup"><span data-stu-id="443c1-130">Type</span></span>|<span data-ttu-id="443c1-131">说明</span><span class="sxs-lookup"><span data-stu-id="443c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="443c1-132">id</span><span class="sxs-lookup"><span data-stu-id="443c1-132">id</span></span>|<span data-ttu-id="443c1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="443c1-133">String</span></span>|<span data-ttu-id="443c1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="443c1-134">Key of the entity.</span></span> <span data-ttu-id="443c1-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="443c1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="443c1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="443c1-137">DateTimeOffset</span></span>|<span data-ttu-id="443c1-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="443c1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="443c1-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="443c1-140">roleScopeTagIds</span></span>|<span data-ttu-id="443c1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="443c1-141">String collection</span></span>|<span data-ttu-id="443c1-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="443c1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="443c1-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="443c1-144">supportsScopeTags</span></span>|<span data-ttu-id="443c1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-145">Boolean</span></span>|<span data-ttu-id="443c1-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="443c1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="443c1-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="443c1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="443c1-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="443c1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="443c1-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="443c1-149">This property is read-only.</span></span> <span data-ttu-id="443c1-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="443c1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="443c1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="443c1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="443c1-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="443c1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="443c1-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="443c1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="443c1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="443c1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="443c1-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="443c1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="443c1-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="443c1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="443c1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="443c1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="443c1-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="443c1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="443c1-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="443c1-163">createdDateTime</span></span>|<span data-ttu-id="443c1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="443c1-164">DateTimeOffset</span></span>|<span data-ttu-id="443c1-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="443c1-165">DateTime the object was created.</span></span> <span data-ttu-id="443c1-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-167">说明</span><span class="sxs-lookup"><span data-stu-id="443c1-167">description</span></span>|<span data-ttu-id="443c1-168">String</span><span class="sxs-lookup"><span data-stu-id="443c1-168">String</span></span>|<span data-ttu-id="443c1-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="443c1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="443c1-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="443c1-171">displayName</span></span>|<span data-ttu-id="443c1-172">String</span><span class="sxs-lookup"><span data-stu-id="443c1-172">String</span></span>|<span data-ttu-id="443c1-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="443c1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="443c1-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-175">version</span><span class="sxs-lookup"><span data-stu-id="443c1-175">version</span></span>|<span data-ttu-id="443c1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="443c1-176">Int32</span></span>|<span data-ttu-id="443c1-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="443c1-177">Version of the device configuration.</span></span> <span data-ttu-id="443c1-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="443c1-179">connectionName</span></span>|<span data-ttu-id="443c1-180">String</span><span class="sxs-lookup"><span data-stu-id="443c1-180">String</span></span>|<span data-ttu-id="443c1-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="443c1-181">Connection name displayed to the user.</span></span> <span data-ttu-id="443c1-182">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-183">台</span><span class="sxs-lookup"><span data-stu-id="443c1-183">servers</span></span>|<span data-ttu-id="443c1-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="443c1-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="443c1-185">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="443c1-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="443c1-186">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="443c1-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="443c1-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="443c1-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="443c1-188">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-189">customXml</span><span class="sxs-lookup"><span data-stu-id="443c1-189">customXml</span></span>|<span data-ttu-id="443c1-190">Binary</span><span class="sxs-lookup"><span data-stu-id="443c1-190">Binary</span></span>|<span data-ttu-id="443c1-191">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="443c1-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="443c1-192">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443c1-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="443c1-193">profileTarget</span><span class="sxs-lookup"><span data-stu-id="443c1-193">profileTarget</span></span>|[<span data-ttu-id="443c1-194">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="443c1-194">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="443c1-195">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="443c1-195">Profile target type.</span></span> <span data-ttu-id="443c1-196">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="443c1-196">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="443c1-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="443c1-197">connectionType</span></span>|[<span data-ttu-id="443c1-198">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="443c1-198">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="443c1-199">连接类型。</span><span class="sxs-lookup"><span data-stu-id="443c1-199">Connection type.</span></span> <span data-ttu-id="443c1-200">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="443c1-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="443c1-201">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="443c1-201">enableSplitTunneling</span></span>|<span data-ttu-id="443c1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-202">Boolean</span></span>|<span data-ttu-id="443c1-203">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="443c1-203">Enable split tunneling.</span></span>|
|<span data-ttu-id="443c1-204">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="443c1-204">enableAlwaysOn</span></span>|<span data-ttu-id="443c1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-205">Boolean</span></span>|<span data-ttu-id="443c1-206">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="443c1-206">Enable Always On mode.</span></span>|
|<span data-ttu-id="443c1-207">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="443c1-207">enableDeviceTunnel</span></span>|<span data-ttu-id="443c1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-208">Boolean</span></span>|<span data-ttu-id="443c1-209">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="443c1-209">Enable device tunnel.</span></span>|
|<span data-ttu-id="443c1-210">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="443c1-210">enableDnsRegistration</span></span>|<span data-ttu-id="443c1-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-211">Boolean</span></span>|<span data-ttu-id="443c1-212">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="443c1-212">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="443c1-213">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="443c1-213">dnsSuffixes</span></span>|<span data-ttu-id="443c1-214">String collection</span><span class="sxs-lookup"><span data-stu-id="443c1-214">String collection</span></span>|<span data-ttu-id="443c1-215">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="443c1-215">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="443c1-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="443c1-216">authenticationMethod</span></span>|[<span data-ttu-id="443c1-217">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="443c1-217">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="443c1-218">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="443c1-218">Authentication method.</span></span> <span data-ttu-id="443c1-219">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="443c1-219">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="443c1-220">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="443c1-220">rememberUserCredentials</span></span>|<span data-ttu-id="443c1-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-221">Boolean</span></span>|<span data-ttu-id="443c1-222">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="443c1-222">Remember user credentials.</span></span>|
|<span data-ttu-id="443c1-223">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="443c1-223">enableConditionalAccess</span></span>|<span data-ttu-id="443c1-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-224">Boolean</span></span>|<span data-ttu-id="443c1-225">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="443c1-225">Enable conditional access.</span></span>|
|<span data-ttu-id="443c1-226">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="443c1-226">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="443c1-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-227">Boolean</span></span>|<span data-ttu-id="443c1-228">启用具有备用证书的单一登录 (SSO)。</span><span class="sxs-lookup"><span data-stu-id="443c1-228">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="443c1-229">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="443c1-229">singleSignOnEku</span></span>|[<span data-ttu-id="443c1-230">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="443c1-230">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="443c1-231">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="443c1-231">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="443c1-232">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="443c1-232">singleSignOnIssuerHash</span></span>|<span data-ttu-id="443c1-233">String</span><span class="sxs-lookup"><span data-stu-id="443c1-233">String</span></span>|<span data-ttu-id="443c1-234">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="443c1-234">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="443c1-235">eapXml</span><span class="sxs-lookup"><span data-stu-id="443c1-235">eapXml</span></span>|<span data-ttu-id="443c1-236">Binary</span><span class="sxs-lookup"><span data-stu-id="443c1-236">Binary</span></span>|<span data-ttu-id="443c1-237">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="443c1-237">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="443c1-238">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="443c1-238">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="443c1-239">proxyServer</span><span class="sxs-lookup"><span data-stu-id="443c1-239">proxyServer</span></span>|[<span data-ttu-id="443c1-240">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="443c1-240">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="443c1-241">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="443c1-241">Proxy Server.</span></span>|
|<span data-ttu-id="443c1-242">associatedApps</span><span class="sxs-lookup"><span data-stu-id="443c1-242">associatedApps</span></span>|<span data-ttu-id="443c1-243">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="443c1-243">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="443c1-244">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="443c1-244">Associated Apps.</span></span> <span data-ttu-id="443c1-245">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="443c1-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="443c1-246">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="443c1-246">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="443c1-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="443c1-247">Boolean</span></span>|<span data-ttu-id="443c1-248">仅关联的应用程序可以使用连接 (每个应用 VPN)。</span><span class="sxs-lookup"><span data-stu-id="443c1-248">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="443c1-249">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="443c1-249">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="443c1-250">String</span><span class="sxs-lookup"><span data-stu-id="443c1-250">String</span></span>|<span data-ttu-id="443c1-251">与此连接关联的 Windows 信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="443c1-251">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="443c1-252">trafficRules</span><span class="sxs-lookup"><span data-stu-id="443c1-252">trafficRules</span></span>|<span data-ttu-id="443c1-253">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="443c1-253">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="443c1-254">流量规则。</span><span class="sxs-lookup"><span data-stu-id="443c1-254">Traffic rules.</span></span> <span data-ttu-id="443c1-255">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="443c1-255">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="443c1-256">航线</span><span class="sxs-lookup"><span data-stu-id="443c1-256">routes</span></span>|<span data-ttu-id="443c1-257">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="443c1-257">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="443c1-258">路由 (可选用于第三方提供程序)。</span><span class="sxs-lookup"><span data-stu-id="443c1-258">Routes (optional for third-party providers).</span></span> <span data-ttu-id="443c1-259">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="443c1-259">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="443c1-260">dnsRules</span><span class="sxs-lookup"><span data-stu-id="443c1-260">dnsRules</span></span>|<span data-ttu-id="443c1-261">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="443c1-261">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="443c1-262">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="443c1-262">DNS rules.</span></span> <span data-ttu-id="443c1-263">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="443c1-263">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="443c1-264">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="443c1-264">trustedNetworkDomains</span></span>|<span data-ttu-id="443c1-265">String collection</span><span class="sxs-lookup"><span data-stu-id="443c1-265">String collection</span></span>|<span data-ttu-id="443c1-266">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="443c1-266">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="443c1-267">响应</span><span class="sxs-lookup"><span data-stu-id="443c1-267">Response</span></span>
<span data-ttu-id="443c1-268">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="443c1-268">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443c1-269">示例</span><span class="sxs-lookup"><span data-stu-id="443c1-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="443c1-270">请求</span><span class="sxs-lookup"><span data-stu-id="443c1-270">Request</span></span>
<span data-ttu-id="443c1-271">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="443c1-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4160

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="443c1-272">响应</span><span class="sxs-lookup"><span data-stu-id="443c1-272">Response</span></span>
<span data-ttu-id="443c1-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="443c1-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4332

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
  ]
}
```






