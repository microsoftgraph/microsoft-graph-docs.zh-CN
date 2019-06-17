---
title: 创建 androidForWorkVpnConfiguration
description: 创建新的 androidForWorkVpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef8e6039bed0d0b80f3306ac6ab875bc58ac4cec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970378"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="ddffe-103">创建 androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddffe-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="ddffe-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ddffe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddffe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddffe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddffe-106">创建新的[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ddffe-106">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddffe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddffe-107">Prerequisites</span></span>
<span data-ttu-id="ddffe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddffe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddffe-110">Permission type</span></span>|<span data-ttu-id="ddffe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddffe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddffe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddffe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddffe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddffe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddffe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddffe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddffe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddffe-115">Not supported.</span></span>|
|<span data-ttu-id="ddffe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddffe-116">Application</span></span>|<span data-ttu-id="ddffe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddffe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddffe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddffe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ddffe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddffe-119">Request headers</span></span>
|<span data-ttu-id="ddffe-120">标头</span><span class="sxs-lookup"><span data-stu-id="ddffe-120">Header</span></span>|<span data-ttu-id="ddffe-121">值</span><span class="sxs-lookup"><span data-stu-id="ddffe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddffe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddffe-122">Authorization</span></span>|<span data-ttu-id="ddffe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddffe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddffe-124">接受</span><span class="sxs-lookup"><span data-stu-id="ddffe-124">Accept</span></span>|<span data-ttu-id="ddffe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddffe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddffe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddffe-126">Request body</span></span>
<span data-ttu-id="ddffe-127">在请求正文中, 提供 androidForWorkVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddffe-127">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="ddffe-128">下表显示创建 androidForWorkVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddffe-128">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="ddffe-129">属性</span><span class="sxs-lookup"><span data-stu-id="ddffe-129">Property</span></span>|<span data-ttu-id="ddffe-130">类型</span><span class="sxs-lookup"><span data-stu-id="ddffe-130">Type</span></span>|<span data-ttu-id="ddffe-131">说明</span><span class="sxs-lookup"><span data-stu-id="ddffe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddffe-132">id</span><span class="sxs-lookup"><span data-stu-id="ddffe-132">id</span></span>|<span data-ttu-id="ddffe-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ddffe-133">String</span></span>|<span data-ttu-id="ddffe-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddffe-134">Key of the entity.</span></span> <span data-ttu-id="ddffe-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddffe-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ddffe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddffe-137">DateTimeOffset</span></span>|<span data-ttu-id="ddffe-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddffe-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ddffe-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddffe-140">roleScopeTagIds</span></span>|<span data-ttu-id="ddffe-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ddffe-141">String collection</span></span>|<span data-ttu-id="ddffe-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ddffe-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ddffe-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ddffe-144">supportsScopeTags</span></span>|<span data-ttu-id="ddffe-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddffe-145">Boolean</span></span>|<span data-ttu-id="ddffe-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ddffe-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ddffe-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ddffe-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ddffe-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ddffe-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ddffe-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ddffe-149">This property is read-only.</span></span> <span data-ttu-id="ddffe-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddffe-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ddffe-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddffe-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ddffe-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ddffe-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ddffe-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddffe-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ddffe-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddffe-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ddffe-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ddffe-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ddffe-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddffe-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ddffe-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddffe-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ddffe-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ddffe-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ddffe-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddffe-163">createdDateTime</span></span>|<span data-ttu-id="ddffe-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddffe-164">DateTimeOffset</span></span>|<span data-ttu-id="ddffe-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddffe-165">DateTime the object was created.</span></span> <span data-ttu-id="ddffe-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-167">说明</span><span class="sxs-lookup"><span data-stu-id="ddffe-167">description</span></span>|<span data-ttu-id="ddffe-168">String</span><span class="sxs-lookup"><span data-stu-id="ddffe-168">String</span></span>|<span data-ttu-id="ddffe-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddffe-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddffe-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ddffe-171">displayName</span></span>|<span data-ttu-id="ddffe-172">String</span><span class="sxs-lookup"><span data-stu-id="ddffe-172">String</span></span>|<span data-ttu-id="ddffe-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddffe-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddffe-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-175">version</span><span class="sxs-lookup"><span data-stu-id="ddffe-175">version</span></span>|<span data-ttu-id="ddffe-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ddffe-176">Int32</span></span>|<span data-ttu-id="ddffe-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddffe-177">Version of the device configuration.</span></span> <span data-ttu-id="ddffe-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddffe-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddffe-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="ddffe-179">connectionName</span></span>|<span data-ttu-id="ddffe-180">String</span><span class="sxs-lookup"><span data-stu-id="ddffe-180">String</span></span>|<span data-ttu-id="ddffe-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="ddffe-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ddffe-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="ddffe-182">connectionType</span></span>|[<span data-ttu-id="ddffe-183">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ddffe-183">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="ddffe-184">连接类型。</span><span class="sxs-lookup"><span data-stu-id="ddffe-184">Connection type.</span></span> <span data-ttu-id="ddffe-185">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="ddffe-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="ddffe-186">role</span><span class="sxs-lookup"><span data-stu-id="ddffe-186">role</span></span>|<span data-ttu-id="ddffe-187">String</span><span class="sxs-lookup"><span data-stu-id="ddffe-187">String</span></span>|<span data-ttu-id="ddffe-188">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="ddffe-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ddffe-189">型</span><span class="sxs-lookup"><span data-stu-id="ddffe-189">realm</span></span>|<span data-ttu-id="ddffe-190">String</span><span class="sxs-lookup"><span data-stu-id="ddffe-190">String</span></span>|<span data-ttu-id="ddffe-191">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="ddffe-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ddffe-192">台</span><span class="sxs-lookup"><span data-stu-id="ddffe-192">servers</span></span>|<span data-ttu-id="ddffe-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="ddffe-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ddffe-194">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="ddffe-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="ddffe-195">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="ddffe-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ddffe-196">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddffe-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ddffe-197">其次</span><span class="sxs-lookup"><span data-stu-id="ddffe-197">fingerprint</span></span>|<span data-ttu-id="ddffe-198">String</span><span class="sxs-lookup"><span data-stu-id="ddffe-198">String</span></span>|<span data-ttu-id="ddffe-199">指纹是一个字符串, 用于验证 VPN 服务器是否可以信任, 这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="ddffe-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ddffe-200">customData</span><span class="sxs-lookup"><span data-stu-id="ddffe-200">customData</span></span>|<span data-ttu-id="ddffe-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddffe-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ddffe-202">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="ddffe-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ddffe-203">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="ddffe-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ddffe-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ddffe-204">customKeyValueData</span></span>|<span data-ttu-id="ddffe-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddffe-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ddffe-206">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="ddffe-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ddffe-207">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="ddffe-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ddffe-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ddffe-208">authenticationMethod</span></span>|[<span data-ttu-id="ddffe-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ddffe-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ddffe-210">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ddffe-210">Authentication method.</span></span> <span data-ttu-id="ddffe-211">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="ddffe-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="ddffe-212">响应</span><span class="sxs-lookup"><span data-stu-id="ddffe-212">Response</span></span>
<span data-ttu-id="ddffe-213">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ddffe-213">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddffe-214">示例</span><span class="sxs-lookup"><span data-stu-id="ddffe-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddffe-215">请求</span><span class="sxs-lookup"><span data-stu-id="ddffe-215">Request</span></span>
<span data-ttu-id="ddffe-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddffe-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1758

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="ddffe-217">响应</span><span class="sxs-lookup"><span data-stu-id="ddffe-217">Response</span></span>
<span data-ttu-id="ddffe-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddffe-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1930

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```





