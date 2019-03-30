---
title: 创建 windows10VpnConfiguration
description: 创建新的 windows10VpnConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa05bee08f30936ca496499090f8bdf9ee1877c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988656"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="0ca97-103">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ca97-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="0ca97-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ca97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ca97-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ca97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ca97-106">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ca97-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ca97-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ca97-107">Prerequisites</span></span>
<span data-ttu-id="0ca97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ca97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ca97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ca97-110">Permission type</span></span>|<span data-ttu-id="0ca97-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ca97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ca97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ca97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ca97-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca97-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ca97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ca97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ca97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ca97-115">Not supported.</span></span>|
|<span data-ttu-id="0ca97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ca97-116">Application</span></span>|<span data-ttu-id="0ca97-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ca97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ca97-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ca97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ca97-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ca97-119">Request headers</span></span>
|<span data-ttu-id="0ca97-120">标头</span><span class="sxs-lookup"><span data-stu-id="0ca97-120">Header</span></span>|<span data-ttu-id="0ca97-121">值</span><span class="sxs-lookup"><span data-stu-id="0ca97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ca97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ca97-122">Authorization</span></span>|<span data-ttu-id="0ca97-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ca97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ca97-124">接受</span><span class="sxs-lookup"><span data-stu-id="0ca97-124">Accept</span></span>|<span data-ttu-id="0ca97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ca97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ca97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ca97-126">Request body</span></span>
<span data-ttu-id="0ca97-127">在请求正文中, 提供 windows10VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ca97-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="0ca97-128">下表显示创建 windows10VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ca97-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="0ca97-129">属性</span><span class="sxs-lookup"><span data-stu-id="0ca97-129">Property</span></span>|<span data-ttu-id="0ca97-130">类型</span><span class="sxs-lookup"><span data-stu-id="0ca97-130">Type</span></span>|<span data-ttu-id="0ca97-131">说明</span><span class="sxs-lookup"><span data-stu-id="0ca97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ca97-132">id</span><span class="sxs-lookup"><span data-stu-id="0ca97-132">id</span></span>|<span data-ttu-id="0ca97-133">String</span><span class="sxs-lookup"><span data-stu-id="0ca97-133">String</span></span>|<span data-ttu-id="0ca97-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ca97-134">Key of the entity.</span></span> <span data-ttu-id="0ca97-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ca97-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0ca97-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ca97-137">DateTimeOffset</span></span>|<span data-ttu-id="0ca97-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ca97-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0ca97-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ca97-140">roleScopeTagIds</span></span>|<span data-ttu-id="0ca97-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-141">String collection</span></span>|<span data-ttu-id="0ca97-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0ca97-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ca97-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ca97-144">supportsScopeTags</span></span>|<span data-ttu-id="0ca97-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-145">Boolean</span></span>|<span data-ttu-id="0ca97-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0ca97-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ca97-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0ca97-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ca97-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0ca97-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ca97-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0ca97-149">This property is read-only.</span></span> <span data-ttu-id="0ca97-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ca97-151">createdDateTime</span></span>|<span data-ttu-id="0ca97-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ca97-152">DateTimeOffset</span></span>|<span data-ttu-id="0ca97-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ca97-153">DateTime the object was created.</span></span> <span data-ttu-id="0ca97-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-155">description</span><span class="sxs-lookup"><span data-stu-id="0ca97-155">description</span></span>|<span data-ttu-id="0ca97-156">String</span><span class="sxs-lookup"><span data-stu-id="0ca97-156">String</span></span>|<span data-ttu-id="0ca97-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0ca97-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ca97-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0ca97-159">displayName</span></span>|<span data-ttu-id="0ca97-160">String</span><span class="sxs-lookup"><span data-stu-id="0ca97-160">String</span></span>|<span data-ttu-id="0ca97-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0ca97-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ca97-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-163">version</span><span class="sxs-lookup"><span data-stu-id="0ca97-163">version</span></span>|<span data-ttu-id="0ca97-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0ca97-164">Int32</span></span>|<span data-ttu-id="0ca97-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0ca97-165">Version of the device configuration.</span></span> <span data-ttu-id="0ca97-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="0ca97-167">connectionName</span></span>|<span data-ttu-id="0ca97-168">String</span><span class="sxs-lookup"><span data-stu-id="0ca97-168">String</span></span>|<span data-ttu-id="0ca97-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0ca97-169">Connection name displayed to the user.</span></span> <span data-ttu-id="0ca97-170">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-171">台</span><span class="sxs-lookup"><span data-stu-id="0ca97-171">servers</span></span>|<span data-ttu-id="0ca97-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0ca97-173">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="0ca97-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="0ca97-174">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="0ca97-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0ca97-175">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ca97-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0ca97-176">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-177">customXml</span><span class="sxs-lookup"><span data-stu-id="0ca97-177">customXml</span></span>|<span data-ttu-id="0ca97-178">Binary</span><span class="sxs-lookup"><span data-stu-id="0ca97-178">Binary</span></span>|<span data-ttu-id="0ca97-179">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="0ca97-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="0ca97-180">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ca97-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ca97-181">profileTarget</span><span class="sxs-lookup"><span data-stu-id="0ca97-181">profileTarget</span></span>|[<span data-ttu-id="0ca97-182">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="0ca97-182">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="0ca97-183">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="0ca97-183">Profile target type.</span></span> <span data-ttu-id="0ca97-184">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="0ca97-184">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="0ca97-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="0ca97-185">connectionType</span></span>|[<span data-ttu-id="0ca97-186">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0ca97-186">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="0ca97-187">连接类型。</span><span class="sxs-lookup"><span data-stu-id="0ca97-187">Connection type.</span></span> <span data-ttu-id="0ca97-188">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="0ca97-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="0ca97-189">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0ca97-189">enableSplitTunneling</span></span>|<span data-ttu-id="0ca97-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-190">Boolean</span></span>|<span data-ttu-id="0ca97-191">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="0ca97-191">Enable split tunneling.</span></span>|
|<span data-ttu-id="0ca97-192">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="0ca97-192">enableAlwaysOn</span></span>|<span data-ttu-id="0ca97-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-193">Boolean</span></span>|<span data-ttu-id="0ca97-194">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="0ca97-194">Enable Always On mode.</span></span>|
|<span data-ttu-id="0ca97-195">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="0ca97-195">enableDeviceTunnel</span></span>|<span data-ttu-id="0ca97-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-196">Boolean</span></span>|<span data-ttu-id="0ca97-197">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="0ca97-197">Enable device tunnel.</span></span>|
|<span data-ttu-id="0ca97-198">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="0ca97-198">enableDnsRegistration</span></span>|<span data-ttu-id="0ca97-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-199">Boolean</span></span>|<span data-ttu-id="0ca97-200">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="0ca97-200">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="0ca97-201">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="0ca97-201">dnsSuffixes</span></span>|<span data-ttu-id="0ca97-202">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-202">String collection</span></span>|<span data-ttu-id="0ca97-203">指定要添加到 dns 搜索列表以正确路由短名称的 dns 后缀。</span><span class="sxs-lookup"><span data-stu-id="0ca97-203">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="0ca97-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ca97-204">authenticationMethod</span></span>|[<span data-ttu-id="0ca97-205">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ca97-205">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="0ca97-206">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0ca97-206">Authentication method.</span></span> <span data-ttu-id="0ca97-207">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="0ca97-207">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="0ca97-208">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="0ca97-208">rememberUserCredentials</span></span>|<span data-ttu-id="0ca97-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-209">Boolean</span></span>|<span data-ttu-id="0ca97-210">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="0ca97-210">Remember user credentials.</span></span>|
|<span data-ttu-id="0ca97-211">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="0ca97-211">enableConditionalAccess</span></span>|<span data-ttu-id="0ca97-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-212">Boolean</span></span>|<span data-ttu-id="0ca97-213">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="0ca97-213">Enable conditional access.</span></span>|
|<span data-ttu-id="0ca97-214">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="0ca97-214">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="0ca97-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-215">Boolean</span></span>|<span data-ttu-id="0ca97-216">启用具有备用证书的单一登录 (SSO)。</span><span class="sxs-lookup"><span data-stu-id="0ca97-216">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="0ca97-217">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="0ca97-217">singleSignOnEku</span></span>|[<span data-ttu-id="0ca97-218">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="0ca97-218">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="0ca97-219">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="0ca97-219">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="0ca97-220">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="0ca97-220">singleSignOnIssuerHash</span></span>|<span data-ttu-id="0ca97-221">String</span><span class="sxs-lookup"><span data-stu-id="0ca97-221">String</span></span>|<span data-ttu-id="0ca97-222">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="0ca97-222">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="0ca97-223">eapXml</span><span class="sxs-lookup"><span data-stu-id="0ca97-223">eapXml</span></span>|<span data-ttu-id="0ca97-224">Binary</span><span class="sxs-lookup"><span data-stu-id="0ca97-224">Binary</span></span>|<span data-ttu-id="0ca97-225">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="0ca97-225">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="0ca97-226">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="0ca97-226">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="0ca97-227">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0ca97-227">proxyServer</span></span>|[<span data-ttu-id="0ca97-228">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0ca97-228">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="0ca97-229">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="0ca97-229">Proxy Server.</span></span>|
|<span data-ttu-id="0ca97-230">associatedApps</span><span class="sxs-lookup"><span data-stu-id="0ca97-230">associatedApps</span></span>|<span data-ttu-id="0ca97-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="0ca97-232">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="0ca97-232">Associated Apps.</span></span> <span data-ttu-id="0ca97-233">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ca97-233">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0ca97-234">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="0ca97-234">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="0ca97-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca97-235">Boolean</span></span>|<span data-ttu-id="0ca97-236">仅关联的应用程序可以使用连接 (每个应用 VPN)。</span><span class="sxs-lookup"><span data-stu-id="0ca97-236">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="0ca97-237">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="0ca97-237">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="0ca97-238">String</span><span class="sxs-lookup"><span data-stu-id="0ca97-238">String</span></span>|<span data-ttu-id="0ca97-239">与此连接关联的 Windows 信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="0ca97-239">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="0ca97-240">trafficRules</span><span class="sxs-lookup"><span data-stu-id="0ca97-240">trafficRules</span></span>|<span data-ttu-id="0ca97-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="0ca97-242">流量规则。</span><span class="sxs-lookup"><span data-stu-id="0ca97-242">Traffic rules.</span></span> <span data-ttu-id="0ca97-243">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ca97-243">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0ca97-244">航线</span><span class="sxs-lookup"><span data-stu-id="0ca97-244">routes</span></span>|<span data-ttu-id="0ca97-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="0ca97-246">路由 (可选用于第三方提供程序)。</span><span class="sxs-lookup"><span data-stu-id="0ca97-246">Routes (optional for third-party providers).</span></span> <span data-ttu-id="0ca97-247">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ca97-247">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0ca97-248">dnsRules</span><span class="sxs-lookup"><span data-stu-id="0ca97-248">dnsRules</span></span>|<span data-ttu-id="0ca97-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="0ca97-250">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="0ca97-250">DNS rules.</span></span> <span data-ttu-id="0ca97-251">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ca97-251">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0ca97-252">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="0ca97-252">trustedNetworkDomains</span></span>|<span data-ttu-id="0ca97-253">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ca97-253">String collection</span></span>|<span data-ttu-id="0ca97-254">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="0ca97-254">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="0ca97-255">响应</span><span class="sxs-lookup"><span data-stu-id="0ca97-255">Response</span></span>
<span data-ttu-id="0ca97-256">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ca97-256">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ca97-257">示例</span><span class="sxs-lookup"><span data-stu-id="0ca97-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ca97-258">请求</span><span class="sxs-lookup"><span data-stu-id="0ca97-258">Request</span></span>
<span data-ttu-id="0ca97-259">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ca97-259">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ca97-260">响应</span><span class="sxs-lookup"><span data-stu-id="0ca97-260">Response</span></span>
<span data-ttu-id="0ca97-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ca97-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




