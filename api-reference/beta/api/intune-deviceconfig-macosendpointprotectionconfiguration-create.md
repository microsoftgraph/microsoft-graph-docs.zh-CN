---
title: 创建 macOSEndpointProtectionConfiguration
description: 创建新的 macOSEndpointProtectionConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0ced93721538f745a05165175090397128e796a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171587"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="63d3d-103">创建 macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="63d3d-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="63d3d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63d3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63d3d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63d3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63d3d-106">创建新的[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63d3d-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63d3d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="63d3d-107">Prerequisites</span></span>
<span data-ttu-id="63d3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="63d3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63d3d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="63d3d-110">Permission type</span></span>|<span data-ttu-id="63d3d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63d3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63d3d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63d3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63d3d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d3d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63d3d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63d3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63d3d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63d3d-115">Not supported.</span></span>|
|<span data-ttu-id="63d3d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="63d3d-116">Application</span></span>|<span data-ttu-id="63d3d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="63d3d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63d3d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63d3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63d3d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="63d3d-119">Request headers</span></span>
|<span data-ttu-id="63d3d-120">标头</span><span class="sxs-lookup"><span data-stu-id="63d3d-120">Header</span></span>|<span data-ttu-id="63d3d-121">值</span><span class="sxs-lookup"><span data-stu-id="63d3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63d3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63d3d-122">Authorization</span></span>|<span data-ttu-id="63d3d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63d3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63d3d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="63d3d-124">Accept</span></span>|<span data-ttu-id="63d3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63d3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63d3d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="63d3d-126">Request body</span></span>
<span data-ttu-id="63d3d-127">在请求正文中, 提供 macOSEndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63d3d-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="63d3d-128">下表显示创建 macOSEndpointProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63d3d-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="63d3d-129">属性</span><span class="sxs-lookup"><span data-stu-id="63d3d-129">Property</span></span>|<span data-ttu-id="63d3d-130">类型</span><span class="sxs-lookup"><span data-stu-id="63d3d-130">Type</span></span>|<span data-ttu-id="63d3d-131">说明</span><span class="sxs-lookup"><span data-stu-id="63d3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63d3d-132">id</span><span class="sxs-lookup"><span data-stu-id="63d3d-132">id</span></span>|<span data-ttu-id="63d3d-133">String</span><span class="sxs-lookup"><span data-stu-id="63d3d-133">String</span></span>|<span data-ttu-id="63d3d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63d3d-134">Key of the entity.</span></span> <span data-ttu-id="63d3d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63d3d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="63d3d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63d3d-137">DateTimeOffset</span></span>|<span data-ttu-id="63d3d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63d3d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="63d3d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63d3d-140">roleScopeTagIds</span></span>|<span data-ttu-id="63d3d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="63d3d-141">String collection</span></span>|<span data-ttu-id="63d3d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="63d3d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63d3d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="63d3d-144">supportsScopeTags</span></span>|<span data-ttu-id="63d3d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="63d3d-145">Boolean</span></span>|<span data-ttu-id="63d3d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="63d3d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="63d3d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="63d3d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="63d3d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="63d3d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="63d3d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="63d3d-149">This property is read-only.</span></span> <span data-ttu-id="63d3d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63d3d-151">createdDateTime</span></span>|<span data-ttu-id="63d3d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63d3d-152">DateTimeOffset</span></span>|<span data-ttu-id="63d3d-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63d3d-153">DateTime the object was created.</span></span> <span data-ttu-id="63d3d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-155">description</span><span class="sxs-lookup"><span data-stu-id="63d3d-155">description</span></span>|<span data-ttu-id="63d3d-156">String</span><span class="sxs-lookup"><span data-stu-id="63d3d-156">String</span></span>|<span data-ttu-id="63d3d-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="63d3d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63d3d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="63d3d-159">displayName</span></span>|<span data-ttu-id="63d3d-160">String</span><span class="sxs-lookup"><span data-stu-id="63d3d-160">String</span></span>|<span data-ttu-id="63d3d-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="63d3d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63d3d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-163">version</span><span class="sxs-lookup"><span data-stu-id="63d3d-163">version</span></span>|<span data-ttu-id="63d3d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="63d3d-164">Int32</span></span>|<span data-ttu-id="63d3d-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="63d3d-165">Version of the device configuration.</span></span> <span data-ttu-id="63d3d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63d3d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63d3d-167">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="63d3d-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="63d3d-168">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="63d3d-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="63d3d-169">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="63d3d-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="63d3d-170">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="63d3d-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="63d3d-171">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="63d3d-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="63d3d-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="63d3d-172">Boolean</span></span>|<span data-ttu-id="63d3d-173">如果设置为 true, 将禁用网关的用户替代。</span><span class="sxs-lookup"><span data-stu-id="63d3d-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="63d3d-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="63d3d-174">firewallEnabled</span></span>|<span data-ttu-id="63d3d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="63d3d-175">Boolean</span></span>|<span data-ttu-id="63d3d-176">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="63d3d-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="63d3d-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="63d3d-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="63d3d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="63d3d-178">Boolean</span></span>|<span data-ttu-id="63d3d-179">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="63d3d-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="63d3d-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="63d3d-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="63d3d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="63d3d-181">Boolean</span></span>|<span data-ttu-id="63d3d-182">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="63d3d-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="63d3d-183">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="63d3d-183">firewallApplications</span></span>|<span data-ttu-id="63d3d-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="63d3d-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="63d3d-185">具有防火墙设置的应用程序列表。</span><span class="sxs-lookup"><span data-stu-id="63d3d-185">List of applications with firewall settings.</span></span> <span data-ttu-id="63d3d-186">不在此列表中的应用程序的防火墙设置由用户决定。</span><span class="sxs-lookup"><span data-stu-id="63d3d-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="63d3d-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="63d3d-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="63d3d-188">响应</span><span class="sxs-lookup"><span data-stu-id="63d3d-188">Response</span></span>
<span data-ttu-id="63d3d-189">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63d3d-189">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63d3d-190">示例</span><span class="sxs-lookup"><span data-stu-id="63d3d-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="63d3d-191">请求</span><span class="sxs-lookup"><span data-stu-id="63d3d-191">Request</span></span>
<span data-ttu-id="63d3d-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63d3d-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="63d3d-193">响应</span><span class="sxs-lookup"><span data-stu-id="63d3d-193">Response</span></span>
<span data-ttu-id="63d3d-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63d3d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




