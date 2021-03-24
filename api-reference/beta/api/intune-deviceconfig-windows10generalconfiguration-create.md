---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c91ad286a007a52e420f8e699ab50b8e74c5aa55
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127835"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="74988-103">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="74988-103">Create windows10GeneralConfiguration</span></span>

<span data-ttu-id="74988-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74988-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74988-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74988-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74988-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74988-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74988-107">创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74988-107">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74988-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="74988-108">Prerequisites</span></span>
<span data-ttu-id="74988-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74988-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74988-111">Permission type</span></span>|<span data-ttu-id="74988-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74988-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74988-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74988-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74988-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74988-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74988-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74988-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74988-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74988-116">Not supported.</span></span>|
|<span data-ttu-id="74988-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74988-117">Application</span></span>|<span data-ttu-id="74988-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74988-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74988-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74988-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74988-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74988-120">Request headers</span></span>
|<span data-ttu-id="74988-121">标头</span><span class="sxs-lookup"><span data-stu-id="74988-121">Header</span></span>|<span data-ttu-id="74988-122">值</span><span class="sxs-lookup"><span data-stu-id="74988-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74988-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74988-123">Authorization</span></span>|<span data-ttu-id="74988-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74988-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74988-125">接受</span><span class="sxs-lookup"><span data-stu-id="74988-125">Accept</span></span>|<span data-ttu-id="74988-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74988-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74988-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74988-127">Request body</span></span>
<span data-ttu-id="74988-128">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74988-128">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="74988-129">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74988-129">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="74988-130">属性</span><span class="sxs-lookup"><span data-stu-id="74988-130">Property</span></span>|<span data-ttu-id="74988-131">类型</span><span class="sxs-lookup"><span data-stu-id="74988-131">Type</span></span>|<span data-ttu-id="74988-132">说明</span><span class="sxs-lookup"><span data-stu-id="74988-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74988-133">id</span><span class="sxs-lookup"><span data-stu-id="74988-133">id</span></span>|<span data-ttu-id="74988-134">String</span><span class="sxs-lookup"><span data-stu-id="74988-134">String</span></span>|<span data-ttu-id="74988-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74988-135">Key of the entity.</span></span> <span data-ttu-id="74988-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74988-137">lastModifiedDateTime</span></span>|<span data-ttu-id="74988-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74988-138">DateTimeOffset</span></span>|<span data-ttu-id="74988-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="74988-139">DateTime the object was last modified.</span></span> <span data-ttu-id="74988-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="74988-141">roleScopeTagIds</span></span>|<span data-ttu-id="74988-142">String collection</span><span class="sxs-lookup"><span data-stu-id="74988-142">String collection</span></span>|<span data-ttu-id="74988-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="74988-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="74988-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="74988-145">supportsScopeTags</span></span>|<span data-ttu-id="74988-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-146">Boolean</span></span>|<span data-ttu-id="74988-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="74988-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="74988-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="74988-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="74988-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="74988-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="74988-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="74988-150">This property is read-only.</span></span> <span data-ttu-id="74988-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="74988-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="74988-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="74988-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="74988-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="74988-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="74988-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="74988-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="74988-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="74988-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="74988-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="74988-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="74988-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="74988-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="74988-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="74988-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="74988-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="74988-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="74988-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74988-164">createdDateTime</span></span>|<span data-ttu-id="74988-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74988-165">DateTimeOffset</span></span>|<span data-ttu-id="74988-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="74988-166">DateTime the object was created.</span></span> <span data-ttu-id="74988-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-168">说明</span><span class="sxs-lookup"><span data-stu-id="74988-168">description</span></span>|<span data-ttu-id="74988-169">String</span><span class="sxs-lookup"><span data-stu-id="74988-169">String</span></span>|<span data-ttu-id="74988-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="74988-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74988-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-172">displayName</span><span class="sxs-lookup"><span data-stu-id="74988-172">displayName</span></span>|<span data-ttu-id="74988-173">String</span><span class="sxs-lookup"><span data-stu-id="74988-173">String</span></span>|<span data-ttu-id="74988-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="74988-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74988-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-176">version</span><span class="sxs-lookup"><span data-stu-id="74988-176">version</span></span>|<span data-ttu-id="74988-177">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-177">Int32</span></span>|<span data-ttu-id="74988-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="74988-178">Version of the device configuration.</span></span> <span data-ttu-id="74988-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74988-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74988-180">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="74988-180">taskManagerBlockEndTask</span></span>|<span data-ttu-id="74988-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-181">Boolean</span></span>|<span data-ttu-id="74988-182">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="74988-182">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="74988-183">energySaverOnBatteryThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="74988-183">energySaverOnBatteryThresholdPercentage</span></span>|<span data-ttu-id="74988-184">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-184">Int32</span></span>|<span data-ttu-id="74988-185">此设置允许你指定节电模式打开的电池充电级别。</span><span class="sxs-lookup"><span data-stu-id="74988-185">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="74988-186">当使用电池时，节电模式将在 (或低于指定) 电量时自动打开。</span><span class="sxs-lookup"><span data-stu-id="74988-186">While on battery, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="74988-187">有效输入范围 (0-100) 。</span><span class="sxs-lookup"><span data-stu-id="74988-187">Valid input range (0-100).</span></span> <span data-ttu-id="74988-188">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="74988-188">Valid values 0 to 100</span></span>|
|<span data-ttu-id="74988-189">energySaverPluggedInThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="74988-189">energySaverPluggedInThresholdPercentage</span></span>|<span data-ttu-id="74988-190">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-190">Int32</span></span>|<span data-ttu-id="74988-191">此设置允许你指定节电模式打开的电池充电级别。</span><span class="sxs-lookup"><span data-stu-id="74988-191">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="74988-192">接通电源时，将在指定的电池充电 (低于) 自动打开节电模式。</span><span class="sxs-lookup"><span data-stu-id="74988-192">While plugged in, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="74988-193">有效输入范围 (0-100) 。</span><span class="sxs-lookup"><span data-stu-id="74988-193">Valid input range (0-100).</span></span> <span data-ttu-id="74988-194">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="74988-194">Valid values 0 to 100</span></span>|
|<span data-ttu-id="74988-195">powerLidCloseActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="74988-195">powerLidCloseActionOnBattery</span></span>|[<span data-ttu-id="74988-196">powerActionType</span><span class="sxs-lookup"><span data-stu-id="74988-196">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="74988-197">此设置指定当用户使用电池时关闭移动电脑上的灯盖时 Windows 执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74988-197">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while on battery.</span></span> <span data-ttu-id="74988-198">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="74988-198">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="74988-199">powerLidCloseActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="74988-199">powerLidCloseActionPluggedIn</span></span>|[<span data-ttu-id="74988-200">powerActionType</span><span class="sxs-lookup"><span data-stu-id="74988-200">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="74988-201">此设置指定当用户在插入时关闭移动电脑上的灯盖时 Windows 执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74988-201">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while plugged in.</span></span> <span data-ttu-id="74988-202">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="74988-202">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="74988-203">powerButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="74988-203">powerButtonActionOnBattery</span></span>|[<span data-ttu-id="74988-204">powerActionType</span><span class="sxs-lookup"><span data-stu-id="74988-204">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="74988-205">此设置指定用户在使用电池时按下电源按钮时 Windows 所执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74988-205">This setting specifies the action that Windows takes when a user presses the Power button while on battery.</span></span> <span data-ttu-id="74988-206">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="74988-206">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="74988-207">powerButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="74988-207">powerButtonActionPluggedIn</span></span>|[<span data-ttu-id="74988-208">powerActionType</span><span class="sxs-lookup"><span data-stu-id="74988-208">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="74988-209">此设置指定用户在接通电源时按下电源按钮时 Windows 所执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74988-209">This setting specifies the action that Windows takes when a user presses the Power button while plugged in.</span></span> <span data-ttu-id="74988-210">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="74988-210">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="74988-211">powerSleepButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="74988-211">powerSleepButtonActionOnBattery</span></span>|[<span data-ttu-id="74988-212">powerActionType</span><span class="sxs-lookup"><span data-stu-id="74988-212">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="74988-213">此设置指定用户在使用电池时按下睡眠按钮时 Windows 所执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74988-213">This setting specifies the action that Windows takes when a user presses the Sleep button while on battery.</span></span> <span data-ttu-id="74988-214">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="74988-214">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="74988-215">powerSleepButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="74988-215">powerSleepButtonActionPluggedIn</span></span>|[<span data-ttu-id="74988-216">powerActionType</span><span class="sxs-lookup"><span data-stu-id="74988-216">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="74988-217">此设置指定用户在插入时按下"睡眠"按钮时 Windows 所执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74988-217">This setting specifies the action that Windows takes when a user presses the Sleep button while plugged in.</span></span> <span data-ttu-id="74988-218">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="74988-218">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="74988-219">powerHybridSleepOnBattery</span><span class="sxs-lookup"><span data-stu-id="74988-219">powerHybridSleepOnBattery</span></span>|[<span data-ttu-id="74988-220">enablement</span><span class="sxs-lookup"><span data-stu-id="74988-220">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="74988-221">此设置允许你在使用电池时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="74988-221">This setting allows you to turn off hybrid sleep while on battery.</span></span> <span data-ttu-id="74988-222">如果将此设置设置为禁用，则当系统切换为睡眠模式时，不会生成休眠文件 (独立) 。</span><span class="sxs-lookup"><span data-stu-id="74988-222">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="74988-223">如果将此设置设置为启用或不配置此策略设置，则用户控制此设置。</span><span class="sxs-lookup"><span data-stu-id="74988-223">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="74988-224">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-224">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-225">powerHybridSleepPluggedIn</span><span class="sxs-lookup"><span data-stu-id="74988-225">powerHybridSleepPluggedIn</span></span>|[<span data-ttu-id="74988-226">enablement</span><span class="sxs-lookup"><span data-stu-id="74988-226">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="74988-227">此设置允许你在插入时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="74988-227">This setting allows you to turn off hybrid sleep while plugged in.</span></span> <span data-ttu-id="74988-228">如果将此设置设置为禁用，则当系统切换为睡眠模式时，不会生成休眠文件 (独立) 。</span><span class="sxs-lookup"><span data-stu-id="74988-228">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="74988-229">如果将此设置设置为启用或不配置此策略设置，则用户控制此设置。</span><span class="sxs-lookup"><span data-stu-id="74988-229">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="74988-230">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-230">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-231">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="74988-231">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="74988-232">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="74988-232">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="74988-233">适用于应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="74988-233">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="74988-234">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="74988-234">enableAutomaticRedeployment</span></span>|<span data-ttu-id="74988-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-235">Boolean</span></span>|<span data-ttu-id="74988-236">允许具有管理权限的用户在设备锁屏界面上使用 Ctrl + Win + R 删除所有用户数据和设置，以便设备可以自动重新配置并重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="74988-236">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="74988-237">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="74988-237">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="74988-238">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="74988-238">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="74988-239">控制 wlidsvc Sign-In NT (的 Microsoft) 助手。</span><span class="sxs-lookup"><span data-stu-id="74988-239">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="74988-240">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-240">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="74988-241">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="74988-241">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="74988-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-242">Boolean</span></span>|<span data-ttu-id="74988-243">允许辅助身份验证设备与 Windows 一起运行。</span><span class="sxs-lookup"><span data-stu-id="74988-243">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="74988-244">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="74988-244">authenticationWebSignIn</span></span>|[<span data-ttu-id="74988-245">enablement</span><span class="sxs-lookup"><span data-stu-id="74988-245">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="74988-246">指示是否将启用 Web 凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="74988-246">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="74988-247">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-247">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-248">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="74988-248">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="74988-249">String</span><span class="sxs-lookup"><span data-stu-id="74988-249">String</span></span>|<span data-ttu-id="74988-250">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="74988-250">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="74988-251">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="74988-251">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="74988-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-252">Boolean</span></span>|<span data-ttu-id="74988-253">指定是允许还是禁止联邦信息处理标准 (FIPS) 策略。</span><span class="sxs-lookup"><span data-stu-id="74988-253">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="74988-254">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="74988-254">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="74988-255">String collection</span><span class="sxs-lookup"><span data-stu-id="74988-255">String collection</span></span>|<span data-ttu-id="74988-256">已打开 GDI DPI 缩放的旧应用程序列表。</span><span class="sxs-lookup"><span data-stu-id="74988-256">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="74988-257">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="74988-257">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="74988-258">String collection</span><span class="sxs-lookup"><span data-stu-id="74988-258">String collection</span></span>|<span data-ttu-id="74988-259">已关闭 GDI DPI 缩放的旧应用程序列表。</span><span class="sxs-lookup"><span data-stu-id="74988-259">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="74988-260">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="74988-260">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="74988-261">String</span><span class="sxs-lookup"><span data-stu-id="74988-261">String</span></span>|<span data-ttu-id="74988-262">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="74988-262">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="74988-263">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="74988-263">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="74988-264">String</span><span class="sxs-lookup"><span data-stu-id="74988-264">String</span></span>|<span data-ttu-id="74988-265">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="74988-265">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="74988-266">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="74988-266">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="74988-267">String</span><span class="sxs-lookup"><span data-stu-id="74988-267">String</span></span>|<span data-ttu-id="74988-268">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="74988-268">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="74988-269">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="74988-269">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="74988-270">String</span><span class="sxs-lookup"><span data-stu-id="74988-270">String</span></span>|<span data-ttu-id="74988-271">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="74988-271">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="74988-272">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="74988-272">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="74988-273">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-273">Int32</span></span>|<span data-ttu-id="74988-274">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="74988-274">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="74988-275">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="74988-275">This is a mobile only setting.</span></span> <span data-ttu-id="74988-276">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="74988-276">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="74988-277">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="74988-277">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="74988-278">String</span><span class="sxs-lookup"><span data-stu-id="74988-278">String</span></span>|<span data-ttu-id="74988-279">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="74988-279">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="74988-280">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="74988-280">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="74988-281">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="74988-281">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="74988-282">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="74988-282">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="74988-283">供 IT 管理员用于阻止跨设备同步但允许用户替代的选项。</span><span class="sxs-lookup"><span data-stu-id="74988-283">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="74988-284">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="74988-284">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="74988-285">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="74988-285">messagingBlockSync</span></span>|<span data-ttu-id="74988-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-286">Boolean</span></span>|<span data-ttu-id="74988-287">指示是否阻止文本消息备份和还原以及邮件无处不在。</span><span class="sxs-lookup"><span data-stu-id="74988-287">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="74988-288">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="74988-288">messagingBlockMMS</span></span>|<span data-ttu-id="74988-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-289">Boolean</span></span>|<span data-ttu-id="74988-290">指示是否阻止设备上 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="74988-290">Indicates whether or not to block the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="74988-291">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="74988-291">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="74988-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-292">Boolean</span></span>|<span data-ttu-id="74988-293">指示是否阻止设备上 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="74988-293">Indicates whether or not to block the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="74988-294">printerNames</span><span class="sxs-lookup"><span data-stu-id="74988-294">printerNames</span></span>|<span data-ttu-id="74988-295">String collection</span><span class="sxs-lookup"><span data-stu-id="74988-295">String collection</span></span>|<span data-ttu-id="74988-296">根据打印机的名称自动预配 (网络主机) 。</span><span class="sxs-lookup"><span data-stu-id="74988-296">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="74988-297">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="74988-297">printerDefaultName</span></span>|<span data-ttu-id="74988-298">String</span><span class="sxs-lookup"><span data-stu-id="74988-298">String</span></span>|<span data-ttu-id="74988-299">名称 (已安装) 的网络主机名。</span><span class="sxs-lookup"><span data-stu-id="74988-299">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="74988-300">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="74988-300">printerBlockAddition</span></span>|<span data-ttu-id="74988-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-301">Boolean</span></span>|<span data-ttu-id="74988-302">阻止用户从打印机设置安装其他打印机。</span><span class="sxs-lookup"><span data-stu-id="74988-302">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="74988-303">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="74988-303">searchBlockDiacritics</span></span>|<span data-ttu-id="74988-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-304">Boolean</span></span>|<span data-ttu-id="74988-305">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="74988-305">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="74988-306">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="74988-306">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="74988-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-307">Boolean</span></span>|<span data-ttu-id="74988-308">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="74988-308">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="74988-309">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="74988-309">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="74988-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-310">Boolean</span></span>|<span data-ttu-id="74988-311">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="74988-311">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="74988-312">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="74988-312">searchEnableRemoteQueries</span></span>|<span data-ttu-id="74988-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-313">Boolean</span></span>|<span data-ttu-id="74988-314">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="74988-314">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="74988-315">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="74988-315">searchDisableUseLocation</span></span>|<span data-ttu-id="74988-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-316">Boolean</span></span>|<span data-ttu-id="74988-317">指定搜索是否可使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="74988-317">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="74988-318">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="74988-318">searchDisableLocation</span></span>|<span data-ttu-id="74988-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-319">Boolean</span></span>|<span data-ttu-id="74988-320">指定搜索是否可使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="74988-320">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="74988-321">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="74988-321">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="74988-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-322">Boolean</span></span>|<span data-ttu-id="74988-323">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="74988-323">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="74988-324">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="74988-324">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="74988-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-325">Boolean</span></span>|<span data-ttu-id="74988-326">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="74988-326">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="74988-327">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="74988-327">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="74988-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-328">Boolean</span></span>|<span data-ttu-id="74988-329">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="74988-329">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="74988-330">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="74988-330">searchBlockWebResults</span></span>|<span data-ttu-id="74988-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-331">Boolean</span></span>|<span data-ttu-id="74988-332">指示是否阻止 Web 搜索。</span><span class="sxs-lookup"><span data-stu-id="74988-332">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="74988-333">findMyFiles</span><span class="sxs-lookup"><span data-stu-id="74988-333">findMyFiles</span></span>|[<span data-ttu-id="74988-334">enablement</span><span class="sxs-lookup"><span data-stu-id="74988-334">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="74988-335">控制用户能否将搜索配置为"查找我的文件"模式，该模式在辅助硬盘驱动器和用户配置文件外部搜索文件。</span><span class="sxs-lookup"><span data-stu-id="74988-335">Controls if the user can configure search to Find My Files mode, which searches files in secondary hard drives and also outside of the user profile.</span></span> <span data-ttu-id="74988-336">"查找我的文件"不允许用户搜索他们无法访问的文件或位置。</span><span class="sxs-lookup"><span data-stu-id="74988-336">Find My Files does not allow users to search files or locations to which they do not have access.</span></span> <span data-ttu-id="74988-337">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-337">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-338">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="74988-338">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="74988-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-339">Boolean</span></span>|<span data-ttu-id="74988-340">指定当设备加入 Azure AD 时，是否允许在 OOBE 期间自动加密设备 (桌面) 。</span><span class="sxs-lookup"><span data-stu-id="74988-340">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="74988-341">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="74988-341">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="74988-342">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="74988-342">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="74988-343">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="74988-343">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="74988-344">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="74988-344">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="74988-345">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="74988-345">oneDriveDisableFileSync</span></span>|<span data-ttu-id="74988-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-346">Boolean</span></span>|<span data-ttu-id="74988-347">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="74988-347">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="74988-348">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="74988-348">systemTelemetryProxyServer</span></span>|<span data-ttu-id="74988-349">String</span><span class="sxs-lookup"><span data-stu-id="74988-349">String</span></span>|<span data-ttu-id="74988-350">获取或设置代理服务器的完全限定 (FQDN) IP 地址，以转发连接用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="74988-350">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="74988-351">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="74988-351">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="74988-352">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="74988-352">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="74988-353">指定向 Microsoft 365 Analytics 发送的遥测 (类型，包括 intranet、) 和/或遥测数据。</span><span class="sxs-lookup"><span data-stu-id="74988-353">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="74988-354">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="74988-354">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="74988-355">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="74988-355">inkWorkspaceAccess</span></span>|[<span data-ttu-id="74988-356">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="74988-356">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="74988-357">控制用户从桌面和锁屏界面上方访问墨迹工作区。</span><span class="sxs-lookup"><span data-stu-id="74988-357">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="74988-358">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-358">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-359">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="74988-359">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="74988-360">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="74988-360">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="74988-361">控制用户从桌面和锁屏界面上方访问墨迹工作区。</span><span class="sxs-lookup"><span data-stu-id="74988-361">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="74988-362">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="74988-362">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="74988-363">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="74988-363">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="74988-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-364">Boolean</span></span>|<span data-ttu-id="74988-365">指定是否在墨迹工作区中显示推荐的应用建议。</span><span class="sxs-lookup"><span data-stu-id="74988-365">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="74988-366">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="74988-366">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="74988-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-367">Boolean</span></span>|<span data-ttu-id="74988-368">此属性将在 2019 年 7 月弃用，并替换为属性 SmartScreenAppInstallControl。</span><span class="sxs-lookup"><span data-stu-id="74988-368">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="74988-369">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="74988-369">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="74988-370">smartScreenAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="74988-370">smartScreenAppInstallControl</span></span>|[<span data-ttu-id="74988-371">appInstallControlType</span><span class="sxs-lookup"><span data-stu-id="74988-371">appInstallControlType</span></span>](../resources/intune-deviceconfig-appinstallcontroltype.md)|<span data-ttu-id="74988-372">在 Windows 10 版本 1703 中添加。</span><span class="sxs-lookup"><span data-stu-id="74988-372">Added in Windows 10, version 1703.</span></span> <span data-ttu-id="74988-373">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="74988-373">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span> <span data-ttu-id="74988-374">可取值为：`notConfigured`、`anywhere`、`storeOnly`、`recommendations`、`preferStore`。</span><span class="sxs-lookup"><span data-stu-id="74988-374">Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.</span></span>|
|<span data-ttu-id="74988-375">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="74988-375">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="74988-376">String</span><span class="sxs-lookup"><span data-stu-id="74988-376">String</span></span>|<span data-ttu-id="74988-377">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="74988-377">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="74988-378">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="74988-378">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="74988-379">String</span><span class="sxs-lookup"><span data-stu-id="74988-379">String</span></span>|<span data-ttu-id="74988-380">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="74988-380">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="74988-381">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="74988-381">bluetoothAllowedServices</span></span>|<span data-ttu-id="74988-382">String 集合</span><span class="sxs-lookup"><span data-stu-id="74988-382">String collection</span></span>|<span data-ttu-id="74988-383">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="74988-383">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="74988-384">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="74988-384">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="74988-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-385">Boolean</span></span>|<span data-ttu-id="74988-386">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="74988-386">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="74988-387">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="74988-387">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="74988-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-388">Boolean</span></span>|<span data-ttu-id="74988-389">是否阻止用户使用 Swift Pair 和其他基于邻近感应的方案。</span><span class="sxs-lookup"><span data-stu-id="74988-389">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="74988-390">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="74988-390">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="74988-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-391">Boolean</span></span>|<span data-ttu-id="74988-392">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="74988-392">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="74988-393">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="74988-393">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="74988-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-394">Boolean</span></span>|<span data-ttu-id="74988-395">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="74988-395">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="74988-396">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="74988-396">edgeBlockAutofill</span></span>|<span data-ttu-id="74988-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-397">Boolean</span></span>|<span data-ttu-id="74988-398">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="74988-398">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="74988-399">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-399">edgeBlocked</span></span>|<span data-ttu-id="74988-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-400">Boolean</span></span>|<span data-ttu-id="74988-401">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="74988-401">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="74988-402">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="74988-402">edgeCookiePolicy</span></span>|[<span data-ttu-id="74988-403">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="74988-403">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="74988-404">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="74988-404">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="74988-405">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="74988-405">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="74988-406">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="74988-406">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="74988-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-407">Boolean</span></span>|<span data-ttu-id="74988-408">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="74988-408">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="74988-409">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="74988-409">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="74988-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-410">Boolean</span></span>|<span data-ttu-id="74988-411">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="74988-411">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="74988-412">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="74988-412">edgeBlockExtensions</span></span>|<span data-ttu-id="74988-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-413">Boolean</span></span>|<span data-ttu-id="74988-414">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="74988-414">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="74988-415">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="74988-415">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="74988-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-416">Boolean</span></span>|<span data-ttu-id="74988-417">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="74988-417">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="74988-418">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="74988-418">edgeBlockJavaScript</span></span>|<span data-ttu-id="74988-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-419">Boolean</span></span>|<span data-ttu-id="74988-420">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="74988-420">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="74988-421">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="74988-421">edgeBlockPasswordManager</span></span>|<span data-ttu-id="74988-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-422">Boolean</span></span>|<span data-ttu-id="74988-423">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="74988-423">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="74988-424">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="74988-424">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="74988-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-425">Boolean</span></span>|<span data-ttu-id="74988-426">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="74988-426">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="74988-427">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="74988-427">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="74988-428">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="74988-428">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="74988-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-429">Boolean</span></span>|<span data-ttu-id="74988-430">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="74988-430">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="74988-431">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="74988-431">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="74988-432">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="74988-432">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="74988-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-433">Boolean</span></span>|<span data-ttu-id="74988-434">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="74988-434">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="74988-435">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="74988-435">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="74988-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-436">Boolean</span></span>|<span data-ttu-id="74988-437">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="74988-437">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="74988-438">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="74988-438">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="74988-439">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="74988-439">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="74988-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-440">Boolean</span></span>|<span data-ttu-id="74988-441">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="74988-441">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="74988-442">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="74988-442">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="74988-443">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="74988-443">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="74988-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-444">Boolean</span></span>|<span data-ttu-id="74988-445">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="74988-445">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="74988-446">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="74988-446">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="74988-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-447">Boolean</span></span>|<span data-ttu-id="74988-448">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="74988-448">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="74988-449">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="74988-449">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="74988-450">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="74988-450">edgeFavoritesListLocation</span></span>|<span data-ttu-id="74988-451">String</span><span class="sxs-lookup"><span data-stu-id="74988-451">String</span></span>|<span data-ttu-id="74988-452">要预配的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="74988-452">The location of the favorites list to provision.</span></span> <span data-ttu-id="74988-453">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="74988-453">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="74988-454">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="74988-454">edgeBlockEditFavorites</span></span>|<span data-ttu-id="74988-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-455">Boolean</span></span>|<span data-ttu-id="74988-456">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="74988-456">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="74988-457">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="74988-457">edgeNewTabPageURL</span></span>|<span data-ttu-id="74988-458">String</span><span class="sxs-lookup"><span data-stu-id="74988-458">String</span></span>|<span data-ttu-id="74988-459">指定在新建选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="74988-459">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="74988-460">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="74988-460">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="74988-461">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="74988-461">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="74988-462">使"主页"按钮隐藏、加载默认起始页、加载"新建"选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="74988-462">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="74988-463">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="74988-463">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="74988-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-464">Boolean</span></span>|<span data-ttu-id="74988-465">启用"主页"按钮配置。</span><span class="sxs-lookup"><span data-stu-id="74988-465">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="74988-466">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="74988-466">edgeOpensWith</span></span>|[<span data-ttu-id="74988-467">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="74988-467">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="74988-468">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="74988-468">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="74988-469">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="74988-469">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="74988-470">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="74988-470">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="74988-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-471">Boolean</span></span>|<span data-ttu-id="74988-472">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="74988-472">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="74988-473">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="74988-473">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="74988-474">String collection</span><span class="sxs-lookup"><span data-stu-id="74988-474">String collection</span></span>|<span data-ttu-id="74988-475">指定需要且用户无法关闭的浏览器扩展的程序包系列名称列表。</span><span class="sxs-lookup"><span data-stu-id="74988-475">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="74988-476">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="74988-476">edgeBlockPrinting</span></span>|<span data-ttu-id="74988-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-477">Boolean</span></span>|<span data-ttu-id="74988-478">配置 Edge 以允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="74988-478">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="74988-479">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="74988-479">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="74988-480">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-480">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-481">获取或设置一个值，该值指定是否将收藏夹栏设置为在任何页面上始终可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-481">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="74988-482">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-482">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-483">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="74988-483">edgeBlockSavingHistory</span></span>|<span data-ttu-id="74988-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-484">Boolean</span></span>|<span data-ttu-id="74988-485">配置 Edge 以允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="74988-485">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="74988-486">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="74988-486">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="74988-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-487">Boolean</span></span>|<span data-ttu-id="74988-488">允许或阻止 Edge 进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="74988-488">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="74988-489">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="74988-489">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="74988-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-490">Boolean</span></span>|<span data-ttu-id="74988-491">配置为在 Edge 中加载空白页，而不是默认的"新建"选项卡页，并阻止用户更改它。</span><span class="sxs-lookup"><span data-stu-id="74988-491">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="74988-492">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="74988-492">edgeBlockTabPreloading</span></span>|<span data-ttu-id="74988-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-493">Boolean</span></span>|<span data-ttu-id="74988-494">配置 Edge 是否在 Windows 启动时预加载新选项卡页。</span><span class="sxs-lookup"><span data-stu-id="74988-494">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="74988-495">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="74988-495">edgeBlockPrelaunch</span></span>|<span data-ttu-id="74988-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-496">Boolean</span></span>|<span data-ttu-id="74988-497">决定是否在 Windows 启动时预启动 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="74988-497">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="74988-498">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="74988-498">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="74988-499">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="74988-499">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="74988-500">在切换到边缘之前，控制边缘Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="74988-500">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="74988-501">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="74988-501">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="74988-502">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="74988-502">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="74988-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-503">Boolean</span></span>|<span data-ttu-id="74988-504">允许或阻止用户重写证书错误。</span><span class="sxs-lookup"><span data-stu-id="74988-504">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="74988-505">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="74988-505">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="74988-506">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="74988-506">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="74988-507">根据配置展台模式控制如何限制 Microsoft Edge 设置。</span><span class="sxs-lookup"><span data-stu-id="74988-507">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="74988-508">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="74988-508">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="74988-509">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="74988-509">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="74988-510">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-510">Int32</span></span>|<span data-ttu-id="74988-511">指定从 Microsoft Edge 展台重置之前的最后一个用户活动开始的时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="74988-511">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="74988-512">有效值为 0-1440。</span><span class="sxs-lookup"><span data-stu-id="74988-512">Valid values are 0-1440.</span></span> <span data-ttu-id="74988-513">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="74988-513">The default is 5.</span></span> <span data-ttu-id="74988-514">0 表示未重置。</span><span class="sxs-lookup"><span data-stu-id="74988-514">0 indicates no reset.</span></span> <span data-ttu-id="74988-515">有效值为 0 到 1440</span><span class="sxs-lookup"><span data-stu-id="74988-515">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="74988-516">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="74988-516">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="74988-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-517">Boolean</span></span>|<span data-ttu-id="74988-518">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="74988-518">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="74988-519">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="74988-519">cellularBlockVpn</span></span>|<span data-ttu-id="74988-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-520">Boolean</span></span>|<span data-ttu-id="74988-521">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="74988-521">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="74988-522">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="74988-522">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="74988-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-523">Boolean</span></span>|<span data-ttu-id="74988-524">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="74988-524">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="74988-525">cellularData</span><span class="sxs-lookup"><span data-stu-id="74988-525">cellularData</span></span>|[<span data-ttu-id="74988-526">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="74988-526">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="74988-527">是否允许在设备上使用手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="74988-527">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="74988-528">如果未配置，则允许手机网络数据通道，用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="74988-528">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="74988-529">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="74988-529">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="74988-530">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="74988-530">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="74988-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-531">Boolean</span></span>|<span data-ttu-id="74988-532">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="74988-532">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="74988-533">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="74988-533">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="74988-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-534">Boolean</span></span>|<span data-ttu-id="74988-535">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="74988-535">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="74988-536">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="74988-536">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="74988-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-537">Boolean</span></span>|<span data-ttu-id="74988-538">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="74988-538">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="74988-539">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="74988-539">defenderScanDownloads</span></span>|<span data-ttu-id="74988-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-540">Boolean</span></span>|<span data-ttu-id="74988-541">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="74988-541">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="74988-542">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="74988-542">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="74988-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-543">Boolean</span></span>|<span data-ttu-id="74988-544">启用后，将在计划扫描期间使用低 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="74988-544">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="74988-545">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="74988-545">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="74988-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-546">Boolean</span></span>|<span data-ttu-id="74988-547">如果阻止，将关闭计划快速扫描的跟进扫描。</span><span class="sxs-lookup"><span data-stu-id="74988-547">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="74988-548">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="74988-548">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="74988-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-549">Boolean</span></span>|<span data-ttu-id="74988-550">如果阻止，将关闭计划完整扫描的跟进扫描。</span><span class="sxs-lookup"><span data-stu-id="74988-550">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="74988-551">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="74988-551">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="74988-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-552">Boolean</span></span>|<span data-ttu-id="74988-553">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="74988-553">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="74988-554">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="74988-554">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="74988-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-555">Boolean</span></span>|<span data-ttu-id="74988-556">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="74988-556">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="74988-557">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="74988-557">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="74988-558">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-558">Int32</span></span>|<span data-ttu-id="74988-559">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="74988-559">The signature update interval in hours.</span></span> <span data-ttu-id="74988-560">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="74988-560">Specify 0 not to check.</span></span> <span data-ttu-id="74988-561">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="74988-561">Valid values 0 to 24</span></span>|
|<span data-ttu-id="74988-562">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="74988-562">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="74988-563">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="74988-563">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="74988-564">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="74988-564">Value for monitoring file activity.</span></span> <span data-ttu-id="74988-565">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="74988-565">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="74988-566">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="74988-566">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="74988-567">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-567">Int32</span></span>|<span data-ttu-id="74988-568">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="74988-568">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="74988-569">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="74988-569">Valid values 0 to 90</span></span>|
|<span data-ttu-id="74988-570">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="74988-570">defenderScanMaxCpu</span></span>|<span data-ttu-id="74988-571">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-571">Int32</span></span>|<span data-ttu-id="74988-572">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="74988-572">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="74988-573">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="74988-573">Valid values 0 to 100</span></span>|
|<span data-ttu-id="74988-574">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="74988-574">defenderScanArchiveFiles</span></span>|<span data-ttu-id="74988-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-575">Boolean</span></span>|<span data-ttu-id="74988-576">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="74988-576">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="74988-577">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="74988-577">defenderScanIncomingMail</span></span>|<span data-ttu-id="74988-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-578">Boolean</span></span>|<span data-ttu-id="74988-579">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="74988-579">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="74988-580">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="74988-580">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="74988-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-581">Boolean</span></span>|<span data-ttu-id="74988-582">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="74988-582">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="74988-583">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="74988-583">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="74988-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-584">Boolean</span></span>|<span data-ttu-id="74988-585">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="74988-585">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="74988-586">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="74988-586">defenderScanNetworkFiles</span></span>|<span data-ttu-id="74988-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-587">Boolean</span></span>|<span data-ttu-id="74988-588">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="74988-588">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="74988-589">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="74988-589">defenderRequireCloudProtection</span></span>|<span data-ttu-id="74988-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-590">Boolean</span></span>|<span data-ttu-id="74988-591">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="74988-591">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="74988-592">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="74988-592">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="74988-593">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="74988-593">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="74988-594">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="74988-594">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="74988-595">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="74988-595">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="74988-596">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="74988-596">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="74988-597">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-597">Int32</span></span>|<span data-ttu-id="74988-598">云文件扫描的超时扩展名。</span><span class="sxs-lookup"><span data-stu-id="74988-598">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="74988-599">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="74988-599">Valid values 0 to 50</span></span>|
|<span data-ttu-id="74988-600">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="74988-600">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="74988-601">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-601">Int32</span></span>|<span data-ttu-id="74988-602">云文件扫描的超时扩展名。</span><span class="sxs-lookup"><span data-stu-id="74988-602">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="74988-603">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="74988-603">Valid values 0 to 50</span></span>|
|<span data-ttu-id="74988-604">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="74988-604">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="74988-605">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="74988-605">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="74988-606">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="74988-606">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="74988-607">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="74988-607">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="74988-608">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="74988-608">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="74988-609">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="74988-609">TimeOfDay</span></span>|<span data-ttu-id="74988-610">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="74988-610">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="74988-611">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="74988-611">defenderScanType</span></span>|[<span data-ttu-id="74988-612">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="74988-612">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="74988-613">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="74988-613">The defender system scan type.</span></span> <span data-ttu-id="74988-614">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="74988-614">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="74988-615">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="74988-615">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="74988-616">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="74988-616">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="74988-617">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="74988-617">Defender day of the week for the system scan.</span></span> <span data-ttu-id="74988-618">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="74988-618">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="74988-619">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="74988-619">defenderScheduledScanTime</span></span>|<span data-ttu-id="74988-620">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="74988-620">TimeOfDay</span></span>|<span data-ttu-id="74988-621">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="74988-621">The defender time for the system scan.</span></span>|
|<span data-ttu-id="74988-622">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="74988-622">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="74988-623">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="74988-623">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="74988-624">获取或设置 Defender 对可能不需要的应用程序 (PUA) 的操作，其中包括具有广告注入行为、软件捆绑、持续付款或订阅费用等的软件。Defender 在下载 PUA 或尝试自行安装时向用户发出警报。</span><span class="sxs-lookup"><span data-stu-id="74988-624">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="74988-625">在 Windows 10 桌面版中添加。</span><span class="sxs-lookup"><span data-stu-id="74988-625">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="74988-626">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="74988-626">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="74988-627">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="74988-627">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="74988-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="74988-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="74988-629">获取或设置 Defender 对可能不需要的应用程序 (PUA) 的操作，其中包括具有广告注入行为、软件捆绑、持续付款或订阅费用等的软件。Defender 在下载 PUA 或尝试自行安装时向用户发出警报。</span><span class="sxs-lookup"><span data-stu-id="74988-629">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="74988-630">在 Windows 10 桌面版中添加。</span><span class="sxs-lookup"><span data-stu-id="74988-630">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="74988-631">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="74988-631">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="74988-632">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="74988-632">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="74988-633">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="74988-633">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="74988-634">在发送数据时检查用户Windows Defender级别。</span><span class="sxs-lookup"><span data-stu-id="74988-634">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="74988-635">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="74988-635">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="74988-636">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="74988-636">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="74988-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-637">Boolean</span></span>|<span data-ttu-id="74988-638">允许或禁止Windows Defender访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="74988-638">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="74988-639">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="74988-639">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="74988-640">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="74988-640">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="74988-641">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="74988-641">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="74988-642">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="74988-642">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="74988-643">String 集合</span><span class="sxs-lookup"><span data-stu-id="74988-643">String collection</span></span>|<span data-ttu-id="74988-644">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="74988-644">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="74988-645">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="74988-645">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="74988-646">String 集合</span><span class="sxs-lookup"><span data-stu-id="74988-646">String collection</span></span>|<span data-ttu-id="74988-647">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="74988-647">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="74988-648">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="74988-648">defenderProcessesToExclude</span></span>|<span data-ttu-id="74988-649">String 集合</span><span class="sxs-lookup"><span data-stu-id="74988-649">String collection</span></span>|<span data-ttu-id="74988-650">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="74988-650">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="74988-651">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="74988-651">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="74988-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-652">Boolean</span></span>|<span data-ttu-id="74988-653">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="74988-653">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="74988-654">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="74988-654">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="74988-655">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="74988-655">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="74988-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-656">Boolean</span></span>|<span data-ttu-id="74988-657">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="74988-657">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="74988-658">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="74988-658">lockScreenBlockCortana</span></span>|<span data-ttu-id="74988-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-659">Boolean</span></span>|<span data-ttu-id="74988-660">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="74988-660">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="74988-661">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="74988-661">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="74988-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-662">Boolean</span></span>|<span data-ttu-id="74988-663">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="74988-663">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="74988-664">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="74988-664">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="74988-665">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-665">Int32</span></span>|<span data-ttu-id="74988-666">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="74988-666">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="74988-667">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="74988-667">Supported values are 11-1800.</span></span> <span data-ttu-id="74988-668">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="74988-668">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="74988-669">lockScreenActivateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="74988-669">lockScreenActivateAppsWithVoice</span></span>|[<span data-ttu-id="74988-670">enablement</span><span class="sxs-lookup"><span data-stu-id="74988-670">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="74988-671">此策略设置指定在系统锁定时是否可以通过语音激活 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="74988-671">This policy setting specifies whether Windows apps can be activated by voice while the system is locked.</span></span> <span data-ttu-id="74988-672">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-672">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-673">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="74988-673">passwordBlockSimple</span></span>|<span data-ttu-id="74988-674">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-674">Boolean</span></span>|<span data-ttu-id="74988-675">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="74988-675">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="74988-676">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="74988-676">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="74988-677">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="74988-677">passwordExpirationDays</span></span>|<span data-ttu-id="74988-678">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-678">Int32</span></span>|<span data-ttu-id="74988-679">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="74988-679">The password expiration in days.</span></span> <span data-ttu-id="74988-680">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="74988-680">Valid values 0 to 730</span></span>|
|<span data-ttu-id="74988-681">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="74988-681">passwordMinimumLength</span></span>|<span data-ttu-id="74988-682">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-682">Int32</span></span>|<span data-ttu-id="74988-683">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="74988-683">The minimum password length.</span></span> <span data-ttu-id="74988-684">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="74988-684">Valid values 4 to 16</span></span>|
|<span data-ttu-id="74988-685">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="74988-685">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="74988-686">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-686">Int32</span></span>|<span data-ttu-id="74988-687">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="74988-687">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="74988-688">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="74988-688">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="74988-689">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-689">Int32</span></span>|<span data-ttu-id="74988-690">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="74988-690">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="74988-691">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="74988-691">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="74988-692">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-692">Int32</span></span>|<span data-ttu-id="74988-693">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="74988-693">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="74988-694">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="74988-694">Valid values 0 to 50</span></span>|
|<span data-ttu-id="74988-695">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="74988-695">passwordRequired</span></span>|<span data-ttu-id="74988-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-696">Boolean</span></span>|<span data-ttu-id="74988-697">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="74988-697">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="74988-698">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="74988-698">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="74988-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-699">Boolean</span></span>|<span data-ttu-id="74988-700">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="74988-700">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="74988-701">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="74988-701">passwordRequiredType</span></span>|[<span data-ttu-id="74988-702">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="74988-702">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="74988-703">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="74988-703">The required password type.</span></span> <span data-ttu-id="74988-704">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="74988-704">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="74988-705">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="74988-705">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="74988-706">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-706">Int32</span></span>|<span data-ttu-id="74988-707">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="74988-707">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="74988-708">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="74988-708">Valid values 0 to 999</span></span>|
|<span data-ttu-id="74988-709">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="74988-709">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="74988-710">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-710">Int32</span></span>|<span data-ttu-id="74988-711">此安全设置确定 (更改) 之前必须使用密码的时间期限（以天表示）。</span><span class="sxs-lookup"><span data-stu-id="74988-711">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="74988-712">有效值为 0 到 998</span><span class="sxs-lookup"><span data-stu-id="74988-712">Valid values 0 to 998</span></span>|
|<span data-ttu-id="74988-713">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="74988-713">privacyAdvertisingId</span></span>|[<span data-ttu-id="74988-714">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="74988-714">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="74988-715">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="74988-715">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="74988-716">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="74988-716">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="74988-717">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="74988-717">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="74988-718">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="74988-718">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="74988-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-719">Boolean</span></span>|<span data-ttu-id="74988-720">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="74988-720">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="74988-721">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="74988-721">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="74988-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-722">Boolean</span></span>|<span data-ttu-id="74988-723">此策略阻止在用户登录新用户和已升级用户期间启动隐私体验。</span><span class="sxs-lookup"><span data-stu-id="74988-723">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="74988-724">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="74988-724">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="74988-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-725">Boolean</span></span>|<span data-ttu-id="74988-726">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="74988-726">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="74988-727">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="74988-727">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="74988-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-728">Boolean</span></span>|<span data-ttu-id="74988-729">阻止任务切换器等中最近使用的资源的共享体验/发现。</span><span class="sxs-lookup"><span data-stu-id="74988-729">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="74988-730">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="74988-730">privacyBlockActivityFeed</span></span>|<span data-ttu-id="74988-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-731">Boolean</span></span>|<span data-ttu-id="74988-732">阻止使用 Cortana、听写或应用商店应用程序的基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="74988-732">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="74988-733">activateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="74988-733">activateAppsWithVoice</span></span>|[<span data-ttu-id="74988-734">enablement</span><span class="sxs-lookup"><span data-stu-id="74988-734">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="74988-735">指定是否可以通过语音激活 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="74988-735">Specifies if Windows apps can be activated by voice.</span></span> <span data-ttu-id="74988-736">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-736">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="74988-737">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="74988-737">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="74988-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-738">Boolean</span></span>|<span data-ttu-id="74988-739">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="74988-739">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="74988-740">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="74988-740">startMenuAppListVisibility</span></span>|[<span data-ttu-id="74988-741">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="74988-741">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="74988-742">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="74988-742">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="74988-743">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="74988-743">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="74988-744">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="74988-744">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="74988-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-745">Boolean</span></span>|<span data-ttu-id="74988-746">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-746">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="74988-747">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="74988-747">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="74988-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-748">Boolean</span></span>|<span data-ttu-id="74988-749">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="74988-749">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="74988-750">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="74988-750">startMenuHideHibernate</span></span>|<span data-ttu-id="74988-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-751">Boolean</span></span>|<span data-ttu-id="74988-752">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-752">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="74988-753">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="74988-753">startMenuHideLock</span></span>|<span data-ttu-id="74988-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-754">Boolean</span></span>|<span data-ttu-id="74988-755">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-755">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="74988-756">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="74988-756">startMenuHidePowerButton</span></span>|<span data-ttu-id="74988-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-757">Boolean</span></span>|<span data-ttu-id="74988-758">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-758">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="74988-759">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="74988-759">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="74988-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-760">Boolean</span></span>|<span data-ttu-id="74988-761">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="74988-761">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="74988-762">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="74988-762">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="74988-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-763">Boolean</span></span>|<span data-ttu-id="74988-764">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="74988-764">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="74988-765">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="74988-765">startMenuHideRestartOptions</span></span>|<span data-ttu-id="74988-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-766">Boolean</span></span>|<span data-ttu-id="74988-767">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-767">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="74988-768">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="74988-768">startMenuHideShutDown</span></span>|<span data-ttu-id="74988-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-769">Boolean</span></span>|<span data-ttu-id="74988-770">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-770">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="74988-771">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="74988-771">startMenuHideSignOut</span></span>|<span data-ttu-id="74988-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-772">Boolean</span></span>|<span data-ttu-id="74988-773">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-773">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="74988-774">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="74988-774">startMenuHideSleep</span></span>|<span data-ttu-id="74988-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-775">Boolean</span></span>|<span data-ttu-id="74988-776">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-776">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="74988-777">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="74988-777">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="74988-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-778">Boolean</span></span>|<span data-ttu-id="74988-779">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-779">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="74988-780">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="74988-780">startMenuHideUserTile</span></span>|<span data-ttu-id="74988-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-781">Boolean</span></span>|<span data-ttu-id="74988-782">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="74988-782">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="74988-783">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="74988-783">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="74988-784">Binary</span><span class="sxs-lookup"><span data-stu-id="74988-784">Binary</span></span>|<span data-ttu-id="74988-785">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="74988-785">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="74988-786">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="74988-786">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="74988-787">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="74988-787">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="74988-788">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="74988-788">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="74988-789">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="74988-789">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="74988-790">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="74988-790">startMenuLayoutXml</span></span>|<span data-ttu-id="74988-791">Binary</span><span class="sxs-lookup"><span data-stu-id="74988-791">Binary</span></span>|<span data-ttu-id="74988-792">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="74988-792">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="74988-793">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="74988-793">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="74988-794">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="74988-794">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="74988-795">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="74988-795">startMenuMode</span></span>|[<span data-ttu-id="74988-796">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="74988-796">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="74988-797">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="74988-797">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="74988-798">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="74988-798">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="74988-799">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="74988-799">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="74988-800">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-800">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-801">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-801">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-802">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-802">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-803">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="74988-803">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="74988-804">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-804">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-805">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-805">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-806">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-806">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-807">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="74988-807">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="74988-808">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-808">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-809">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-809">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="74988-810">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-810">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-811">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="74988-811">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="74988-812">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-812">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-813">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-813">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-814">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-814">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-815">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="74988-815">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="74988-816">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-816">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-817">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-817">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-818">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-818">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-819">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="74988-819">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="74988-820">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-820">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-821">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-821">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-822">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-822">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-823">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="74988-823">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="74988-824">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-824">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-825">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-825">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-826">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-826">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-827">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="74988-827">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="74988-828">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-828">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-829">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-829">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-830">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-830">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-831">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="74988-831">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="74988-832">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-832">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-833">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-833">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-834">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-834">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-835">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="74988-835">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="74988-836">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="74988-836">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="74988-837">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="74988-837">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="74988-838">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="74988-838">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="74988-839">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="74988-839">settingsBlockSettingsApp</span></span>|<span data-ttu-id="74988-840">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-840">Boolean</span></span>|<span data-ttu-id="74988-841">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="74988-841">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="74988-842">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="74988-842">settingsBlockSystemPage</span></span>|<span data-ttu-id="74988-843">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-843">Boolean</span></span>|<span data-ttu-id="74988-844">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="74988-844">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="74988-845">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="74988-845">settingsBlockDevicesPage</span></span>|<span data-ttu-id="74988-846">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-846">Boolean</span></span>|<span data-ttu-id="74988-847">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="74988-847">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="74988-848">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="74988-848">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="74988-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-849">Boolean</span></span>|<span data-ttu-id="74988-850">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="74988-850">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="74988-851">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="74988-851">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="74988-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-852">Boolean</span></span>|<span data-ttu-id="74988-853">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="74988-853">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="74988-854">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="74988-854">settingsBlockAccountsPage</span></span>|<span data-ttu-id="74988-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-855">Boolean</span></span>|<span data-ttu-id="74988-856">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="74988-856">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="74988-857">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="74988-857">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="74988-858">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-858">Boolean</span></span>|<span data-ttu-id="74988-859">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="74988-859">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="74988-860">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="74988-860">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="74988-861">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-861">Boolean</span></span>|<span data-ttu-id="74988-862">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="74988-862">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="74988-863">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="74988-863">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="74988-864">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-864">Boolean</span></span>|<span data-ttu-id="74988-865">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="74988-865">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="74988-866">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="74988-866">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="74988-867">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-867">Boolean</span></span>|<span data-ttu-id="74988-868">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="74988-868">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="74988-869">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="74988-869">settingsBlockAppsPage</span></span>|<span data-ttu-id="74988-870">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-870">Boolean</span></span>|<span data-ttu-id="74988-871">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="74988-871">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="74988-872">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="74988-872">settingsBlockGamingPage</span></span>|<span data-ttu-id="74988-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-873">Boolean</span></span>|<span data-ttu-id="74988-874">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="74988-874">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="74988-875">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="74988-875">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="74988-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-876">Boolean</span></span>|<span data-ttu-id="74988-877">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="74988-877">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="74988-878">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-878">windowsSpotlightBlocked</span></span>|<span data-ttu-id="74988-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-879">Boolean</span></span>|<span data-ttu-id="74988-880">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="74988-880">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="74988-881">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="74988-881">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="74988-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-882">Boolean</span></span>|<span data-ttu-id="74988-883">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="74988-883">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="74988-884">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="74988-884">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="74988-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-885">Boolean</span></span>|<span data-ttu-id="74988-886">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="74988-886">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="74988-887">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="74988-887">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="74988-888">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-888">Boolean</span></span>|<span data-ttu-id="74988-889">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="74988-889">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="74988-890">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="74988-890">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="74988-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-891">Boolean</span></span>|<span data-ttu-id="74988-892">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="74988-892">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="74988-893">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="74988-893">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="74988-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-894">Boolean</span></span>|<span data-ttu-id="74988-895">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="74988-895">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="74988-896">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="74988-896">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="74988-897">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="74988-897">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="74988-898">指定聚焦的类型。</span><span class="sxs-lookup"><span data-stu-id="74988-898">Specifies the type of Spotlight.</span></span> <span data-ttu-id="74988-899">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="74988-899">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="74988-900">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="74988-900">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="74988-901">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-901">Boolean</span></span>|<span data-ttu-id="74988-902">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="74988-902">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="74988-903">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="74988-903">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="74988-904">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="74988-904">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="74988-905">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-905">Boolean</span></span>|<span data-ttu-id="74988-906">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="74988-906">Disable automatic detection of settings.</span></span> <span data-ttu-id="74988-907">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="74988-907">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="74988-908">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="74988-908">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="74988-909">String</span><span class="sxs-lookup"><span data-stu-id="74988-909">String</span></span>|<span data-ttu-id="74988-910">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="74988-910">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="74988-911">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="74988-911">networkProxyServer</span></span>|[<span data-ttu-id="74988-912">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="74988-912">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="74988-913">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="74988-913">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="74988-914">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="74988-914">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="74988-915">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-915">Boolean</span></span>|<span data-ttu-id="74988-916">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="74988-916">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="74988-917">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-917">antiTheftModeBlocked</span></span>|<span data-ttu-id="74988-918">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-918">Boolean</span></span>|<span data-ttu-id="74988-919">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="74988-919">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="74988-920">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-920">bluetoothBlocked</span></span>|<span data-ttu-id="74988-921">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-921">Boolean</span></span>|<span data-ttu-id="74988-922">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="74988-922">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="74988-923">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-923">cameraBlocked</span></span>|<span data-ttu-id="74988-924">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-924">Boolean</span></span>|<span data-ttu-id="74988-925">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="74988-925">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="74988-926">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-926">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="74988-927">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-927">Boolean</span></span>|<span data-ttu-id="74988-928">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="74988-928">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="74988-929">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="74988-929">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="74988-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-930">Boolean</span></span>|<span data-ttu-id="74988-931">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="74988-931">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="74988-932">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-932">copyPasteBlocked</span></span>|<span data-ttu-id="74988-933">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-933">Boolean</span></span>|<span data-ttu-id="74988-934">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="74988-934">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="74988-935">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-935">cortanaBlocked</span></span>|<span data-ttu-id="74988-936">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-936">Boolean</span></span>|<span data-ttu-id="74988-937">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="74988-937">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="74988-938">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="74988-938">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="74988-939">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-939">Boolean</span></span>|<span data-ttu-id="74988-940">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="74988-940">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="74988-941">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="74988-941">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="74988-942">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-942">Boolean</span></span>|<span data-ttu-id="74988-943">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="74988-943">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="74988-944">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="74988-944">safeSearchFilter</span></span>|[<span data-ttu-id="74988-945">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="74988-945">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="74988-946">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="74988-946">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="74988-947">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="74988-947">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="74988-948">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="74988-948">edgeBlockPopups</span></span>|<span data-ttu-id="74988-949">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-949">Boolean</span></span>|<span data-ttu-id="74988-950">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="74988-950">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="74988-951">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="74988-951">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="74988-952">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-952">Boolean</span></span>|<span data-ttu-id="74988-953">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="74988-953">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="74988-954">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="74988-954">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="74988-955">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-955">Boolean</span></span>|<span data-ttu-id="74988-956">指示是否阻止用户添加新搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="74988-956">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="74988-957">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="74988-957">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="74988-958">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-958">Boolean</span></span>|<span data-ttu-id="74988-959">指示是否将 Intranet 流量从 Edge 切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="74988-959">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="74988-960">注意：此属性的名称令人误解;属性已过时，请改为使用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="74988-960">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="74988-961">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="74988-961">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="74988-962">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-962">Boolean</span></span>|<span data-ttu-id="74988-963">指示是否将 Intranet 流量从 Edge 切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="74988-963">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="74988-964">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="74988-964">edgeRequireSmartScreen</span></span>|<span data-ttu-id="74988-965">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-965">Boolean</span></span>|<span data-ttu-id="74988-966">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="74988-966">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="74988-967">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="74988-967">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="74988-968">String</span><span class="sxs-lookup"><span data-stu-id="74988-968">String</span></span>|<span data-ttu-id="74988-969">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="74988-969">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="74988-970">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="74988-970">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="74988-971">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="74988-971">edgeFirstRunUrl</span></span>|<span data-ttu-id="74988-972">String</span><span class="sxs-lookup"><span data-stu-id="74988-972">String</span></span>|<span data-ttu-id="74988-973">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="74988-973">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="74988-974">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="74988-974">edgeSearchEngine</span></span>|[<span data-ttu-id="74988-975">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="74988-975">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="74988-976">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="74988-976">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="74988-977">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="74988-977">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="74988-978">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="74988-978">edgeHomepageUrls</span></span>|<span data-ttu-id="74988-979">String 集合</span><span class="sxs-lookup"><span data-stu-id="74988-979">String collection</span></span>|<span data-ttu-id="74988-980">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="74988-980">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="74988-981">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="74988-981">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="74988-982">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-982">Boolean</span></span>|<span data-ttu-id="74988-983">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="74988-983">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="74988-984">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="74988-984">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="74988-985">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-985">Boolean</span></span>|<span data-ttu-id="74988-986">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="74988-986">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="74988-987">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="74988-987">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="74988-988">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-988">Boolean</span></span>|<span data-ttu-id="74988-989">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="74988-989">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="74988-990">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="74988-990">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="74988-991">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-991">Boolean</span></span>|<span data-ttu-id="74988-992">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="74988-992">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="74988-993">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-993">internetSharingBlocked</span></span>|<span data-ttu-id="74988-994">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-994">Boolean</span></span>|<span data-ttu-id="74988-995">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="74988-995">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="74988-996">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="74988-996">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="74988-997">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-997">Boolean</span></span>|<span data-ttu-id="74988-998">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="74988-998">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="74988-999">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="74988-999">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="74988-1000">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1000">Boolean</span></span>|<span data-ttu-id="74988-1001">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="74988-1001">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="74988-1002">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="74988-1002">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="74988-1003">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1003">Boolean</span></span>|<span data-ttu-id="74988-1004">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="74988-1004">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="74988-1005">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="74988-1005">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="74988-1006">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1006">Boolean</span></span>|<span data-ttu-id="74988-1007">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="74988-1007">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="74988-1008">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="74988-1008">settingsBlockChangeRegion</span></span>|<span data-ttu-id="74988-1009">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1009">Boolean</span></span>|<span data-ttu-id="74988-1010">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="74988-1010">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="74988-1011">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="74988-1011">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="74988-1012">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1012">Boolean</span></span>|<span data-ttu-id="74988-1013">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="74988-1013">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="74988-1014">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="74988-1014">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="74988-1015">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1015">Boolean</span></span>|<span data-ttu-id="74988-1016">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="74988-1016">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="74988-1017">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1017">locationServicesBlocked</span></span>|<span data-ttu-id="74988-1018">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1018">Boolean</span></span>|<span data-ttu-id="74988-1019">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="74988-1019">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="74988-1020">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1020">microsoftAccountBlocked</span></span>|<span data-ttu-id="74988-1021">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1021">Boolean</span></span>|<span data-ttu-id="74988-1022">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="74988-1022">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="74988-1023">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="74988-1023">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="74988-1024">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1024">Boolean</span></span>|<span data-ttu-id="74988-1025">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="74988-1025">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="74988-1026">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1026">nfcBlocked</span></span>|<span data-ttu-id="74988-1027">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1027">Boolean</span></span>|<span data-ttu-id="74988-1028">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="74988-1028">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="74988-1029">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1029">resetProtectionModeBlocked</span></span>|<span data-ttu-id="74988-1030">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1030">Boolean</span></span>|<span data-ttu-id="74988-1031">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="74988-1031">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="74988-1032">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1032">screenCaptureBlocked</span></span>|<span data-ttu-id="74988-1033">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1033">Boolean</span></span>|<span data-ttu-id="74988-1034">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="74988-1034">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="74988-1035">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="74988-1035">storageBlockRemovableStorage</span></span>|<span data-ttu-id="74988-1036">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1036">Boolean</span></span>|<span data-ttu-id="74988-1037">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="74988-1037">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="74988-1038">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="74988-1038">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="74988-1039">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1039">Boolean</span></span>|<span data-ttu-id="74988-1040">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="74988-1040">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="74988-1041">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1041">usbBlocked</span></span>|<span data-ttu-id="74988-1042">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1042">Boolean</span></span>|<span data-ttu-id="74988-1043">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="74988-1043">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="74988-1044">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1044">voiceRecordingBlocked</span></span>|<span data-ttu-id="74988-1045">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1045">Boolean</span></span>|<span data-ttu-id="74988-1046">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="74988-1046">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="74988-1047">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="74988-1047">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="74988-1048">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1048">Boolean</span></span>|<span data-ttu-id="74988-1049">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="74988-1049">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="74988-1050">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="74988-1050">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="74988-1051">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1051">wiFiBlocked</span></span>|<span data-ttu-id="74988-1052">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1052">Boolean</span></span>|<span data-ttu-id="74988-1053">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="74988-1053">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="74988-1054">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="74988-1054">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="74988-1055">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1055">Boolean</span></span>|<span data-ttu-id="74988-1056">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="74988-1056">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="74988-1057">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="74988-1057">wiFiScanInterval</span></span>|<span data-ttu-id="74988-1058">Int32</span><span class="sxs-lookup"><span data-stu-id="74988-1058">Int32</span></span>|<span data-ttu-id="74988-1059">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="74988-1059">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="74988-1060">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="74988-1060">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="74988-1061">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="74988-1061">Valid values 1 to 500</span></span>|
|<span data-ttu-id="74988-1062">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="74988-1062">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="74988-1063">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1063">Boolean</span></span>|<span data-ttu-id="74988-1064">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="74988-1064">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="74988-1065">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="74988-1065">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="74988-1066">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1066">Boolean</span></span>|<span data-ttu-id="74988-1067">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="74988-1067">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="74988-1068">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="74988-1068">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="74988-1069">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1069">Boolean</span></span>|<span data-ttu-id="74988-1070">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="74988-1070">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="74988-1071">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1071">windowsStoreBlocked</span></span>|<span data-ttu-id="74988-1072">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1072">Boolean</span></span>|<span data-ttu-id="74988-1073">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="74988-1073">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="74988-1074">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="74988-1074">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="74988-1075">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="74988-1075">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="74988-1076">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="74988-1076">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="74988-1077">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="74988-1077">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="74988-1078">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="74988-1078">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="74988-1079">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1079">Boolean</span></span>|<span data-ttu-id="74988-1080">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="74988-1080">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="74988-1081">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="74988-1081">developerUnlockSetting</span></span>|[<span data-ttu-id="74988-1082">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="74988-1082">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="74988-1083">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="74988-1083">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="74988-1084">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="74988-1084">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="74988-1085">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="74988-1085">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="74988-1086">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1086">Boolean</span></span>|<span data-ttu-id="74988-1087">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="74988-1087">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="74988-1088">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="74988-1088">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="74988-1089">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1089">Boolean</span></span>|<span data-ttu-id="74988-1090">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="74988-1090">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="74988-1091">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="74988-1091">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="74988-1092">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1092">Boolean</span></span>|<span data-ttu-id="74988-1093">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="74988-1093">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="74988-1094">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="74988-1094">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="74988-1095">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1095">Boolean</span></span>|<span data-ttu-id="74988-1096">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="74988-1096">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="74988-1097">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="74988-1097">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="74988-1098">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1098">Boolean</span></span>|<span data-ttu-id="74988-1099">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="74988-1099">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="74988-1100">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="74988-1100">gameDvrBlocked</span></span>|<span data-ttu-id="74988-1101">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1101">Boolean</span></span>|<span data-ttu-id="74988-1102">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="74988-1102">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="74988-1103">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="74988-1103">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="74988-1104">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1104">Boolean</span></span>|<span data-ttu-id="74988-1105">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="74988-1105">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="74988-1106">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="74988-1106">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="74988-1107">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1107">Boolean</span></span>|<span data-ttu-id="74988-1108">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="74988-1108">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="74988-1109">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="74988-1109">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="74988-1110">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1110">Boolean</span></span>|<span data-ttu-id="74988-1111">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="74988-1111">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="74988-1112">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="74988-1112">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="74988-1113">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1113">Boolean</span></span>|<span data-ttu-id="74988-1114">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="74988-1114">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="74988-1115">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="74988-1115">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="74988-1116">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1116">Boolean</span></span>|<span data-ttu-id="74988-1117">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="74988-1117">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="74988-1118">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="74988-1118">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="74988-1119">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1119">Boolean</span></span>|<span data-ttu-id="74988-1120">此策略设置允许用户更改通常仅对系统管理员可用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="74988-1120">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="74988-1121">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="74988-1121">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="74988-1122">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1122">Boolean</span></span>|<span data-ttu-id="74988-1123">此策略设置指示 Windows Installer 在系统安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="74988-1123">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="74988-1124">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="74988-1124">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="74988-1125">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1125">Boolean</span></span>|<span data-ttu-id="74988-1126">此策略设置允许你阻止所有可 (PCI) 端口的 DMA 直接内存访问，直到用户登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="74988-1126">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="74988-1127">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="74988-1127">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="74988-1128">String collection</span><span class="sxs-lookup"><span data-stu-id="74988-1128">String collection</span></span>|<span data-ttu-id="74988-1129">以分号分隔的 Windows 应用的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="74988-1129">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="74988-1130">列出的 Windows 应用将在登录后启动。</span><span class="sxs-lookup"><span data-stu-id="74988-1130">Listed Windows apps are to be launched after logon.</span></span>|
|<span data-ttu-id="74988-1131">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="74988-1131">uninstallBuiltInApps</span></span>|<span data-ttu-id="74988-1132">Boolean</span><span class="sxs-lookup"><span data-stu-id="74988-1132">Boolean</span></span>|<span data-ttu-id="74988-1133">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="74988-1133">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|
|<span data-ttu-id="74988-1134">configureTimeZone</span><span class="sxs-lookup"><span data-stu-id="74988-1134">configureTimeZone</span></span>|<span data-ttu-id="74988-1135">String</span><span class="sxs-lookup"><span data-stu-id="74988-1135">String</span></span>|<span data-ttu-id="74988-1136">指定要应用于设备的时区。</span><span class="sxs-lookup"><span data-stu-id="74988-1136">Specifies the time zone to be applied to the device.</span></span> <span data-ttu-id="74988-1137">这是目标时区的标准 Windows 名称。</span><span class="sxs-lookup"><span data-stu-id="74988-1137">This is the standard Windows name for the target time zone.</span></span>|



## <a name="response"></a><span data-ttu-id="74988-1138">响应</span><span class="sxs-lookup"><span data-stu-id="74988-1138">Response</span></span>
<span data-ttu-id="74988-1139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74988-1139">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74988-1140">示例</span><span class="sxs-lookup"><span data-stu-id="74988-1140">Example</span></span>

### <a name="request"></a><span data-ttu-id="74988-1141">请求</span><span class="sxs-lookup"><span data-stu-id="74988-1141">Request</span></span>
<span data-ttu-id="74988-1142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74988-1142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 15009

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "taskManagerBlockEndTask": true,
  "energySaverOnBatteryThresholdPercentage": 7,
  "energySaverPluggedInThresholdPercentage": 7,
  "powerLidCloseActionOnBattery": "noAction",
  "powerLidCloseActionPluggedIn": "noAction",
  "powerButtonActionOnBattery": "noAction",
  "powerButtonActionPluggedIn": "noAction",
  "powerSleepButtonActionOnBattery": "noAction",
  "powerSleepButtonActionPluggedIn": "noAction",
  "powerHybridSleepOnBattery": "enabled",
  "powerHybridSleepPluggedIn": "enabled",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "findMyFiles": "enabled",
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderBlockOnAccessProtection": true,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "activateAppsWithVoice": "enabled",
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ],
  "uninstallBuiltInApps": true,
  "configureTimeZone": "Configure Time Zone value"
}
```

### <a name="response"></a><span data-ttu-id="74988-1143">响应</span><span class="sxs-lookup"><span data-stu-id="74988-1143">Response</span></span>
<span data-ttu-id="74988-p199">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74988-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 15181

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
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
  "taskManagerBlockEndTask": true,
  "energySaverOnBatteryThresholdPercentage": 7,
  "energySaverPluggedInThresholdPercentage": 7,
  "powerLidCloseActionOnBattery": "noAction",
  "powerLidCloseActionPluggedIn": "noAction",
  "powerButtonActionOnBattery": "noAction",
  "powerButtonActionPluggedIn": "noAction",
  "powerSleepButtonActionOnBattery": "noAction",
  "powerSleepButtonActionPluggedIn": "noAction",
  "powerHybridSleepOnBattery": "enabled",
  "powerHybridSleepPluggedIn": "enabled",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "findMyFiles": "enabled",
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderBlockOnAccessProtection": true,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "activateAppsWithVoice": "enabled",
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ],
  "uninstallBuiltInApps": true,
  "configureTimeZone": "Configure Time Zone value"
}
```




