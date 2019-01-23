---
title: 更新 macOSEndpointProtectionConfiguration
description: 更新 macOSEndpointProtectionConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1659141c75ec003b4cfe2cd47279e02917e59dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407639"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="d9a22-103">更新 macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a22-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="d9a22-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d9a22-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9a22-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9a22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9a22-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9a22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a22-107">更新[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9a22-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9a22-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9a22-108">Prerequisites</span></span>
<span data-ttu-id="d9a22-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d9a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9a22-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9a22-111">Permission type</span></span>|<span data-ttu-id="d9a22-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9a22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9a22-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9a22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9a22-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a22-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9a22-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9a22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9a22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9a22-116">Not supported.</span></span>|
|<span data-ttu-id="d9a22-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9a22-117">Application</span></span>|<span data-ttu-id="d9a22-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9a22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9a22-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9a22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d9a22-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9a22-120">Request headers</span></span>
|<span data-ttu-id="d9a22-121">标头</span><span class="sxs-lookup"><span data-stu-id="d9a22-121">Header</span></span>|<span data-ttu-id="d9a22-122">值</span><span class="sxs-lookup"><span data-stu-id="d9a22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9a22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9a22-123">Authorization</span></span>|<span data-ttu-id="d9a22-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9a22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9a22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9a22-125">Accept</span></span>|<span data-ttu-id="d9a22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9a22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9a22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9a22-127">Request body</span></span>
<span data-ttu-id="d9a22-128">在请求正文中，提供[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9a22-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="d9a22-129">下表显示时创建[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9a22-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="d9a22-130">属性</span><span class="sxs-lookup"><span data-stu-id="d9a22-130">Property</span></span>|<span data-ttu-id="d9a22-131">类型</span><span class="sxs-lookup"><span data-stu-id="d9a22-131">Type</span></span>|<span data-ttu-id="d9a22-132">说明</span><span class="sxs-lookup"><span data-stu-id="d9a22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a22-133">id</span><span class="sxs-lookup"><span data-stu-id="d9a22-133">id</span></span>|<span data-ttu-id="d9a22-134">String</span><span class="sxs-lookup"><span data-stu-id="d9a22-134">String</span></span>|<span data-ttu-id="d9a22-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9a22-135">Key of the entity.</span></span> <span data-ttu-id="d9a22-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9a22-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d9a22-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9a22-138">DateTimeOffset</span></span>|<span data-ttu-id="d9a22-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9a22-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d9a22-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9a22-141">roleScopeTagIds</span></span>|<span data-ttu-id="d9a22-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9a22-142">String collection</span></span>|<span data-ttu-id="d9a22-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d9a22-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9a22-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d9a22-145">supportsScopeTags</span></span>|<span data-ttu-id="d9a22-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a22-146">Boolean</span></span>|<span data-ttu-id="d9a22-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d9a22-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d9a22-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d9a22-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d9a22-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d9a22-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d9a22-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d9a22-150">This property is read-only.</span></span> <span data-ttu-id="d9a22-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9a22-152">createdDateTime</span></span>|<span data-ttu-id="d9a22-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9a22-153">DateTimeOffset</span></span>|<span data-ttu-id="d9a22-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9a22-154">DateTime the object was created.</span></span> <span data-ttu-id="d9a22-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-156">description</span><span class="sxs-lookup"><span data-stu-id="d9a22-156">description</span></span>|<span data-ttu-id="d9a22-157">String</span><span class="sxs-lookup"><span data-stu-id="d9a22-157">String</span></span>|<span data-ttu-id="d9a22-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d9a22-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9a22-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d9a22-160">displayName</span></span>|<span data-ttu-id="d9a22-161">String</span><span class="sxs-lookup"><span data-stu-id="d9a22-161">String</span></span>|<span data-ttu-id="d9a22-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d9a22-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9a22-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-164">version</span><span class="sxs-lookup"><span data-stu-id="d9a22-164">version</span></span>|<span data-ttu-id="d9a22-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a22-165">Int32</span></span>|<span data-ttu-id="d9a22-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d9a22-166">Version of the device configuration.</span></span> <span data-ttu-id="d9a22-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a22-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a22-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="d9a22-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="d9a22-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="d9a22-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="d9a22-170">系统和确定可以从 macOS 设备上运行的下载位置应用程序的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="d9a22-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="d9a22-171">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="d9a22-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="d9a22-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="d9a22-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="d9a22-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a22-173">Boolean</span></span>|<span data-ttu-id="d9a22-174">如果设置为 true，则用户将覆盖网关守卫将被禁用。</span><span class="sxs-lookup"><span data-stu-id="d9a22-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="d9a22-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="d9a22-175">firewallEnabled</span></span>|<span data-ttu-id="d9a22-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a22-176">Boolean</span></span>|<span data-ttu-id="d9a22-177">是否应启用防火墙，或不。</span><span class="sxs-lookup"><span data-stu-id="d9a22-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="d9a22-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="d9a22-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="d9a22-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a22-179">Boolean</span></span>|<span data-ttu-id="d9a22-180">对应于"阻止所有传入连接"选项。</span><span class="sxs-lookup"><span data-stu-id="d9a22-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="d9a22-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="d9a22-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="d9a22-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a22-182">Boolean</span></span>|<span data-ttu-id="d9a22-183">对应于"启用隐藏模式"。</span><span class="sxs-lookup"><span data-stu-id="d9a22-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="d9a22-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="d9a22-184">firewallApplications</span></span>|<span data-ttu-id="d9a22-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9a22-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="d9a22-186">具有防火墙设置的应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="d9a22-186">List of applications with firewall settings.</span></span> <span data-ttu-id="d9a22-187">由用户决定不在此列表上的应用程序的防火墙设置。</span><span class="sxs-lookup"><span data-stu-id="d9a22-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="d9a22-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d9a22-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d9a22-189">响应</span><span class="sxs-lookup"><span data-stu-id="d9a22-189">Response</span></span>
<span data-ttu-id="d9a22-190">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d9a22-190">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9a22-191">示例</span><span class="sxs-lookup"><span data-stu-id="d9a22-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9a22-192">请求</span><span class="sxs-lookup"><span data-stu-id="d9a22-192">Request</span></span>
<span data-ttu-id="d9a22-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9a22-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="d9a22-194">响应</span><span class="sxs-lookup"><span data-stu-id="d9a22-194">Response</span></span>
<span data-ttu-id="d9a22-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9a22-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




