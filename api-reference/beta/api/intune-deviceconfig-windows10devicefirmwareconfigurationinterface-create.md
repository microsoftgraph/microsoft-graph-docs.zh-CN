---
title: 创建 windows10DeviceFirmwareConfigurationInterface
description: 创建新的 windows10DeviceFirmwareConfigurationInterface 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0469bb40efeda2ab1292594005be3a717295c720
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947587"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="27523-103">创建 windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="27523-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

> <span data-ttu-id="27523-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27523-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27523-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27523-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27523-106">创建新的[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27523-106">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27523-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="27523-107">Prerequisites</span></span>
<span data-ttu-id="27523-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27523-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27523-110">Permission type</span></span>|<span data-ttu-id="27523-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27523-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27523-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27523-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27523-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27523-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27523-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27523-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27523-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27523-115">Not supported.</span></span>|
|<span data-ttu-id="27523-116">Application</span><span class="sxs-lookup"><span data-stu-id="27523-116">Application</span></span>|<span data-ttu-id="27523-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27523-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27523-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27523-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="27523-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="27523-119">Request headers</span></span>
|<span data-ttu-id="27523-120">标头</span><span class="sxs-lookup"><span data-stu-id="27523-120">Header</span></span>|<span data-ttu-id="27523-121">值</span><span class="sxs-lookup"><span data-stu-id="27523-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27523-122">授权</span><span class="sxs-lookup"><span data-stu-id="27523-122">Authorization</span></span>|<span data-ttu-id="27523-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27523-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27523-124">接受</span><span class="sxs-lookup"><span data-stu-id="27523-124">Accept</span></span>|<span data-ttu-id="27523-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27523-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27523-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="27523-126">Request body</span></span>
<span data-ttu-id="27523-127">在请求正文中，提供 windows10DeviceFirmwareConfigurationInterface 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27523-127">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="27523-128">下表显示创建 windows10DeviceFirmwareConfigurationInterface 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27523-128">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="27523-129">属性</span><span class="sxs-lookup"><span data-stu-id="27523-129">Property</span></span>|<span data-ttu-id="27523-130">类型</span><span class="sxs-lookup"><span data-stu-id="27523-130">Type</span></span>|<span data-ttu-id="27523-131">说明</span><span class="sxs-lookup"><span data-stu-id="27523-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27523-132">id</span><span class="sxs-lookup"><span data-stu-id="27523-132">id</span></span>|<span data-ttu-id="27523-133">字符串</span><span class="sxs-lookup"><span data-stu-id="27523-133">String</span></span>|<span data-ttu-id="27523-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27523-134">Key of the entity.</span></span> <span data-ttu-id="27523-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27523-136">lastModifiedDateTime</span></span>|<span data-ttu-id="27523-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27523-137">DateTimeOffset</span></span>|<span data-ttu-id="27523-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27523-138">DateTime the object was last modified.</span></span> <span data-ttu-id="27523-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27523-140">roleScopeTagIds</span></span>|<span data-ttu-id="27523-141">String collection</span><span class="sxs-lookup"><span data-stu-id="27523-141">String collection</span></span>|<span data-ttu-id="27523-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="27523-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="27523-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="27523-144">supportsScopeTags</span></span>|<span data-ttu-id="27523-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="27523-145">Boolean</span></span>|<span data-ttu-id="27523-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="27523-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="27523-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="27523-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="27523-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="27523-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="27523-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="27523-149">This property is read-only.</span></span> <span data-ttu-id="27523-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="27523-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="27523-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="27523-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="27523-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="27523-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="27523-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="27523-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="27523-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="27523-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="27523-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="27523-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="27523-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="27523-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="27523-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="27523-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="27523-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="27523-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="27523-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27523-163">createdDateTime</span></span>|<span data-ttu-id="27523-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27523-164">DateTimeOffset</span></span>|<span data-ttu-id="27523-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27523-165">DateTime the object was created.</span></span> <span data-ttu-id="27523-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-167">说明</span><span class="sxs-lookup"><span data-stu-id="27523-167">description</span></span>|<span data-ttu-id="27523-168">String</span><span class="sxs-lookup"><span data-stu-id="27523-168">String</span></span>|<span data-ttu-id="27523-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="27523-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27523-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-171">displayName</span><span class="sxs-lookup"><span data-stu-id="27523-171">displayName</span></span>|<span data-ttu-id="27523-172">String</span><span class="sxs-lookup"><span data-stu-id="27523-172">String</span></span>|<span data-ttu-id="27523-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="27523-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27523-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-175">version</span><span class="sxs-lookup"><span data-stu-id="27523-175">version</span></span>|<span data-ttu-id="27523-176">Int32</span><span class="sxs-lookup"><span data-stu-id="27523-176">Int32</span></span>|<span data-ttu-id="27523-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="27523-177">Version of the device configuration.</span></span> <span data-ttu-id="27523-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27523-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27523-179">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="27523-179">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="27523-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="27523-180">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="27523-181">定义授予用户更改 UEFI 设置的权限级别。</span><span class="sxs-lookup"><span data-stu-id="27523-181">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="27523-182">可取值为：`notConfiguredOnly`、`none`。</span><span class="sxs-lookup"><span data-stu-id="27523-182">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="27523-183">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="27523-183">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="27523-184">启用</span><span class="sxs-lookup"><span data-stu-id="27523-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27523-185">定义是否启用 CPU 和 IO 虚拟化。</span><span class="sxs-lookup"><span data-stu-id="27523-185">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="27523-186">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27523-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="27523-187">照相机</span><span class="sxs-lookup"><span data-stu-id="27523-187">cameras</span></span>|[<span data-ttu-id="27523-188">启用</span><span class="sxs-lookup"><span data-stu-id="27523-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27523-189">定义是否启用内置相机。</span><span class="sxs-lookup"><span data-stu-id="27523-189">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="27523-190">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27523-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="27523-191">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="27523-191">microphonesAndSpeakers</span></span>|[<span data-ttu-id="27523-192">启用</span><span class="sxs-lookup"><span data-stu-id="27523-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27523-193">定义是否启用内置麦克风或扬声器。</span><span class="sxs-lookup"><span data-stu-id="27523-193">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="27523-194">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27523-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="27523-195">收发</span><span class="sxs-lookup"><span data-stu-id="27523-195">radios</span></span>|[<span data-ttu-id="27523-196">启用</span><span class="sxs-lookup"><span data-stu-id="27523-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27523-197">定义是否启用内置无线收发器（例如，WLAN、NFC、蓝牙）。</span><span class="sxs-lookup"><span data-stu-id="27523-197">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="27523-198">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27523-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="27523-199">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="27523-199">bootFromExternalMedia</span></span>|[<span data-ttu-id="27523-200">启用</span><span class="sxs-lookup"><span data-stu-id="27523-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27523-201">定义是否允许用户从外部媒体进行引导。</span><span class="sxs-lookup"><span data-stu-id="27523-201">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="27523-202">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27523-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="27523-203">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="27523-203">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="27523-204">启用</span><span class="sxs-lookup"><span data-stu-id="27523-204">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27523-205">定义是否允许用户从内置网络适配器启动。</span><span class="sxs-lookup"><span data-stu-id="27523-205">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="27523-206">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27523-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="27523-207">响应</span><span class="sxs-lookup"><span data-stu-id="27523-207">Response</span></span>
<span data-ttu-id="27523-208">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27523-208">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27523-209">示例</span><span class="sxs-lookup"><span data-stu-id="27523-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="27523-210">请求</span><span class="sxs-lookup"><span data-stu-id="27523-210">Request</span></span>
<span data-ttu-id="27523-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27523-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1309

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="27523-212">响应</span><span class="sxs-lookup"><span data-stu-id="27523-212">Response</span></span>
<span data-ttu-id="27523-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27523-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1481

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```





