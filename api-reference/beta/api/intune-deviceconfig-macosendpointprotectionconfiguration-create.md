---
title: 创建 macOSEndpointProtectionConfiguration
description: 创建新的 macOSEndpointProtectionConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 49f50856b00229ab6df952847172cda9b7cd19f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302105"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="b692f-103">创建 macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b692f-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="b692f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b692f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b692f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b692f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b692f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b692f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b692f-107">创建新的[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b692f-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b692f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b692f-108">Prerequisites</span></span>
<span data-ttu-id="b692f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b692f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b692f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b692f-111">Permission type</span></span>|<span data-ttu-id="b692f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b692f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b692f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b692f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b692f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b692f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b692f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b692f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b692f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b692f-116">Not supported.</span></span>|
|<span data-ttu-id="b692f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b692f-117">Application</span></span>|<span data-ttu-id="b692f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b692f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b692f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b692f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b692f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b692f-120">Request headers</span></span>
|<span data-ttu-id="b692f-121">标头</span><span class="sxs-lookup"><span data-stu-id="b692f-121">Header</span></span>|<span data-ttu-id="b692f-122">值</span><span class="sxs-lookup"><span data-stu-id="b692f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b692f-123">授权</span><span class="sxs-lookup"><span data-stu-id="b692f-123">Authorization</span></span>|<span data-ttu-id="b692f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b692f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b692f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b692f-125">Accept</span></span>|<span data-ttu-id="b692f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b692f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b692f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b692f-127">Request body</span></span>
<span data-ttu-id="b692f-128">在请求正文中，提供 macOSEndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b692f-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="b692f-129">下表显示时创建 macOSEndpointProtectionConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b692f-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="b692f-130">属性</span><span class="sxs-lookup"><span data-stu-id="b692f-130">Property</span></span>|<span data-ttu-id="b692f-131">类型</span><span class="sxs-lookup"><span data-stu-id="b692f-131">Type</span></span>|<span data-ttu-id="b692f-132">说明</span><span class="sxs-lookup"><span data-stu-id="b692f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b692f-133">id</span><span class="sxs-lookup"><span data-stu-id="b692f-133">id</span></span>|<span data-ttu-id="b692f-134">String</span><span class="sxs-lookup"><span data-stu-id="b692f-134">String</span></span>|<span data-ttu-id="b692f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b692f-135">Key of the entity.</span></span> <span data-ttu-id="b692f-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b692f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b692f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b692f-138">DateTimeOffset</span></span>|<span data-ttu-id="b692f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b692f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b692f-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b692f-141">roleScopeTagIds</span></span>|<span data-ttu-id="b692f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b692f-142">String collection</span></span>|<span data-ttu-id="b692f-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="b692f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b692f-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b692f-145">supportsScopeTags</span></span>|<span data-ttu-id="b692f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b692f-146">Boolean</span></span>|<span data-ttu-id="b692f-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="b692f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b692f-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b692f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b692f-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="b692f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b692f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b692f-150">This property is read-only.</span></span> <span data-ttu-id="b692f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b692f-152">createdDateTime</span></span>|<span data-ttu-id="b692f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b692f-153">DateTimeOffset</span></span>|<span data-ttu-id="b692f-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b692f-154">DateTime the object was created.</span></span> <span data-ttu-id="b692f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-156">description</span><span class="sxs-lookup"><span data-stu-id="b692f-156">description</span></span>|<span data-ttu-id="b692f-157">String</span><span class="sxs-lookup"><span data-stu-id="b692f-157">String</span></span>|<span data-ttu-id="b692f-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b692f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b692f-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b692f-160">displayName</span></span>|<span data-ttu-id="b692f-161">String</span><span class="sxs-lookup"><span data-stu-id="b692f-161">String</span></span>|<span data-ttu-id="b692f-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b692f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b692f-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-164">version</span><span class="sxs-lookup"><span data-stu-id="b692f-164">version</span></span>|<span data-ttu-id="b692f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b692f-165">Int32</span></span>|<span data-ttu-id="b692f-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b692f-166">Version of the device configuration.</span></span> <span data-ttu-id="b692f-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b692f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b692f-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="b692f-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="b692f-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="b692f-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="b692f-170">系统和确定可以从 macOS 设备上运行的下载位置应用程序的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="b692f-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="b692f-171">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="b692f-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="b692f-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="b692f-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="b692f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b692f-173">Boolean</span></span>|<span data-ttu-id="b692f-174">如果设置为 true，则用户将覆盖网关守卫将被禁用。</span><span class="sxs-lookup"><span data-stu-id="b692f-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="b692f-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="b692f-175">firewallEnabled</span></span>|<span data-ttu-id="b692f-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b692f-176">Boolean</span></span>|<span data-ttu-id="b692f-177">是否应启用防火墙，或不。</span><span class="sxs-lookup"><span data-stu-id="b692f-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="b692f-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="b692f-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="b692f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b692f-179">Boolean</span></span>|<span data-ttu-id="b692f-180">对应于"阻止所有传入连接"选项。</span><span class="sxs-lookup"><span data-stu-id="b692f-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="b692f-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="b692f-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="b692f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b692f-182">Boolean</span></span>|<span data-ttu-id="b692f-183">对应于"启用隐藏模式"。</span><span class="sxs-lookup"><span data-stu-id="b692f-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="b692f-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="b692f-184">firewallApplications</span></span>|<span data-ttu-id="b692f-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="b692f-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="b692f-186">具有防火墙设置的应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b692f-186">List of applications with firewall settings.</span></span> <span data-ttu-id="b692f-187">由用户决定不在此列表上的应用程序的防火墙设置。</span><span class="sxs-lookup"><span data-stu-id="b692f-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="b692f-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b692f-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b692f-189">响应</span><span class="sxs-lookup"><span data-stu-id="b692f-189">Response</span></span>
<span data-ttu-id="b692f-190">如果成功，此方法返回`201 Created`响应代码和响应正文中的[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b692f-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b692f-191">示例</span><span class="sxs-lookup"><span data-stu-id="b692f-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="b692f-192">请求</span><span class="sxs-lookup"><span data-stu-id="b692f-192">Request</span></span>
<span data-ttu-id="b692f-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b692f-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 711

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b692f-194">响应</span><span class="sxs-lookup"><span data-stu-id="b692f-194">Response</span></span>
<span data-ttu-id="b692f-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b692f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 819

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```





