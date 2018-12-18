---
title: 创建 windows10VpnConfiguration
description: 创建新的 windows10VpnConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 02cbb520f32e26a3f4303521491031b0d3aeb090
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308839"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="6c923-103">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c923-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="6c923-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c923-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c923-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c923-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c923-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c923-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c923-107">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c923-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c923-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c923-108">Prerequisites</span></span>
<span data-ttu-id="6c923-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6c923-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c923-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c923-111">Permission type</span></span>|<span data-ttu-id="6c923-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c923-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c923-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c923-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c923-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c923-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c923-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c923-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c923-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c923-116">Not supported.</span></span>|
|<span data-ttu-id="6c923-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c923-117">Application</span></span>|<span data-ttu-id="6c923-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c923-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c923-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c923-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c923-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c923-120">Request headers</span></span>
|<span data-ttu-id="6c923-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c923-121">Header</span></span>|<span data-ttu-id="6c923-122">值</span><span class="sxs-lookup"><span data-stu-id="6c923-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c923-123">授权</span><span class="sxs-lookup"><span data-stu-id="6c923-123">Authorization</span></span>|<span data-ttu-id="6c923-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c923-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c923-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c923-125">Accept</span></span>|<span data-ttu-id="6c923-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c923-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c923-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c923-127">Request body</span></span>
<span data-ttu-id="6c923-128">在请求正文中，提供 windows10VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c923-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="6c923-129">下表显示时创建 windows10VpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6c923-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="6c923-130">属性</span><span class="sxs-lookup"><span data-stu-id="6c923-130">Property</span></span>|<span data-ttu-id="6c923-131">类型</span><span class="sxs-lookup"><span data-stu-id="6c923-131">Type</span></span>|<span data-ttu-id="6c923-132">说明</span><span class="sxs-lookup"><span data-stu-id="6c923-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c923-133">id</span><span class="sxs-lookup"><span data-stu-id="6c923-133">id</span></span>|<span data-ttu-id="6c923-134">String</span><span class="sxs-lookup"><span data-stu-id="6c923-134">String</span></span>|<span data-ttu-id="6c923-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c923-135">Key of the entity.</span></span> <span data-ttu-id="6c923-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c923-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6c923-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c923-138">DateTimeOffset</span></span>|<span data-ttu-id="6c923-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c923-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6c923-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c923-141">roleScopeTagIds</span></span>|<span data-ttu-id="6c923-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6c923-142">String collection</span></span>|<span data-ttu-id="6c923-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6c923-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c923-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c923-145">supportsScopeTags</span></span>|<span data-ttu-id="6c923-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-146">Boolean</span></span>|<span data-ttu-id="6c923-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6c923-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c923-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6c923-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c923-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6c923-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c923-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6c923-150">This property is read-only.</span></span> <span data-ttu-id="6c923-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c923-152">createdDateTime</span></span>|<span data-ttu-id="6c923-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c923-153">DateTimeOffset</span></span>|<span data-ttu-id="6c923-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c923-154">DateTime the object was created.</span></span> <span data-ttu-id="6c923-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-156">description</span><span class="sxs-lookup"><span data-stu-id="6c923-156">description</span></span>|<span data-ttu-id="6c923-157">String</span><span class="sxs-lookup"><span data-stu-id="6c923-157">String</span></span>|<span data-ttu-id="6c923-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6c923-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c923-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6c923-160">displayName</span></span>|<span data-ttu-id="6c923-161">String</span><span class="sxs-lookup"><span data-stu-id="6c923-161">String</span></span>|<span data-ttu-id="6c923-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6c923-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c923-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-164">version</span><span class="sxs-lookup"><span data-stu-id="6c923-164">version</span></span>|<span data-ttu-id="6c923-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6c923-165">Int32</span></span>|<span data-ttu-id="6c923-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6c923-166">Version of the device configuration.</span></span> <span data-ttu-id="6c923-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="6c923-168">connectionName</span></span>|<span data-ttu-id="6c923-169">字符串</span><span class="sxs-lookup"><span data-stu-id="6c923-169">String</span></span>|<span data-ttu-id="6c923-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="6c923-170">Connection name displayed to the user.</span></span> <span data-ttu-id="6c923-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-172">服务器</span><span class="sxs-lookup"><span data-stu-id="6c923-172">servers</span></span>|<span data-ttu-id="6c923-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c923-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6c923-174">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="6c923-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="6c923-175">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="6c923-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6c923-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c923-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6c923-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-178">customXml</span><span class="sxs-lookup"><span data-stu-id="6c923-178">customXml</span></span>|<span data-ttu-id="6c923-179">Binary</span><span class="sxs-lookup"><span data-stu-id="6c923-179">Binary</span></span>|<span data-ttu-id="6c923-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="6c923-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6c923-181">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c923-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6c923-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="6c923-182">profileTarget</span></span>|[<span data-ttu-id="6c923-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="6c923-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="6c923-184">配置文件的目标类型。</span><span class="sxs-lookup"><span data-stu-id="6c923-184">Profile target type.</span></span> <span data-ttu-id="6c923-185">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="6c923-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="6c923-186">连接</span><span class="sxs-lookup"><span data-stu-id="6c923-186">connectionType</span></span>|[<span data-ttu-id="6c923-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6c923-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="6c923-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="6c923-188">Connection type.</span></span> <span data-ttu-id="6c923-189">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="6c923-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="6c923-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6c923-190">enableSplitTunneling</span></span>|<span data-ttu-id="6c923-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-191">Boolean</span></span>|<span data-ttu-id="6c923-192">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="6c923-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="6c923-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="6c923-193">enableAlwaysOn</span></span>|<span data-ttu-id="6c923-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-194">Boolean</span></span>|<span data-ttu-id="6c923-195">启用 Always On 模式。</span><span class="sxs-lookup"><span data-stu-id="6c923-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="6c923-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="6c923-196">enableDeviceTunnel</span></span>|<span data-ttu-id="6c923-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-197">Boolean</span></span>|<span data-ttu-id="6c923-198">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="6c923-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="6c923-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="6c923-199">enableDnsRegistration</span></span>|<span data-ttu-id="6c923-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-200">Boolean</span></span>|<span data-ttu-id="6c923-201">启用内部 DNS 注册的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="6c923-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="6c923-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="6c923-202">dnsSuffixes</span></span>|<span data-ttu-id="6c923-203">String 集合</span><span class="sxs-lookup"><span data-stu-id="6c923-203">String collection</span></span>|<span data-ttu-id="6c923-204">指定要向 DNS 搜索列表正确路由短名称添加 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="6c923-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="6c923-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c923-205">authenticationMethod</span></span>|[<span data-ttu-id="6c923-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c923-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="6c923-207">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6c923-207">Authentication method.</span></span> <span data-ttu-id="6c923-208">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="6c923-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="6c923-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="6c923-209">rememberUserCredentials</span></span>|<span data-ttu-id="6c923-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-210">Boolean</span></span>|<span data-ttu-id="6c923-211">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="6c923-211">Remember user credentials.</span></span>|
|<span data-ttu-id="6c923-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6c923-212">enableConditionalAccess</span></span>|<span data-ttu-id="6c923-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-213">Boolean</span></span>|<span data-ttu-id="6c923-214">启用条件的访问。</span><span class="sxs-lookup"><span data-stu-id="6c923-214">Enable conditional access.</span></span>|
|<span data-ttu-id="6c923-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="6c923-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="6c923-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-216">Boolean</span></span>|<span data-ttu-id="6c923-217">启用单一登录 (SSO) 与备用证书。</span><span class="sxs-lookup"><span data-stu-id="6c923-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="6c923-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="6c923-218">singleSignOnEku</span></span>|[<span data-ttu-id="6c923-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6c923-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="6c923-220">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="6c923-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="6c923-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="6c923-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="6c923-222">字符串</span><span class="sxs-lookup"><span data-stu-id="6c923-222">String</span></span>|<span data-ttu-id="6c923-223">单一登录颁发者哈希值。</span><span class="sxs-lookup"><span data-stu-id="6c923-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="6c923-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="6c923-224">eapXml</span></span>|<span data-ttu-id="6c923-225">Binary</span><span class="sxs-lookup"><span data-stu-id="6c923-225">Binary</span></span>|<span data-ttu-id="6c923-226">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="6c923-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="6c923-227">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="6c923-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6c923-228">代理服务器</span><span class="sxs-lookup"><span data-stu-id="6c923-228">proxyServer</span></span>|[<span data-ttu-id="6c923-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6c923-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="6c923-230">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="6c923-230">Proxy Server.</span></span>|
|<span data-ttu-id="6c923-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="6c923-231">associatedApps</span></span>|<span data-ttu-id="6c923-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c923-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="6c923-233">关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6c923-233">Associated Apps.</span></span> <span data-ttu-id="6c923-234">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c923-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6c923-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="6c923-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="6c923-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c923-236">Boolean</span></span>|<span data-ttu-id="6c923-237">仅关联的应用程序可以使用 (每个应用程序 VPN) 连接。</span><span class="sxs-lookup"><span data-stu-id="6c923-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="6c923-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="6c923-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="6c923-239">字符串</span><span class="sxs-lookup"><span data-stu-id="6c923-239">String</span></span>|<span data-ttu-id="6c923-240">要与此连接关联的 Windows 的信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="6c923-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="6c923-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="6c923-241">trafficRules</span></span>|<span data-ttu-id="6c923-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c923-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="6c923-243">流量的规则。</span><span class="sxs-lookup"><span data-stu-id="6c923-243">Traffic rules.</span></span> <span data-ttu-id="6c923-244">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c923-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6c923-245">路由</span><span class="sxs-lookup"><span data-stu-id="6c923-245">routes</span></span>|<span data-ttu-id="6c923-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c923-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="6c923-247">（可选第三方提供程序） 的路由。</span><span class="sxs-lookup"><span data-stu-id="6c923-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="6c923-248">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c923-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6c923-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="6c923-249">dnsRules</span></span>|<span data-ttu-id="6c923-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c923-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="6c923-251">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="6c923-251">DNS rules.</span></span> <span data-ttu-id="6c923-252">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c923-252">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6c923-253">响应</span><span class="sxs-lookup"><span data-stu-id="6c923-253">Response</span></span>
<span data-ttu-id="6c923-254">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c923-254">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c923-255">示例</span><span class="sxs-lookup"><span data-stu-id="6c923-255">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c923-256">请求</span><span class="sxs-lookup"><span data-stu-id="6c923-256">Request</span></span>
<span data-ttu-id="6c923-257">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c923-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3323

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6c923-258">响应</span><span class="sxs-lookup"><span data-stu-id="6c923-258">Response</span></span>
<span data-ttu-id="6c923-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c923-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3431

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```





