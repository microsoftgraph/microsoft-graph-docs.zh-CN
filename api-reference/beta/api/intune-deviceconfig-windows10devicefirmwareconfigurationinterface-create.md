---
title: 创建 windows10DeviceFirmwareConfigurationInterface
description: 创建新的 windows10DeviceFirmwareConfigurationInterface 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7536a8f518b4b8d4bc55063ba8b45eab90777446
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725693"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="7ee6c-103">创建 windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="7ee6c-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

<span data-ttu-id="7ee6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ee6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ee6c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ee6c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ee6c-107">创建新的 [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-107">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ee6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ee6c-108">Prerequisites</span></span>
<span data-ttu-id="7ee6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ee6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ee6c-111">Permission type</span></span>|<span data-ttu-id="7ee6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ee6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ee6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ee6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ee6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ee6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ee6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ee6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ee6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-116">Not supported.</span></span>|
|<span data-ttu-id="7ee6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ee6c-117">Application</span></span>|<span data-ttu-id="7ee6c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ee6c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ee6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ee6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ee6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ee6c-120">Request headers</span></span>
|<span data-ttu-id="7ee6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ee6c-121">Header</span></span>|<span data-ttu-id="7ee6c-122">值</span><span class="sxs-lookup"><span data-stu-id="7ee6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ee6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ee6c-123">Authorization</span></span>|<span data-ttu-id="7ee6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ee6c-125">接受</span><span class="sxs-lookup"><span data-stu-id="7ee6c-125">Accept</span></span>|<span data-ttu-id="7ee6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ee6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ee6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ee6c-127">Request body</span></span>
<span data-ttu-id="7ee6c-128">在请求正文中，提供 windows10DeviceFirmwareConfigurationInterface 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-128">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="7ee6c-129">下表显示创建 windows10DeviceFirmwareConfigurationInterface 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-129">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="7ee6c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ee6c-130">Property</span></span>|<span data-ttu-id="7ee6c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ee6c-131">Type</span></span>|<span data-ttu-id="7ee6c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ee6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ee6c-133">id</span><span class="sxs-lookup"><span data-stu-id="7ee6c-133">id</span></span>|<span data-ttu-id="7ee6c-134">String</span><span class="sxs-lookup"><span data-stu-id="7ee6c-134">String</span></span>|<span data-ttu-id="7ee6c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-135">Key of the entity.</span></span> <span data-ttu-id="7ee6c-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ee6c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7ee6c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ee6c-138">DateTimeOffset</span></span>|<span data-ttu-id="7ee6c-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7ee6c-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ee6c-141">roleScopeTagIds</span></span>|<span data-ttu-id="7ee6c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="7ee6c-142">String collection</span></span>|<span data-ttu-id="7ee6c-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7ee6c-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7ee6c-145">supportsScopeTags</span></span>|<span data-ttu-id="7ee6c-146">布尔</span><span class="sxs-lookup"><span data-stu-id="7ee6c-146">Boolean</span></span>|<span data-ttu-id="7ee6c-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7ee6c-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7ee6c-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7ee6c-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-150">This property is read-only.</span></span> <span data-ttu-id="7ee6c-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7ee6c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7ee6c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7ee6c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7ee6c-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7ee6c-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7ee6c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7ee6c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7ee6c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7ee6c-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7ee6c-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7ee6c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7ee6c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7ee6c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7ee6c-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7ee6c-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ee6c-164">createdDateTime</span></span>|<span data-ttu-id="7ee6c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ee6c-165">DateTimeOffset</span></span>|<span data-ttu-id="7ee6c-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-166">DateTime the object was created.</span></span> <span data-ttu-id="7ee6c-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-168">说明</span><span class="sxs-lookup"><span data-stu-id="7ee6c-168">description</span></span>|<span data-ttu-id="7ee6c-169">String</span><span class="sxs-lookup"><span data-stu-id="7ee6c-169">String</span></span>|<span data-ttu-id="7ee6c-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ee6c-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7ee6c-172">displayName</span></span>|<span data-ttu-id="7ee6c-173">String</span><span class="sxs-lookup"><span data-stu-id="7ee6c-173">String</span></span>|<span data-ttu-id="7ee6c-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ee6c-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-176">version</span><span class="sxs-lookup"><span data-stu-id="7ee6c-176">version</span></span>|<span data-ttu-id="7ee6c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee6c-177">Int32</span></span>|<span data-ttu-id="7ee6c-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-178">Version of the device configuration.</span></span> <span data-ttu-id="7ee6c-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ee6c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ee6c-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="7ee6c-180">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="7ee6c-181">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="7ee6c-181">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="7ee6c-182">定义授予用户更改 UEFI 设置的权限级别。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-182">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="7ee6c-183">可取值为：`notConfiguredOnly`、`none`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-183">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="7ee6c-184">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="7ee6c-184">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="7ee6c-185">启用</span><span class="sxs-lookup"><span data-stu-id="7ee6c-185">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ee6c-186">定义是否启用 CPU 和 IO 虚拟化。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-186">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="7ee6c-187">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7ee6c-188">照相机</span><span class="sxs-lookup"><span data-stu-id="7ee6c-188">cameras</span></span>|[<span data-ttu-id="7ee6c-189">启用</span><span class="sxs-lookup"><span data-stu-id="7ee6c-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ee6c-190">定义是否启用内置相机。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-190">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="7ee6c-191">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7ee6c-192">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="7ee6c-192">microphonesAndSpeakers</span></span>|[<span data-ttu-id="7ee6c-193">启用</span><span class="sxs-lookup"><span data-stu-id="7ee6c-193">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ee6c-194">定义是否启用内置麦克风或扬声器。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-194">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="7ee6c-195">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-195">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7ee6c-196">收发</span><span class="sxs-lookup"><span data-stu-id="7ee6c-196">radios</span></span>|[<span data-ttu-id="7ee6c-197">启用</span><span class="sxs-lookup"><span data-stu-id="7ee6c-197">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ee6c-198">定义是否启用内置无线收发器（例如，WLAN、NFC、蓝牙）。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-198">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="7ee6c-199">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-199">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7ee6c-200">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="7ee6c-200">bootFromExternalMedia</span></span>|[<span data-ttu-id="7ee6c-201">启用</span><span class="sxs-lookup"><span data-stu-id="7ee6c-201">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ee6c-202">定义是否允许用户从外部媒体进行引导。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-202">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="7ee6c-203">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-203">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7ee6c-204">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="7ee6c-204">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="7ee6c-205">启用</span><span class="sxs-lookup"><span data-stu-id="7ee6c-205">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ee6c-206">定义是否允许用户从内置网络适配器启动。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-206">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="7ee6c-207">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-207">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ee6c-208">响应</span><span class="sxs-lookup"><span data-stu-id="7ee6c-208">Response</span></span>
<span data-ttu-id="7ee6c-209">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-209">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ee6c-210">示例</span><span class="sxs-lookup"><span data-stu-id="7ee6c-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ee6c-211">请求</span><span class="sxs-lookup"><span data-stu-id="7ee6c-211">Request</span></span>
<span data-ttu-id="7ee6c-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ee6c-213">响应</span><span class="sxs-lookup"><span data-stu-id="7ee6c-213">Response</span></span>
<span data-ttu-id="7ee6c-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ee6c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





