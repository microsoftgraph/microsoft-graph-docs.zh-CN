---
title: 创建 windows10VpnConfiguration
description: 创建新的 windows10VpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bff78f58039cbe4be3c471d81a783ba6f8fcde01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477698"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="b30ca-103">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b30ca-103">Create windows10VpnConfiguration</span></span>

<span data-ttu-id="b30ca-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b30ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b30ca-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b30ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b30ca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b30ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b30ca-107">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b30ca-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b30ca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b30ca-108">Prerequisites</span></span>
<span data-ttu-id="b30ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b30ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b30ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b30ca-111">Permission type</span></span>|<span data-ttu-id="b30ca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b30ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b30ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b30ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b30ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b30ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b30ca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b30ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b30ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b30ca-116">Not supported.</span></span>|
|<span data-ttu-id="b30ca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b30ca-117">Application</span></span>|<span data-ttu-id="b30ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b30ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b30ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b30ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b30ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b30ca-120">Request headers</span></span>
|<span data-ttu-id="b30ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="b30ca-121">Header</span></span>|<span data-ttu-id="b30ca-122">值</span><span class="sxs-lookup"><span data-stu-id="b30ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b30ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b30ca-123">Authorization</span></span>|<span data-ttu-id="b30ca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b30ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b30ca-125">接受</span><span class="sxs-lookup"><span data-stu-id="b30ca-125">Accept</span></span>|<span data-ttu-id="b30ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b30ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b30ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b30ca-127">Request body</span></span>
<span data-ttu-id="b30ca-128">在请求正文中，提供 windows10VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b30ca-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="b30ca-129">下表显示创建 windows10VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b30ca-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="b30ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="b30ca-130">Property</span></span>|<span data-ttu-id="b30ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="b30ca-131">Type</span></span>|<span data-ttu-id="b30ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="b30ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b30ca-133">id</span><span class="sxs-lookup"><span data-stu-id="b30ca-133">id</span></span>|<span data-ttu-id="b30ca-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b30ca-134">String</span></span>|<span data-ttu-id="b30ca-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b30ca-135">Key of the entity.</span></span> <span data-ttu-id="b30ca-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b30ca-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b30ca-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b30ca-138">DateTimeOffset</span></span>|<span data-ttu-id="b30ca-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b30ca-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b30ca-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b30ca-141">roleScopeTagIds</span></span>|<span data-ttu-id="b30ca-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-142">String collection</span></span>|<span data-ttu-id="b30ca-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b30ca-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b30ca-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b30ca-145">supportsScopeTags</span></span>|<span data-ttu-id="b30ca-146">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-146">Boolean</span></span>|<span data-ttu-id="b30ca-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b30ca-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b30ca-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b30ca-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b30ca-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b30ca-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b30ca-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b30ca-150">This property is read-only.</span></span> <span data-ttu-id="b30ca-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b30ca-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b30ca-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b30ca-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b30ca-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b30ca-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b30ca-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b30ca-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b30ca-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b30ca-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b30ca-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b30ca-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b30ca-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b30ca-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b30ca-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b30ca-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b30ca-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b30ca-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b30ca-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b30ca-164">createdDateTime</span></span>|<span data-ttu-id="b30ca-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b30ca-165">DateTimeOffset</span></span>|<span data-ttu-id="b30ca-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b30ca-166">DateTime the object was created.</span></span> <span data-ttu-id="b30ca-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-168">说明</span><span class="sxs-lookup"><span data-stu-id="b30ca-168">description</span></span>|<span data-ttu-id="b30ca-169">String</span><span class="sxs-lookup"><span data-stu-id="b30ca-169">String</span></span>|<span data-ttu-id="b30ca-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b30ca-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b30ca-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b30ca-172">displayName</span></span>|<span data-ttu-id="b30ca-173">String</span><span class="sxs-lookup"><span data-stu-id="b30ca-173">String</span></span>|<span data-ttu-id="b30ca-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b30ca-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b30ca-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-176">version</span><span class="sxs-lookup"><span data-stu-id="b30ca-176">version</span></span>|<span data-ttu-id="b30ca-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b30ca-177">Int32</span></span>|<span data-ttu-id="b30ca-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b30ca-178">Version of the device configuration.</span></span> <span data-ttu-id="b30ca-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="b30ca-180">connectionName</span></span>|<span data-ttu-id="b30ca-181">String</span><span class="sxs-lookup"><span data-stu-id="b30ca-181">String</span></span>|<span data-ttu-id="b30ca-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="b30ca-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b30ca-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-184">台</span><span class="sxs-lookup"><span data-stu-id="b30ca-184">servers</span></span>|<span data-ttu-id="b30ca-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b30ca-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="b30ca-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="b30ca-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="b30ca-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b30ca-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b30ca-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b30ca-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-190">customXml</span><span class="sxs-lookup"><span data-stu-id="b30ca-190">customXml</span></span>|<span data-ttu-id="b30ca-191">Binary</span><span class="sxs-lookup"><span data-stu-id="b30ca-191">Binary</span></span>|<span data-ttu-id="b30ca-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="b30ca-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b30ca-193">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b30ca-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b30ca-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="b30ca-194">profileTarget</span></span>|[<span data-ttu-id="b30ca-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="b30ca-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="b30ca-196">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="b30ca-196">Profile target type.</span></span> <span data-ttu-id="b30ca-197">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="b30ca-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="b30ca-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="b30ca-198">connectionType</span></span>|[<span data-ttu-id="b30ca-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b30ca-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="b30ca-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="b30ca-200">Connection type.</span></span> <span data-ttu-id="b30ca-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="b30ca-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="b30ca-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b30ca-202">enableSplitTunneling</span></span>|<span data-ttu-id="b30ca-203">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-203">Boolean</span></span>|<span data-ttu-id="b30ca-204">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="b30ca-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="b30ca-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="b30ca-205">enableAlwaysOn</span></span>|<span data-ttu-id="b30ca-206">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-206">Boolean</span></span>|<span data-ttu-id="b30ca-207">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="b30ca-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="b30ca-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="b30ca-208">enableDeviceTunnel</span></span>|<span data-ttu-id="b30ca-209">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-209">Boolean</span></span>|<span data-ttu-id="b30ca-210">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="b30ca-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="b30ca-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="b30ca-211">enableDnsRegistration</span></span>|<span data-ttu-id="b30ca-212">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-212">Boolean</span></span>|<span data-ttu-id="b30ca-213">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="b30ca-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="b30ca-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="b30ca-214">dnsSuffixes</span></span>|<span data-ttu-id="b30ca-215">String 集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-215">String collection</span></span>|<span data-ttu-id="b30ca-216">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="b30ca-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="b30ca-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b30ca-217">authenticationMethod</span></span>|[<span data-ttu-id="b30ca-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b30ca-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="b30ca-219">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b30ca-219">Authentication method.</span></span> <span data-ttu-id="b30ca-220">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="b30ca-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="b30ca-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="b30ca-221">rememberUserCredentials</span></span>|<span data-ttu-id="b30ca-222">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-222">Boolean</span></span>|<span data-ttu-id="b30ca-223">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="b30ca-223">Remember user credentials.</span></span>|
|<span data-ttu-id="b30ca-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b30ca-224">enableConditionalAccess</span></span>|<span data-ttu-id="b30ca-225">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-225">Boolean</span></span>|<span data-ttu-id="b30ca-226">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="b30ca-226">Enable conditional access.</span></span>|
|<span data-ttu-id="b30ca-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="b30ca-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="b30ca-228">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-228">Boolean</span></span>|<span data-ttu-id="b30ca-229">启用具有备用证书的单一登录（SSO）。</span><span class="sxs-lookup"><span data-stu-id="b30ca-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="b30ca-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="b30ca-230">singleSignOnEku</span></span>|[<span data-ttu-id="b30ca-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="b30ca-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="b30ca-232">单一登录扩展密钥用法（EKU）。</span><span class="sxs-lookup"><span data-stu-id="b30ca-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="b30ca-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="b30ca-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="b30ca-234">String</span><span class="sxs-lookup"><span data-stu-id="b30ca-234">String</span></span>|<span data-ttu-id="b30ca-235">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="b30ca-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="b30ca-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="b30ca-236">eapXml</span></span>|<span data-ttu-id="b30ca-237">Binary</span><span class="sxs-lookup"><span data-stu-id="b30ca-237">Binary</span></span>|<span data-ttu-id="b30ca-238">可扩展的身份验证协议（EAP） XML。</span><span class="sxs-lookup"><span data-stu-id="b30ca-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="b30ca-239">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="b30ca-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="b30ca-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b30ca-240">proxyServer</span></span>|[<span data-ttu-id="b30ca-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b30ca-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="b30ca-242">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="b30ca-242">Proxy Server.</span></span>|
|<span data-ttu-id="b30ca-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="b30ca-243">associatedApps</span></span>|<span data-ttu-id="b30ca-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="b30ca-245">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="b30ca-245">Associated Apps.</span></span> <span data-ttu-id="b30ca-246">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b30ca-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b30ca-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="b30ca-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="b30ca-248">布尔</span><span class="sxs-lookup"><span data-stu-id="b30ca-248">Boolean</span></span>|<span data-ttu-id="b30ca-249">仅关联的应用程序可以使用连接（每个应用 VPN）。</span><span class="sxs-lookup"><span data-stu-id="b30ca-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="b30ca-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="b30ca-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="b30ca-251">String</span><span class="sxs-lookup"><span data-stu-id="b30ca-251">String</span></span>|<span data-ttu-id="b30ca-252">与此连接关联的 Windows 信息保护（WIP）域。</span><span class="sxs-lookup"><span data-stu-id="b30ca-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="b30ca-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="b30ca-253">trafficRules</span></span>|<span data-ttu-id="b30ca-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="b30ca-255">流量规则。</span><span class="sxs-lookup"><span data-stu-id="b30ca-255">Traffic rules.</span></span> <span data-ttu-id="b30ca-256">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b30ca-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b30ca-257">航线</span><span class="sxs-lookup"><span data-stu-id="b30ca-257">routes</span></span>|<span data-ttu-id="b30ca-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="b30ca-259">路由（可选用于第三方提供程序）。</span><span class="sxs-lookup"><span data-stu-id="b30ca-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="b30ca-260">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b30ca-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b30ca-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="b30ca-261">dnsRules</span></span>|<span data-ttu-id="b30ca-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="b30ca-263">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="b30ca-263">DNS rules.</span></span> <span data-ttu-id="b30ca-264">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b30ca-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b30ca-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="b30ca-265">trustedNetworkDomains</span></span>|<span data-ttu-id="b30ca-266">String 集合</span><span class="sxs-lookup"><span data-stu-id="b30ca-266">String collection</span></span>|<span data-ttu-id="b30ca-267">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="b30ca-267">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="b30ca-268">响应</span><span class="sxs-lookup"><span data-stu-id="b30ca-268">Response</span></span>
<span data-ttu-id="b30ca-269">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b30ca-269">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b30ca-270">示例</span><span class="sxs-lookup"><span data-stu-id="b30ca-270">Example</span></span>

### <a name="request"></a><span data-ttu-id="b30ca-271">请求</span><span class="sxs-lookup"><span data-stu-id="b30ca-271">Request</span></span>
<span data-ttu-id="b30ca-272">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b30ca-272">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b30ca-273">响应</span><span class="sxs-lookup"><span data-stu-id="b30ca-273">Response</span></span>
<span data-ttu-id="b30ca-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b30ca-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





