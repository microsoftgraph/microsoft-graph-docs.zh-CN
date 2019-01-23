---
title: 创建 windows10VpnConfiguration
description: 创建新的 windows10VpnConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 72264db454928358068f31dc5a439a5e74ce1da6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412042"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="bd5fc-103">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5fc-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="bd5fc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd5fc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd5fc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd5fc-107">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd5fc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd5fc-108">Prerequisites</span></span>
<span data-ttu-id="bd5fc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd5fc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd5fc-111">Permission type</span></span>|<span data-ttu-id="bd5fc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd5fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd5fc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd5fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd5fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd5fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd5fc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd5fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd5fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-116">Not supported.</span></span>|
|<span data-ttu-id="bd5fc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd5fc-117">Application</span></span>|<span data-ttu-id="bd5fc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd5fc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd5fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd5fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd5fc-120">Request headers</span></span>
|<span data-ttu-id="bd5fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd5fc-121">Header</span></span>|<span data-ttu-id="bd5fc-122">值</span><span class="sxs-lookup"><span data-stu-id="bd5fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd5fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd5fc-123">Authorization</span></span>|<span data-ttu-id="bd5fc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd5fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd5fc-125">Accept</span></span>|<span data-ttu-id="bd5fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd5fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd5fc-127">Request body</span></span>
<span data-ttu-id="bd5fc-128">在请求正文中，提供 windows10VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="bd5fc-129">下表显示时创建 windows10VpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="bd5fc-130">属性</span><span class="sxs-lookup"><span data-stu-id="bd5fc-130">Property</span></span>|<span data-ttu-id="bd5fc-131">类型</span><span class="sxs-lookup"><span data-stu-id="bd5fc-131">Type</span></span>|<span data-ttu-id="bd5fc-132">说明</span><span class="sxs-lookup"><span data-stu-id="bd5fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd5fc-133">id</span><span class="sxs-lookup"><span data-stu-id="bd5fc-133">id</span></span>|<span data-ttu-id="bd5fc-134">String</span><span class="sxs-lookup"><span data-stu-id="bd5fc-134">String</span></span>|<span data-ttu-id="bd5fc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-135">Key of the entity.</span></span> <span data-ttu-id="bd5fc-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5fc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bd5fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5fc-138">DateTimeOffset</span></span>|<span data-ttu-id="bd5fc-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bd5fc-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd5fc-141">roleScopeTagIds</span></span>|<span data-ttu-id="bd5fc-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-142">String collection</span></span>|<span data-ttu-id="bd5fc-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd5fc-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bd5fc-145">supportsScopeTags</span></span>|<span data-ttu-id="bd5fc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-146">Boolean</span></span>|<span data-ttu-id="bd5fc-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bd5fc-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bd5fc-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bd5fc-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-150">This property is read-only.</span></span> <span data-ttu-id="bd5fc-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5fc-152">createdDateTime</span></span>|<span data-ttu-id="bd5fc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5fc-153">DateTimeOffset</span></span>|<span data-ttu-id="bd5fc-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-154">DateTime the object was created.</span></span> <span data-ttu-id="bd5fc-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-156">description</span><span class="sxs-lookup"><span data-stu-id="bd5fc-156">description</span></span>|<span data-ttu-id="bd5fc-157">String</span><span class="sxs-lookup"><span data-stu-id="bd5fc-157">String</span></span>|<span data-ttu-id="bd5fc-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd5fc-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bd5fc-160">displayName</span></span>|<span data-ttu-id="bd5fc-161">String</span><span class="sxs-lookup"><span data-stu-id="bd5fc-161">String</span></span>|<span data-ttu-id="bd5fc-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd5fc-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-164">version</span><span class="sxs-lookup"><span data-stu-id="bd5fc-164">version</span></span>|<span data-ttu-id="bd5fc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5fc-165">Int32</span></span>|<span data-ttu-id="bd5fc-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-166">Version of the device configuration.</span></span> <span data-ttu-id="bd5fc-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="bd5fc-168">connectionName</span></span>|<span data-ttu-id="bd5fc-169">String</span><span class="sxs-lookup"><span data-stu-id="bd5fc-169">String</span></span>|<span data-ttu-id="bd5fc-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-170">Connection name displayed to the user.</span></span> <span data-ttu-id="bd5fc-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-172">服务器</span><span class="sxs-lookup"><span data-stu-id="bd5fc-172">servers</span></span>|<span data-ttu-id="bd5fc-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="bd5fc-174">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="bd5fc-175">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="bd5fc-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bd5fc-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-178">customXml</span><span class="sxs-lookup"><span data-stu-id="bd5fc-178">customXml</span></span>|<span data-ttu-id="bd5fc-179">Binary</span><span class="sxs-lookup"><span data-stu-id="bd5fc-179">Binary</span></span>|<span data-ttu-id="bd5fc-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="bd5fc-181">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5fc-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="bd5fc-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="bd5fc-182">profileTarget</span></span>|[<span data-ttu-id="bd5fc-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="bd5fc-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="bd5fc-184">配置文件的目标类型。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-184">Profile target type.</span></span> <span data-ttu-id="bd5fc-185">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="bd5fc-186">连接</span><span class="sxs-lookup"><span data-stu-id="bd5fc-186">connectionType</span></span>|[<span data-ttu-id="bd5fc-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="bd5fc-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="bd5fc-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-188">Connection type.</span></span> <span data-ttu-id="bd5fc-189">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="bd5fc-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="bd5fc-190">enableSplitTunneling</span></span>|<span data-ttu-id="bd5fc-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-191">Boolean</span></span>|<span data-ttu-id="bd5fc-192">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="bd5fc-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="bd5fc-193">enableAlwaysOn</span></span>|<span data-ttu-id="bd5fc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-194">Boolean</span></span>|<span data-ttu-id="bd5fc-195">启用 Always On 模式。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="bd5fc-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="bd5fc-196">enableDeviceTunnel</span></span>|<span data-ttu-id="bd5fc-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-197">Boolean</span></span>|<span data-ttu-id="bd5fc-198">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="bd5fc-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="bd5fc-199">enableDnsRegistration</span></span>|<span data-ttu-id="bd5fc-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-200">Boolean</span></span>|<span data-ttu-id="bd5fc-201">启用内部 DNS 注册的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="bd5fc-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="bd5fc-202">dnsSuffixes</span></span>|<span data-ttu-id="bd5fc-203">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-203">String collection</span></span>|<span data-ttu-id="bd5fc-204">指定要向 DNS 搜索列表正确路由短名称添加 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="bd5fc-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bd5fc-205">authenticationMethod</span></span>|[<span data-ttu-id="bd5fc-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bd5fc-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="bd5fc-207">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-207">Authentication method.</span></span> <span data-ttu-id="bd5fc-208">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="bd5fc-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="bd5fc-209">rememberUserCredentials</span></span>|<span data-ttu-id="bd5fc-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-210">Boolean</span></span>|<span data-ttu-id="bd5fc-211">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-211">Remember user credentials.</span></span>|
|<span data-ttu-id="bd5fc-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="bd5fc-212">enableConditionalAccess</span></span>|<span data-ttu-id="bd5fc-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-213">Boolean</span></span>|<span data-ttu-id="bd5fc-214">启用条件的访问。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-214">Enable conditional access.</span></span>|
|<span data-ttu-id="bd5fc-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="bd5fc-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="bd5fc-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-216">Boolean</span></span>|<span data-ttu-id="bd5fc-217">启用单一登录 (SSO) 与备用证书。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="bd5fc-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="bd5fc-218">singleSignOnEku</span></span>|[<span data-ttu-id="bd5fc-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="bd5fc-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="bd5fc-220">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="bd5fc-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="bd5fc-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="bd5fc-222">String</span><span class="sxs-lookup"><span data-stu-id="bd5fc-222">String</span></span>|<span data-ttu-id="bd5fc-223">单一登录颁发者哈希值。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="bd5fc-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="bd5fc-224">eapXml</span></span>|<span data-ttu-id="bd5fc-225">Binary</span><span class="sxs-lookup"><span data-stu-id="bd5fc-225">Binary</span></span>|<span data-ttu-id="bd5fc-226">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="bd5fc-227">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="bd5fc-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="bd5fc-228">代理服务器</span><span class="sxs-lookup"><span data-stu-id="bd5fc-228">proxyServer</span></span>|[<span data-ttu-id="bd5fc-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="bd5fc-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="bd5fc-230">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-230">Proxy Server.</span></span>|
|<span data-ttu-id="bd5fc-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="bd5fc-231">associatedApps</span></span>|<span data-ttu-id="bd5fc-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="bd5fc-233">关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-233">Associated Apps.</span></span> <span data-ttu-id="bd5fc-234">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bd5fc-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="bd5fc-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="bd5fc-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fc-236">Boolean</span></span>|<span data-ttu-id="bd5fc-237">仅关联的应用程序可以使用 (每个应用程序 VPN) 连接。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="bd5fc-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="bd5fc-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="bd5fc-239">String</span><span class="sxs-lookup"><span data-stu-id="bd5fc-239">String</span></span>|<span data-ttu-id="bd5fc-240">要与此连接关联的 Windows 的信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="bd5fc-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="bd5fc-241">trafficRules</span></span>|<span data-ttu-id="bd5fc-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="bd5fc-243">流量的规则。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-243">Traffic rules.</span></span> <span data-ttu-id="bd5fc-244">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="bd5fc-245">路由</span><span class="sxs-lookup"><span data-stu-id="bd5fc-245">routes</span></span>|<span data-ttu-id="bd5fc-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="bd5fc-247">（可选第三方提供程序） 的路由。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="bd5fc-248">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="bd5fc-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="bd5fc-249">dnsRules</span></span>|<span data-ttu-id="bd5fc-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="bd5fc-251">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-251">DNS rules.</span></span> <span data-ttu-id="bd5fc-252">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="bd5fc-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="bd5fc-253">trustedNetworkDomains</span></span>|<span data-ttu-id="bd5fc-254">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd5fc-254">String collection</span></span>|<span data-ttu-id="bd5fc-255">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="bd5fc-255">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="bd5fc-256">响应</span><span class="sxs-lookup"><span data-stu-id="bd5fc-256">Response</span></span>
<span data-ttu-id="bd5fc-257">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-257">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd5fc-258">示例</span><span class="sxs-lookup"><span data-stu-id="bd5fc-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd5fc-259">请求</span><span class="sxs-lookup"><span data-stu-id="bd5fc-259">Request</span></span>
<span data-ttu-id="bd5fc-260">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3387

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="bd5fc-261">响应</span><span class="sxs-lookup"><span data-stu-id="bd5fc-261">Response</span></span>
<span data-ttu-id="bd5fc-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd5fc-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3559

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




