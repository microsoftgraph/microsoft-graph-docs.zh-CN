---
title: 更新 windowsPhone81VpnConfiguration
description: 更新 windowsPhone81VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32729154f29a784d61fa61267fd8855207a64e75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972376"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="ef9ae-103">更新 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef9ae-103">Update windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="ef9ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef9ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef9ae-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef9ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef9ae-107">更新 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef9ae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef9ae-108">Prerequisites</span></span>
<span data-ttu-id="ef9ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef9ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef9ae-111">Permission type</span></span>|<span data-ttu-id="ef9ae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef9ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef9ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef9ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef9ae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef9ae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef9ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef9ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef9ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-116">Not supported.</span></span>|
|<span data-ttu-id="ef9ae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef9ae-117">Application</span></span>|<span data-ttu-id="ef9ae-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef9ae-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef9ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef9ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef9ae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef9ae-120">Request headers</span></span>
|<span data-ttu-id="ef9ae-121">标头</span><span class="sxs-lookup"><span data-stu-id="ef9ae-121">Header</span></span>|<span data-ttu-id="ef9ae-122">值</span><span class="sxs-lookup"><span data-stu-id="ef9ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef9ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef9ae-123">Authorization</span></span>|<span data-ttu-id="ef9ae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef9ae-125">接受</span><span class="sxs-lookup"><span data-stu-id="ef9ae-125">Accept</span></span>|<span data-ttu-id="ef9ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef9ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef9ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef9ae-127">Request body</span></span>
<span data-ttu-id="ef9ae-128">在请求正文中，提供 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="ef9ae-129">下表显示创建 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="ef9ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="ef9ae-130">Property</span></span>|<span data-ttu-id="ef9ae-131">类型</span><span class="sxs-lookup"><span data-stu-id="ef9ae-131">Type</span></span>|<span data-ttu-id="ef9ae-132">说明</span><span class="sxs-lookup"><span data-stu-id="ef9ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef9ae-133">id</span><span class="sxs-lookup"><span data-stu-id="ef9ae-133">id</span></span>|<span data-ttu-id="ef9ae-134">String</span><span class="sxs-lookup"><span data-stu-id="ef9ae-134">String</span></span>|<span data-ttu-id="ef9ae-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-135">Key of the entity.</span></span> <span data-ttu-id="ef9ae-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef9ae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ef9ae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef9ae-138">DateTimeOffset</span></span>|<span data-ttu-id="ef9ae-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ef9ae-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef9ae-141">roleScopeTagIds</span></span>|<span data-ttu-id="ef9ae-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ef9ae-142">String collection</span></span>|<span data-ttu-id="ef9ae-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef9ae-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef9ae-145">supportsScopeTags</span></span>|<span data-ttu-id="ef9ae-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9ae-146">Boolean</span></span>|<span data-ttu-id="ef9ae-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef9ae-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef9ae-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef9ae-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-150">This property is read-only.</span></span> <span data-ttu-id="ef9ae-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef9ae-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ef9ae-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef9ae-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ef9ae-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ef9ae-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef9ae-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ef9ae-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef9ae-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ef9ae-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ef9ae-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef9ae-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ef9ae-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef9ae-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ef9ae-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ef9ae-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef9ae-164">createdDateTime</span></span>|<span data-ttu-id="ef9ae-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef9ae-165">DateTimeOffset</span></span>|<span data-ttu-id="ef9ae-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-166">DateTime the object was created.</span></span> <span data-ttu-id="ef9ae-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-168">description</span><span class="sxs-lookup"><span data-stu-id="ef9ae-168">description</span></span>|<span data-ttu-id="ef9ae-169">String</span><span class="sxs-lookup"><span data-stu-id="ef9ae-169">String</span></span>|<span data-ttu-id="ef9ae-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef9ae-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ef9ae-172">displayName</span></span>|<span data-ttu-id="ef9ae-173">String</span><span class="sxs-lookup"><span data-stu-id="ef9ae-173">String</span></span>|<span data-ttu-id="ef9ae-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef9ae-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-176">version</span><span class="sxs-lookup"><span data-stu-id="ef9ae-176">version</span></span>|<span data-ttu-id="ef9ae-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9ae-177">Int32</span></span>|<span data-ttu-id="ef9ae-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-178">Version of the device configuration.</span></span> <span data-ttu-id="ef9ae-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="ef9ae-180">connectionName</span></span>|<span data-ttu-id="ef9ae-181">String</span><span class="sxs-lookup"><span data-stu-id="ef9ae-181">String</span></span>|<span data-ttu-id="ef9ae-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-182">Connection name displayed to the user.</span></span> <span data-ttu-id="ef9ae-183">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-184">台</span><span class="sxs-lookup"><span data-stu-id="ef9ae-184">servers</span></span>|<span data-ttu-id="ef9ae-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef9ae-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ef9ae-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="ef9ae-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ef9ae-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ef9ae-189">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-190">customXml</span><span class="sxs-lookup"><span data-stu-id="ef9ae-190">customXml</span></span>|<span data-ttu-id="ef9ae-191">Binary</span><span class="sxs-lookup"><span data-stu-id="ef9ae-191">Binary</span></span>|<span data-ttu-id="ef9ae-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="ef9ae-193">从[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)继承的 (UTF8 编码的字节数组) </span><span class="sxs-lookup"><span data-stu-id="ef9ae-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ef9ae-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="ef9ae-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9ae-195">Boolean</span></span>|<span data-ttu-id="ef9ae-196">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ef9ae-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-197">This property is read-only.</span></span> <span data-ttu-id="ef9ae-198">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="ef9ae-199">connectionType</span></span>|[<span data-ttu-id="ef9ae-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ef9ae-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="ef9ae-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-201">Connection type.</span></span> <span data-ttu-id="ef9ae-202">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="ef9ae-203">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="ef9ae-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ef9ae-204">loginGroupOrDomain</span></span>|<span data-ttu-id="ef9ae-205">String</span><span class="sxs-lookup"><span data-stu-id="ef9ae-205">String</span></span>|<span data-ttu-id="ef9ae-206">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ef9ae-207">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ef9ae-208">enableSplitTunneling</span></span>|<span data-ttu-id="ef9ae-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9ae-209">Boolean</span></span>|<span data-ttu-id="ef9ae-210">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="ef9ae-211">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ef9ae-212">proxyServer</span></span>|[<span data-ttu-id="ef9ae-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ef9ae-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="ef9ae-214">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-214">Proxy Server.</span></span> <span data-ttu-id="ef9ae-215">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9ae-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9ae-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="ef9ae-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="ef9ae-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9ae-217">Boolean</span></span>|<span data-ttu-id="ef9ae-218">在公司 Wi-fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="ef9ae-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="ef9ae-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="ef9ae-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9ae-220">Boolean</span></span>|<span data-ttu-id="ef9ae-221">绕过家庭 Wi-fi 上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="ef9ae-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef9ae-222">authenticationMethod</span></span>|[<span data-ttu-id="ef9ae-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef9ae-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ef9ae-224">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-224">Authentication method.</span></span> <span data-ttu-id="ef9ae-225">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ef9ae-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="ef9ae-226">rememberUserCredentials</span></span>|<span data-ttu-id="ef9ae-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9ae-227">Boolean</span></span>|<span data-ttu-id="ef9ae-228">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-228">Remember user credentials.</span></span>|
|<span data-ttu-id="ef9ae-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="ef9ae-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="ef9ae-230">String collection</span><span class="sxs-lookup"><span data-stu-id="ef9ae-230">String collection</span></span>|<span data-ttu-id="ef9ae-231">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="ef9ae-232">响应</span><span class="sxs-lookup"><span data-stu-id="ef9ae-232">Response</span></span>
<span data-ttu-id="ef9ae-233">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef9ae-234">示例</span><span class="sxs-lookup"><span data-stu-id="ef9ae-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef9ae-235">请求</span><span class="sxs-lookup"><span data-stu-id="ef9ae-235">Request</span></span>
<span data-ttu-id="ef9ae-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ef9ae-237">响应</span><span class="sxs-lookup"><span data-stu-id="ef9ae-237">Response</span></span>
<span data-ttu-id="ef9ae-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef9ae-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```






