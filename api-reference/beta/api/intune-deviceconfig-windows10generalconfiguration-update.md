---
title: 更新 windows10GeneralConfiguration
description: 更新 windows10GeneralConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e7a1e82fa3e4413e83dc64f9b5652d8f6194289
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947426"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="584de-103">更新 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="584de-103">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="584de-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="584de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="584de-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="584de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="584de-106">更新 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="584de-106">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="584de-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="584de-107">Prerequisites</span></span>
<span data-ttu-id="584de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="584de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="584de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="584de-110">Permission type</span></span>|<span data-ttu-id="584de-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="584de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="584de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="584de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="584de-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584de-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="584de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="584de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="584de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="584de-115">Not supported.</span></span>|
|<span data-ttu-id="584de-116">Application</span><span class="sxs-lookup"><span data-stu-id="584de-116">Application</span></span>|<span data-ttu-id="584de-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584de-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="584de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="584de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="584de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="584de-119">Request headers</span></span>
|<span data-ttu-id="584de-120">标头</span><span class="sxs-lookup"><span data-stu-id="584de-120">Header</span></span>|<span data-ttu-id="584de-121">值</span><span class="sxs-lookup"><span data-stu-id="584de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="584de-122">授权</span><span class="sxs-lookup"><span data-stu-id="584de-122">Authorization</span></span>|<span data-ttu-id="584de-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="584de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="584de-124">接受</span><span class="sxs-lookup"><span data-stu-id="584de-124">Accept</span></span>|<span data-ttu-id="584de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="584de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="584de-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="584de-126">Request body</span></span>
<span data-ttu-id="584de-127">在请求正文中，提供 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="584de-127">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="584de-128">下表显示了创建 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="584de-128">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="584de-129">属性</span><span class="sxs-lookup"><span data-stu-id="584de-129">Property</span></span>|<span data-ttu-id="584de-130">类型</span><span class="sxs-lookup"><span data-stu-id="584de-130">Type</span></span>|<span data-ttu-id="584de-131">说明</span><span class="sxs-lookup"><span data-stu-id="584de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="584de-132">id</span><span class="sxs-lookup"><span data-stu-id="584de-132">id</span></span>|<span data-ttu-id="584de-133">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-133">String</span></span>|<span data-ttu-id="584de-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="584de-134">Key of the entity.</span></span> <span data-ttu-id="584de-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="584de-136">lastModifiedDateTime</span></span>|<span data-ttu-id="584de-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="584de-137">DateTimeOffset</span></span>|<span data-ttu-id="584de-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="584de-138">DateTime the object was last modified.</span></span> <span data-ttu-id="584de-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="584de-140">roleScopeTagIds</span></span>|<span data-ttu-id="584de-141">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-141">String collection</span></span>|<span data-ttu-id="584de-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="584de-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="584de-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="584de-144">supportsScopeTags</span></span>|<span data-ttu-id="584de-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-145">Boolean</span></span>|<span data-ttu-id="584de-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="584de-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="584de-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="584de-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="584de-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="584de-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="584de-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="584de-149">This property is read-only.</span></span> <span data-ttu-id="584de-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="584de-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="584de-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="584de-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="584de-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="584de-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="584de-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="584de-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="584de-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="584de-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="584de-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="584de-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="584de-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="584de-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="584de-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="584de-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="584de-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="584de-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="584de-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="584de-163">createdDateTime</span></span>|<span data-ttu-id="584de-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="584de-164">DateTimeOffset</span></span>|<span data-ttu-id="584de-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="584de-165">DateTime the object was created.</span></span> <span data-ttu-id="584de-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-167">说明</span><span class="sxs-lookup"><span data-stu-id="584de-167">description</span></span>|<span data-ttu-id="584de-168">String</span><span class="sxs-lookup"><span data-stu-id="584de-168">String</span></span>|<span data-ttu-id="584de-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="584de-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="584de-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-171">displayName</span><span class="sxs-lookup"><span data-stu-id="584de-171">displayName</span></span>|<span data-ttu-id="584de-172">String</span><span class="sxs-lookup"><span data-stu-id="584de-172">String</span></span>|<span data-ttu-id="584de-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="584de-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="584de-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-175">version</span><span class="sxs-lookup"><span data-stu-id="584de-175">version</span></span>|<span data-ttu-id="584de-176">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-176">Int32</span></span>|<span data-ttu-id="584de-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="584de-177">Version of the device configuration.</span></span> <span data-ttu-id="584de-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="584de-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="584de-179">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="584de-179">taskManagerBlockEndTask</span></span>|<span data-ttu-id="584de-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-180">Boolean</span></span>|<span data-ttu-id="584de-181">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="584de-181">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="584de-182">energySaverOnBatteryThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="584de-182">energySaverOnBatteryThresholdPercentage</span></span>|<span data-ttu-id="584de-183">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-183">Int32</span></span>|<span data-ttu-id="584de-184">此设置允许您指定节能程序打开时的电池电量水平。</span><span class="sxs-lookup"><span data-stu-id="584de-184">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="584de-185">在使用电池时，将自动打开（和低于）指定电池电量级别的节能保护程序。</span><span class="sxs-lookup"><span data-stu-id="584de-185">While on battery, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="584de-186">有效的输入范围（0-100）。</span><span class="sxs-lookup"><span data-stu-id="584de-186">Valid input range (0-100).</span></span> <span data-ttu-id="584de-187">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="584de-187">Valid values 0 to 100</span></span>|
|<span data-ttu-id="584de-188">energySaverPluggedInThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="584de-188">energySaverPluggedInThresholdPercentage</span></span>|<span data-ttu-id="584de-189">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-189">Int32</span></span>|<span data-ttu-id="584de-190">此设置允许您指定节能程序打开时的电池电量水平。</span><span class="sxs-lookup"><span data-stu-id="584de-190">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="584de-191">接通电源时，将自动打开（和低于）指定电池电量级别的节能保护程序。</span><span class="sxs-lookup"><span data-stu-id="584de-191">While plugged in, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="584de-192">有效的输入范围（0-100）。</span><span class="sxs-lookup"><span data-stu-id="584de-192">Valid input range (0-100).</span></span> <span data-ttu-id="584de-193">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="584de-193">Valid values 0 to 100</span></span>|
|<span data-ttu-id="584de-194">powerLidCloseActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="584de-194">powerLidCloseActionOnBattery</span></span>|[<span data-ttu-id="584de-195">powerActionType</span><span class="sxs-lookup"><span data-stu-id="584de-195">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="584de-196">此设置指定当用户在使用电池时关闭移动电脑上的盖子时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="584de-196">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while on battery.</span></span> <span data-ttu-id="584de-197">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="584de-197">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="584de-198">powerLidCloseActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="584de-198">powerLidCloseActionPluggedIn</span></span>|[<span data-ttu-id="584de-199">powerActionType</span><span class="sxs-lookup"><span data-stu-id="584de-199">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="584de-200">此设置指定当用户在插入时关闭移动 PC 上的盖子时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="584de-200">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while plugged in.</span></span> <span data-ttu-id="584de-201">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="584de-201">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="584de-202">powerButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="584de-202">powerButtonActionOnBattery</span></span>|[<span data-ttu-id="584de-203">powerActionType</span><span class="sxs-lookup"><span data-stu-id="584de-203">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="584de-204">此设置指定当用户在使用电池时按下电源按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="584de-204">This setting specifies the action that Windows takes when a user presses the Power button while on battery.</span></span> <span data-ttu-id="584de-205">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="584de-205">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="584de-206">powerButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="584de-206">powerButtonActionPluggedIn</span></span>|[<span data-ttu-id="584de-207">powerActionType</span><span class="sxs-lookup"><span data-stu-id="584de-207">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="584de-208">此设置指定当用户在插入时按下电源按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="584de-208">This setting specifies the action that Windows takes when a user presses the Power button while plugged in.</span></span> <span data-ttu-id="584de-209">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="584de-209">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="584de-210">powerSleepButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="584de-210">powerSleepButtonActionOnBattery</span></span>|[<span data-ttu-id="584de-211">powerActionType</span><span class="sxs-lookup"><span data-stu-id="584de-211">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="584de-212">此设置指定当用户在使用电池时按 "睡眠" 按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="584de-212">This setting specifies the action that Windows takes when a user presses the Sleep button while on battery.</span></span> <span data-ttu-id="584de-213">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="584de-213">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="584de-214">powerSleepButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="584de-214">powerSleepButtonActionPluggedIn</span></span>|[<span data-ttu-id="584de-215">powerActionType</span><span class="sxs-lookup"><span data-stu-id="584de-215">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="584de-216">此设置指定当用户在插入时按 "睡眠" 按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="584de-216">This setting specifies the action that Windows takes when a user presses the Sleep button while plugged in.</span></span> <span data-ttu-id="584de-217">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="584de-217">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="584de-218">powerHybridSleepOnBattery</span><span class="sxs-lookup"><span data-stu-id="584de-218">powerHybridSleepOnBattery</span></span>|[<span data-ttu-id="584de-219">启用</span><span class="sxs-lookup"><span data-stu-id="584de-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="584de-220">通过此设置，可以在使用电池时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="584de-220">This setting allows you to turn off hybrid sleep while on battery.</span></span> <span data-ttu-id="584de-221">如果将此设置设置为禁用，则当系统转换为睡眠（待机）时不会生成 hiberfile。</span><span class="sxs-lookup"><span data-stu-id="584de-221">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="584de-222">如果将此设置设置为启用或未配置此策略设置，则用户将控制此设置。</span><span class="sxs-lookup"><span data-stu-id="584de-222">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="584de-223">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-223">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="584de-224">powerHybridSleepPluggedIn</span><span class="sxs-lookup"><span data-stu-id="584de-224">powerHybridSleepPluggedIn</span></span>|[<span data-ttu-id="584de-225">启用</span><span class="sxs-lookup"><span data-stu-id="584de-225">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="584de-226">此设置允许你在接通电源时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="584de-226">This setting allows you to turn off hybrid sleep while plugged in.</span></span> <span data-ttu-id="584de-227">如果将此设置设置为禁用，则当系统转换为睡眠（待机）时不会生成 hiberfile。</span><span class="sxs-lookup"><span data-stu-id="584de-227">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="584de-228">如果将此设置设置为启用或未配置此策略设置，则用户将控制此设置。</span><span class="sxs-lookup"><span data-stu-id="584de-228">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="584de-229">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-229">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="584de-230">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="584de-230">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="584de-231">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="584de-231">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="584de-232">应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="584de-232">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="584de-233">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="584de-233">enableAutomaticRedeployment</span></span>|<span data-ttu-id="584de-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-234">Boolean</span></span>|<span data-ttu-id="584de-235">允许具有管理权限的用户在设备锁屏的屏幕上使用 CTRL + Win + R 删除所有用户数据和设置，以便可以自动重新配置设备并将其重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="584de-235">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="584de-236">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="584de-236">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="584de-237">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="584de-237">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="584de-238">控制 Microsoft 帐户登录助手（wlidsvc） NT 服务。</span><span class="sxs-lookup"><span data-stu-id="584de-238">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="584de-239">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-239">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="584de-240">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="584de-240">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="584de-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-241">Boolean</span></span>|<span data-ttu-id="584de-242">允许辅助身份验证设备使用 Windows。</span><span class="sxs-lookup"><span data-stu-id="584de-242">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="584de-243">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="584de-243">authenticationWebSignIn</span></span>|[<span data-ttu-id="584de-244">启用</span><span class="sxs-lookup"><span data-stu-id="584de-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="584de-245">指示是否将启用 Web 凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="584de-245">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="584de-246">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="584de-247">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="584de-247">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="584de-248">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-248">String</span></span>|<span data-ttu-id="584de-249">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="584de-249">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="584de-250">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="584de-250">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="584de-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-251">Boolean</span></span>|<span data-ttu-id="584de-252">指定是否允许或禁止联邦信息处理标准（FIPS）策略。</span><span class="sxs-lookup"><span data-stu-id="584de-252">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="584de-253">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="584de-253">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="584de-254">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-254">String collection</span></span>|<span data-ttu-id="584de-255">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="584de-255">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="584de-256">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="584de-256">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="584de-257">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-257">String collection</span></span>|<span data-ttu-id="584de-258">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="584de-258">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="584de-259">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="584de-259">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="584de-260">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-260">String</span></span>|<span data-ttu-id="584de-261">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="584de-261">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="584de-262">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="584de-262">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="584de-263">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-263">String</span></span>|<span data-ttu-id="584de-264">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="584de-264">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="584de-265">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="584de-265">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="584de-266">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-266">String</span></span>|<span data-ttu-id="584de-267">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="584de-267">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="584de-268">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="584de-268">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="584de-269">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-269">String</span></span>|<span data-ttu-id="584de-270">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="584de-270">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="584de-271">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="584de-271">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="584de-272">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-272">Int32</span></span>|<span data-ttu-id="584de-273">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="584de-273">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="584de-274">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="584de-274">This is a mobile only setting.</span></span> <span data-ttu-id="584de-275">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="584de-275">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="584de-276">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="584de-276">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="584de-277">String</span><span class="sxs-lookup"><span data-stu-id="584de-277">String</span></span>|<span data-ttu-id="584de-278">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="584de-278">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="584de-279">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="584de-279">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="584de-280">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="584de-280">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="584de-281">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="584de-281">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="584de-282">选项可供 IT 管理员阻止跨设备同步，但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="584de-282">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="584de-283">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="584de-283">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="584de-284">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="584de-284">messagingBlockSync</span></span>|<span data-ttu-id="584de-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-285">Boolean</span></span>|<span data-ttu-id="584de-286">指示是否在所有位置阻止短信备份和还原和消息传递。</span><span class="sxs-lookup"><span data-stu-id="584de-286">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="584de-287">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="584de-287">messagingBlockMMS</span></span>|<span data-ttu-id="584de-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-288">Boolean</span></span>|<span data-ttu-id="584de-289">指示是否阻止设备上的 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="584de-289">Indicates whether or not to block the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="584de-290">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="584de-290">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="584de-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-291">Boolean</span></span>|<span data-ttu-id="584de-292">指示是否阻止设备上的 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="584de-292">Indicates whether or not to block the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="584de-293">printerNames</span><span class="sxs-lookup"><span data-stu-id="584de-293">printerNames</span></span>|<span data-ttu-id="584de-294">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-294">String collection</span></span>|<span data-ttu-id="584de-295">根据打印机的名称（网络主机名称）自动预配打印机。</span><span class="sxs-lookup"><span data-stu-id="584de-295">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="584de-296">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="584de-296">printerDefaultName</span></span>|<span data-ttu-id="584de-297">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-297">String</span></span>|<span data-ttu-id="584de-298">已安装的打印机的名称（网络主机名称）。</span><span class="sxs-lookup"><span data-stu-id="584de-298">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="584de-299">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="584de-299">printerBlockAddition</span></span>|<span data-ttu-id="584de-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-300">Boolean</span></span>|<span data-ttu-id="584de-301">阻止用户安装来自打印机设置的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="584de-301">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="584de-302">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="584de-302">searchBlockDiacritics</span></span>|<span data-ttu-id="584de-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-303">Boolean</span></span>|<span data-ttu-id="584de-304">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="584de-304">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="584de-305">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="584de-305">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="584de-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-306">Boolean</span></span>|<span data-ttu-id="584de-307">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="584de-307">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="584de-308">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="584de-308">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="584de-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-309">Boolean</span></span>|<span data-ttu-id="584de-310">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="584de-310">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="584de-311">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="584de-311">searchEnableRemoteQueries</span></span>|<span data-ttu-id="584de-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-312">Boolean</span></span>|<span data-ttu-id="584de-313">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="584de-313">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="584de-314">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="584de-314">searchDisableUseLocation</span></span>|<span data-ttu-id="584de-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-315">Boolean</span></span>|<span data-ttu-id="584de-316">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="584de-316">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="584de-317">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="584de-317">searchDisableLocation</span></span>|<span data-ttu-id="584de-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-318">Boolean</span></span>|<span data-ttu-id="584de-319">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="584de-319">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="584de-320">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="584de-320">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="584de-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-321">Boolean</span></span>|<span data-ttu-id="584de-322">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="584de-322">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="584de-323">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="584de-323">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="584de-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-324">Boolean</span></span>|<span data-ttu-id="584de-325">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="584de-325">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="584de-326">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="584de-326">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="584de-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-327">Boolean</span></span>|<span data-ttu-id="584de-328">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="584de-328">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="584de-329">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="584de-329">searchBlockWebResults</span></span>|<span data-ttu-id="584de-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-330">Boolean</span></span>|<span data-ttu-id="584de-331">指示是否阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="584de-331">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="584de-332">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="584de-332">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="584de-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-333">Boolean</span></span>|<span data-ttu-id="584de-334">在设备已加入 Azure AD 时，指定是否允许在 OOBE 期间自动设备加密（仅限桌面）。</span><span class="sxs-lookup"><span data-stu-id="584de-334">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="584de-335">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="584de-335">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="584de-336">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="584de-336">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="584de-337">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="584de-337">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="584de-338">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="584de-338">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="584de-339">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="584de-339">oneDriveDisableFileSync</span></span>|<span data-ttu-id="584de-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-340">Boolean</span></span>|<span data-ttu-id="584de-341">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="584de-341">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="584de-342">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="584de-342">systemTelemetryProxyServer</span></span>|<span data-ttu-id="584de-343">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-343">String</span></span>|<span data-ttu-id="584de-344">获取或设置代理服务器的完全限定域名（FQDN）或 IP 地址，以转发连接的用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="584de-344">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="584de-345">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="584de-345">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="584de-346">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="584de-346">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="584de-347">指定将哪种类型的遥测数据（无、intranet、internet、两者）发送到 Microsoft 365 Analytics。</span><span class="sxs-lookup"><span data-stu-id="584de-347">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="584de-348">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="584de-348">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="584de-349">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="584de-349">inkWorkspaceAccess</span></span>|[<span data-ttu-id="584de-350">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="584de-350">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="584de-351">控制用户对墨迹工作区的访问权限，从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="584de-351">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="584de-352">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-352">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="584de-353">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="584de-353">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="584de-354">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="584de-354">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="584de-355">控制用户对墨迹工作区的访问权限，从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="584de-355">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="584de-356">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="584de-356">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="584de-357">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="584de-357">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="584de-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-358">Boolean</span></span>|<span data-ttu-id="584de-359">指定是否在墨迹工作区中显示建议的应用建议。</span><span class="sxs-lookup"><span data-stu-id="584de-359">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="584de-360">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="584de-360">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="584de-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-361">Boolean</span></span>|<span data-ttu-id="584de-362">此属性将在7月2019中弃用，并将替换为属性 SmartScreenAppInstallControl。</span><span class="sxs-lookup"><span data-stu-id="584de-362">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="584de-363">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="584de-363">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="584de-364">smartScreenAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="584de-364">smartScreenAppInstallControl</span></span>|[<span data-ttu-id="584de-365">appInstallControlType</span><span class="sxs-lookup"><span data-stu-id="584de-365">appInstallControlType</span></span>](../resources/intune-deviceconfig-appinstallcontroltype.md)|<span data-ttu-id="584de-366">在 Windows 10 版本1703中添加。</span><span class="sxs-lookup"><span data-stu-id="584de-366">Added in Windows 10, version 1703.</span></span> <span data-ttu-id="584de-367">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="584de-367">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span> <span data-ttu-id="584de-368">可取值为：`notConfigured`、`anywhere`、`storeOnly`、`recommendations`、`preferStore`。</span><span class="sxs-lookup"><span data-stu-id="584de-368">Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.</span></span>|
|<span data-ttu-id="584de-369">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="584de-369">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="584de-370">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-370">String</span></span>|<span data-ttu-id="584de-371">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="584de-371">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="584de-372">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="584de-372">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="584de-373">String</span><span class="sxs-lookup"><span data-stu-id="584de-373">String</span></span>|<span data-ttu-id="584de-374">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="584de-374">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="584de-375">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="584de-375">bluetoothAllowedServices</span></span>|<span data-ttu-id="584de-376">String 集合</span><span class="sxs-lookup"><span data-stu-id="584de-376">String collection</span></span>|<span data-ttu-id="584de-377">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="584de-377">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="584de-378">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="584de-378">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="584de-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-379">Boolean</span></span>|<span data-ttu-id="584de-380">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="584de-380">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="584de-381">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="584de-381">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="584de-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-382">Boolean</span></span>|<span data-ttu-id="584de-383">是否阻止用户使用 Swift 对和其他基于邻近的应用场景。</span><span class="sxs-lookup"><span data-stu-id="584de-383">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="584de-384">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="584de-384">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="584de-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-385">Boolean</span></span>|<span data-ttu-id="584de-386">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="584de-386">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="584de-387">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="584de-387">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="584de-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-388">Boolean</span></span>|<span data-ttu-id="584de-389">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="584de-389">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="584de-390">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="584de-390">edgeBlockAutofill</span></span>|<span data-ttu-id="584de-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-391">Boolean</span></span>|<span data-ttu-id="584de-392">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="584de-392">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="584de-393">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-393">edgeBlocked</span></span>|<span data-ttu-id="584de-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-394">Boolean</span></span>|<span data-ttu-id="584de-395">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="584de-395">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="584de-396">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="584de-396">edgeCookiePolicy</span></span>|[<span data-ttu-id="584de-397">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="584de-397">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="584de-398">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="584de-398">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="584de-399">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="584de-399">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="584de-400">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="584de-400">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="584de-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-401">Boolean</span></span>|<span data-ttu-id="584de-402">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="584de-402">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="584de-403">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="584de-403">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="584de-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-404">Boolean</span></span>|<span data-ttu-id="584de-405">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="584de-405">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="584de-406">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="584de-406">edgeBlockExtensions</span></span>|<span data-ttu-id="584de-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-407">Boolean</span></span>|<span data-ttu-id="584de-408">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="584de-408">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="584de-409">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="584de-409">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="584de-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-410">Boolean</span></span>|<span data-ttu-id="584de-411">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="584de-411">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="584de-412">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="584de-412">edgeBlockJavaScript</span></span>|<span data-ttu-id="584de-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-413">Boolean</span></span>|<span data-ttu-id="584de-414">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="584de-414">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="584de-415">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="584de-415">edgeBlockPasswordManager</span></span>|<span data-ttu-id="584de-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-416">Boolean</span></span>|<span data-ttu-id="584de-417">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="584de-417">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="584de-418">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="584de-418">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="584de-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-419">Boolean</span></span>|<span data-ttu-id="584de-420">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="584de-420">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="584de-421">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="584de-421">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="584de-422">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="584de-422">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="584de-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-423">Boolean</span></span>|<span data-ttu-id="584de-424">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="584de-424">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="584de-425">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="584de-425">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="584de-426">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="584de-426">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="584de-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-427">Boolean</span></span>|<span data-ttu-id="584de-428">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="584de-428">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="584de-429">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="584de-429">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="584de-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-430">Boolean</span></span>|<span data-ttu-id="584de-431">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="584de-431">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="584de-432">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="584de-432">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="584de-433">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="584de-433">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="584de-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-434">Boolean</span></span>|<span data-ttu-id="584de-435">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="584de-435">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="584de-436">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="584de-436">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="584de-437">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="584de-437">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="584de-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-438">Boolean</span></span>|<span data-ttu-id="584de-439">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="584de-439">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="584de-440">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="584de-440">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="584de-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-441">Boolean</span></span>|<span data-ttu-id="584de-442">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="584de-442">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="584de-443">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="584de-443">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="584de-444">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="584de-444">edgeFavoritesListLocation</span></span>|<span data-ttu-id="584de-445">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-445">String</span></span>|<span data-ttu-id="584de-446">要设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="584de-446">The location of the favorites list to provision.</span></span> <span data-ttu-id="584de-447">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="584de-447">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="584de-448">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="584de-448">edgeBlockEditFavorites</span></span>|<span data-ttu-id="584de-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-449">Boolean</span></span>|<span data-ttu-id="584de-450">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="584de-450">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="584de-451">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="584de-451">edgeNewTabPageURL</span></span>|<span data-ttu-id="584de-452">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-452">String</span></span>|<span data-ttu-id="584de-453">指定在创建新选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="584de-453">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="584de-454">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="584de-454">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="584de-455">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="584de-455">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="584de-456">使 Home 按钮可以隐藏、加载默认起始页、加载新的选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="584de-456">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="584de-457">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="584de-457">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="584de-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-458">Boolean</span></span>|<span data-ttu-id="584de-459">启用 "主页" 按钮配置。</span><span class="sxs-lookup"><span data-stu-id="584de-459">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="584de-460">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="584de-460">edgeOpensWith</span></span>|[<span data-ttu-id="584de-461">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="584de-461">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="584de-462">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="584de-462">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="584de-463">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="584de-463">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="584de-464">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="584de-464">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="584de-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-465">Boolean</span></span>|<span data-ttu-id="584de-466">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="584de-466">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="584de-467">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="584de-467">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="584de-468">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-468">String collection</span></span>|<span data-ttu-id="584de-469">指定所需的浏览器扩展的程序包系列名称列表，用户无法关闭这些扩展。</span><span class="sxs-lookup"><span data-stu-id="584de-469">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="584de-470">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="584de-470">edgeBlockPrinting</span></span>|<span data-ttu-id="584de-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-471">Boolean</span></span>|<span data-ttu-id="584de-472">将 Edge 配置为允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="584de-472">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="584de-473">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="584de-473">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="584de-474">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-474">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-475">获取或设置一个值，该值指定是否将收藏夹栏设置为始终在任何页面上都可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-475">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="584de-476">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-476">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-477">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="584de-477">edgeBlockSavingHistory</span></span>|<span data-ttu-id="584de-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-478">Boolean</span></span>|<span data-ttu-id="584de-479">将 Edge 配置为允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="584de-479">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="584de-480">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="584de-480">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="584de-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-481">Boolean</span></span>|<span data-ttu-id="584de-482">允许或阻止边缘进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="584de-482">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="584de-483">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="584de-483">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="584de-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-484">Boolean</span></span>|<span data-ttu-id="584de-485">将配置为在 Edge 中加载空白页面，而不是默认的新选项卡页面，并防止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="584de-485">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="584de-486">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="584de-486">edgeBlockTabPreloading</span></span>|<span data-ttu-id="584de-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-487">Boolean</span></span>|<span data-ttu-id="584de-488">配置边缘是否在 Windows 启动时预加载新的选项卡页。</span><span class="sxs-lookup"><span data-stu-id="584de-488">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="584de-489">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="584de-489">edgeBlockPrelaunch</span></span>|<span data-ttu-id="584de-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-490">Boolean</span></span>|<span data-ttu-id="584de-491">确定 Microsoft Edge 在 Windows 启动时是否为 prelaunched。</span><span class="sxs-lookup"><span data-stu-id="584de-491">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="584de-492">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="584de-492">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="584de-493">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="584de-493">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="584de-494">控制边缘在切换到 Internet Explorer 之前显示的消息。</span><span class="sxs-lookup"><span data-stu-id="584de-494">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="584de-495">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="584de-495">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="584de-496">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="584de-496">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="584de-497">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-497">Boolean</span></span>|<span data-ttu-id="584de-498">允许或阻止用户覆盖证书错误。</span><span class="sxs-lookup"><span data-stu-id="584de-498">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="584de-499">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="584de-499">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="584de-500">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="584de-500">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="584de-501">根据配置展台模式，控制 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="584de-501">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="584de-502">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="584de-502">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="584de-503">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="584de-503">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="584de-504">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-504">Int32</span></span>|<span data-ttu-id="584de-505">指定在 Microsoft Edge 展台重置前的上次用户活动的时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="584de-505">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="584de-506">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="584de-506">Valid values are 0-1440.</span></span> <span data-ttu-id="584de-507">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="584de-507">The default is 5.</span></span> <span data-ttu-id="584de-508">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="584de-508">0 indicates no reset.</span></span> <span data-ttu-id="584de-509">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="584de-509">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="584de-510">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="584de-510">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="584de-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-511">Boolean</span></span>|<span data-ttu-id="584de-512">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="584de-512">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="584de-513">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="584de-513">cellularBlockVpn</span></span>|<span data-ttu-id="584de-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-514">Boolean</span></span>|<span data-ttu-id="584de-515">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="584de-515">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="584de-516">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="584de-516">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="584de-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-517">Boolean</span></span>|<span data-ttu-id="584de-518">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="584de-518">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="584de-519">cellularData</span><span class="sxs-lookup"><span data-stu-id="584de-519">cellularData</span></span>|[<span data-ttu-id="584de-520">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="584de-520">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="584de-521">是否允许设备上的手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="584de-521">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="584de-522">如果未配置，则允许手机网络数据通道，用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="584de-522">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="584de-523">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="584de-523">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="584de-524">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="584de-524">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="584de-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-525">Boolean</span></span>|<span data-ttu-id="584de-526">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="584de-526">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="584de-527">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="584de-527">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="584de-528">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-528">Int32</span></span>|<span data-ttu-id="584de-529">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="584de-529">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="584de-530">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="584de-530">Valid values 0 to 90</span></span>|
|<span data-ttu-id="584de-531">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="584de-531">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="584de-532">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="584de-532">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="584de-533">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="584de-533">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="584de-534">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="584de-534">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="584de-535">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="584de-535">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="584de-536">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="584de-536">Defender day of the week for the system scan.</span></span> <span data-ttu-id="584de-537">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="584de-537">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="584de-538">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="584de-538">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="584de-539">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-539">String collection</span></span>|<span data-ttu-id="584de-540">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="584de-540">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="584de-541">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="584de-541">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="584de-542">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-542">String collection</span></span>|<span data-ttu-id="584de-543">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="584de-543">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="584de-544">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="584de-544">defenderScanMaxCpu</span></span>|<span data-ttu-id="584de-545">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-545">Int32</span></span>|<span data-ttu-id="584de-546">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="584de-546">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="584de-547">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="584de-547">Valid values 0 to 100</span></span>|
|<span data-ttu-id="584de-548">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="584de-548">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="584de-549">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="584de-549">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="584de-550">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="584de-550">Value for monitoring file activity.</span></span> <span data-ttu-id="584de-551">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="584de-551">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="584de-552">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="584de-552">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="584de-553">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="584de-553">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="584de-554">获取或设置要对可能有害的应用程序（PUA）执行的 Defender 操作，其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时，Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="584de-554">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="584de-555">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="584de-555">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="584de-556">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="584de-556">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="584de-557">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="584de-557">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="584de-558">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="584de-558">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="584de-559">获取或设置要对可能有害的应用程序（PUA）执行的 Defender 操作，其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时，Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="584de-559">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="584de-560">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="584de-560">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="584de-561">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="584de-561">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="584de-562">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="584de-562">defenderProcessesToExclude</span></span>|<span data-ttu-id="584de-563">String 集合</span><span class="sxs-lookup"><span data-stu-id="584de-563">String collection</span></span>|<span data-ttu-id="584de-564">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="584de-564">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="584de-565">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="584de-565">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="584de-566">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="584de-566">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="584de-567">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="584de-567">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="584de-568">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="584de-568">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="584de-569">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="584de-569">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="584de-570">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-570">Boolean</span></span>|<span data-ttu-id="584de-571">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="584de-571">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="584de-572">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="584de-572">defenderRequireCloudProtection</span></span>|<span data-ttu-id="584de-573">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-573">Boolean</span></span>|<span data-ttu-id="584de-574">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="584de-574">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="584de-575">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="584de-575">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="584de-576">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-576">Boolean</span></span>|<span data-ttu-id="584de-577">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="584de-577">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="584de-578">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="584de-578">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="584de-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-579">Boolean</span></span>|<span data-ttu-id="584de-580">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="584de-580">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="584de-581">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="584de-581">defenderScanArchiveFiles</span></span>|<span data-ttu-id="584de-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-582">Boolean</span></span>|<span data-ttu-id="584de-583">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="584de-583">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="584de-584">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="584de-584">defenderScanDownloads</span></span>|<span data-ttu-id="584de-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-585">Boolean</span></span>|<span data-ttu-id="584de-586">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="584de-586">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="584de-587">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="584de-587">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="584de-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-588">Boolean</span></span>|<span data-ttu-id="584de-589">启用后，在计划扫描期间将使用较低的 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="584de-589">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="584de-590">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="584de-590">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="584de-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-591">Boolean</span></span>|<span data-ttu-id="584de-592">当被阻止时，将关闭计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="584de-592">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="584de-593">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="584de-593">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="584de-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-594">Boolean</span></span>|<span data-ttu-id="584de-595">当被阻止时，计划的完全扫描的追赶扫描将被禁用。</span><span class="sxs-lookup"><span data-stu-id="584de-595">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="584de-596">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="584de-596">defenderScanNetworkFiles</span></span>|<span data-ttu-id="584de-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-597">Boolean</span></span>|<span data-ttu-id="584de-598">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="584de-598">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="584de-599">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="584de-599">defenderScanIncomingMail</span></span>|<span data-ttu-id="584de-600">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-600">Boolean</span></span>|<span data-ttu-id="584de-601">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="584de-601">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="584de-602">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="584de-602">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="584de-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-603">Boolean</span></span>|<span data-ttu-id="584de-604">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="584de-604">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="584de-605">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="584de-605">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="584de-606">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-606">Boolean</span></span>|<span data-ttu-id="584de-607">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="584de-607">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="584de-608">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="584de-608">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="584de-609">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-609">Boolean</span></span>|<span data-ttu-id="584de-610">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="584de-610">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="584de-611">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="584de-611">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="584de-612">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-612">Int32</span></span>|<span data-ttu-id="584de-613">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="584de-613">The signature update interval in hours.</span></span> <span data-ttu-id="584de-614">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="584de-614">Specify 0 not to check.</span></span> <span data-ttu-id="584de-615">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="584de-615">Valid values 0 to 24</span></span>|
|<span data-ttu-id="584de-616">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="584de-616">defenderScanType</span></span>|[<span data-ttu-id="584de-617">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="584de-617">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="584de-618">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="584de-618">The defender system scan type.</span></span> <span data-ttu-id="584de-619">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="584de-619">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="584de-620">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="584de-620">defenderScheduledScanTime</span></span>|<span data-ttu-id="584de-621">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="584de-621">TimeOfDay</span></span>|<span data-ttu-id="584de-622">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="584de-622">The defender time for the system scan.</span></span>|
|<span data-ttu-id="584de-623">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="584de-623">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="584de-624">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="584de-624">TimeOfDay</span></span>|<span data-ttu-id="584de-625">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="584de-625">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="584de-626">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="584de-626">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="584de-627">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="584de-627">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="584de-628">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="584de-628">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="584de-629">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="584de-629">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="584de-630">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="584de-630">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="584de-631">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-631">Int32</span></span>|<span data-ttu-id="584de-632">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="584de-632">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="584de-633">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="584de-633">Valid values 0 to 50</span></span>|
|<span data-ttu-id="584de-634">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="584de-634">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="584de-635">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-635">Int32</span></span>|<span data-ttu-id="584de-636">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="584de-636">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="584de-637">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="584de-637">Valid values 0 to 50</span></span>|
|<span data-ttu-id="584de-638">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="584de-638">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="584de-639">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-639">Boolean</span></span>|<span data-ttu-id="584de-640">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="584de-640">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="584de-641">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="584de-641">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="584de-642">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="584de-642">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="584de-643">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="584de-643">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="584de-644">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="584de-644">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="584de-645">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="584de-645">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="584de-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-646">Boolean</span></span>|<span data-ttu-id="584de-647">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="584de-647">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="584de-648">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="584de-648">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="584de-649">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="584de-649">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="584de-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-650">Boolean</span></span>|<span data-ttu-id="584de-651">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="584de-651">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="584de-652">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="584de-652">lockScreenBlockCortana</span></span>|<span data-ttu-id="584de-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-653">Boolean</span></span>|<span data-ttu-id="584de-654">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="584de-654">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="584de-655">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="584de-655">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="584de-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-656">Boolean</span></span>|<span data-ttu-id="584de-657">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="584de-657">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="584de-658">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="584de-658">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="584de-659">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-659">Int32</span></span>|<span data-ttu-id="584de-660">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="584de-660">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="584de-661">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="584de-661">Supported values are 11-1800.</span></span> <span data-ttu-id="584de-662">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="584de-662">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="584de-663">lockScreenActivateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="584de-663">lockScreenActivateAppsWithVoice</span></span>|[<span data-ttu-id="584de-664">启用</span><span class="sxs-lookup"><span data-stu-id="584de-664">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="584de-665">此策略设置指定在系统处于锁定状态时，Windows 应用是否可以通过语音激活。</span><span class="sxs-lookup"><span data-stu-id="584de-665">This policy setting specifies whether Windows apps can be activated by voice while the system is locked.</span></span> <span data-ttu-id="584de-666">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-666">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="584de-667">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="584de-667">passwordBlockSimple</span></span>|<span data-ttu-id="584de-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-668">Boolean</span></span>|<span data-ttu-id="584de-669">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="584de-669">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="584de-670">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="584de-670">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="584de-671">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="584de-671">passwordExpirationDays</span></span>|<span data-ttu-id="584de-672">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-672">Int32</span></span>|<span data-ttu-id="584de-673">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="584de-673">The password expiration in days.</span></span> <span data-ttu-id="584de-674">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="584de-674">Valid values 0 to 730</span></span>|
|<span data-ttu-id="584de-675">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="584de-675">passwordMinimumLength</span></span>|<span data-ttu-id="584de-676">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-676">Int32</span></span>|<span data-ttu-id="584de-677">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="584de-677">The minimum password length.</span></span> <span data-ttu-id="584de-678">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="584de-678">Valid values 4 to 16</span></span>|
|<span data-ttu-id="584de-679">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="584de-679">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="584de-680">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-680">Int32</span></span>|<span data-ttu-id="584de-681">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="584de-681">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="584de-682">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="584de-682">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="584de-683">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-683">Int32</span></span>|<span data-ttu-id="584de-684">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="584de-684">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="584de-685">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="584de-685">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="584de-686">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-686">Int32</span></span>|<span data-ttu-id="584de-687">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="584de-687">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="584de-688">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="584de-688">Valid values 0 to 50</span></span>|
|<span data-ttu-id="584de-689">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="584de-689">passwordRequired</span></span>|<span data-ttu-id="584de-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-690">Boolean</span></span>|<span data-ttu-id="584de-691">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="584de-691">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="584de-692">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="584de-692">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="584de-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-693">Boolean</span></span>|<span data-ttu-id="584de-694">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="584de-694">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="584de-695">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="584de-695">passwordRequiredType</span></span>|[<span data-ttu-id="584de-696">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="584de-696">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="584de-697">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="584de-697">The required password type.</span></span> <span data-ttu-id="584de-698">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="584de-698">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="584de-699">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="584de-699">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="584de-700">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-700">Int32</span></span>|<span data-ttu-id="584de-701">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="584de-701">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="584de-702">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="584de-702">Valid values 0 to 999</span></span>|
|<span data-ttu-id="584de-703">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="584de-703">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="584de-704">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-704">Int32</span></span>|<span data-ttu-id="584de-705">此安全设置确定用户可以更改密码之前必须使用该密码的时间（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="584de-705">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="584de-706">有效值为0至998</span><span class="sxs-lookup"><span data-stu-id="584de-706">Valid values 0 to 998</span></span>|
|<span data-ttu-id="584de-707">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="584de-707">privacyAdvertisingId</span></span>|[<span data-ttu-id="584de-708">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="584de-708">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="584de-709">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="584de-709">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="584de-710">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="584de-710">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="584de-711">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="584de-711">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="584de-712">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="584de-712">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="584de-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-713">Boolean</span></span>|<span data-ttu-id="584de-714">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="584de-714">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="584de-715">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="584de-715">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="584de-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-716">Boolean</span></span>|<span data-ttu-id="584de-717">此策略可防止在用户登录时为新的和已升级的用户启动隐私体验。</span><span class="sxs-lookup"><span data-stu-id="584de-717">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="584de-718">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="584de-718">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="584de-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-719">Boolean</span></span>|<span data-ttu-id="584de-720">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="584de-720">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="584de-721">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="584de-721">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="584de-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-722">Boolean</span></span>|<span data-ttu-id="584de-723">阻止共享体验和发现任务切换器等中的最近使用的资源。</span><span class="sxs-lookup"><span data-stu-id="584de-723">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="584de-724">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="584de-724">privacyBlockActivityFeed</span></span>|<span data-ttu-id="584de-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-725">Boolean</span></span>|<span data-ttu-id="584de-726">阻止 Cortana、听写或存储应用程序的基于云的语音服务的使用。</span><span class="sxs-lookup"><span data-stu-id="584de-726">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="584de-727">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="584de-727">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="584de-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-728">Boolean</span></span>|<span data-ttu-id="584de-729">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="584de-729">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="584de-730">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="584de-730">startMenuAppListVisibility</span></span>|[<span data-ttu-id="584de-731">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="584de-731">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="584de-732">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="584de-732">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="584de-733">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="584de-733">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="584de-734">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="584de-734">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="584de-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-735">Boolean</span></span>|<span data-ttu-id="584de-736">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-736">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="584de-737">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="584de-737">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="584de-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-738">Boolean</span></span>|<span data-ttu-id="584de-739">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="584de-739">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="584de-740">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="584de-740">startMenuHideHibernate</span></span>|<span data-ttu-id="584de-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-741">Boolean</span></span>|<span data-ttu-id="584de-742">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-742">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="584de-743">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="584de-743">startMenuHideLock</span></span>|<span data-ttu-id="584de-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-744">Boolean</span></span>|<span data-ttu-id="584de-745">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-745">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="584de-746">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="584de-746">startMenuHidePowerButton</span></span>|<span data-ttu-id="584de-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-747">Boolean</span></span>|<span data-ttu-id="584de-748">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-748">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="584de-749">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="584de-749">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="584de-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-750">Boolean</span></span>|<span data-ttu-id="584de-751">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="584de-751">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="584de-752">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="584de-752">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="584de-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-753">Boolean</span></span>|<span data-ttu-id="584de-754">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="584de-754">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="584de-755">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="584de-755">startMenuHideRestartOptions</span></span>|<span data-ttu-id="584de-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-756">Boolean</span></span>|<span data-ttu-id="584de-757">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-757">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="584de-758">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="584de-758">startMenuHideShutDown</span></span>|<span data-ttu-id="584de-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-759">Boolean</span></span>|<span data-ttu-id="584de-760">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-760">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="584de-761">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="584de-761">startMenuHideSignOut</span></span>|<span data-ttu-id="584de-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-762">Boolean</span></span>|<span data-ttu-id="584de-763">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-763">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="584de-764">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="584de-764">startMenuHideSleep</span></span>|<span data-ttu-id="584de-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-765">Boolean</span></span>|<span data-ttu-id="584de-766">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-766">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="584de-767">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="584de-767">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="584de-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-768">Boolean</span></span>|<span data-ttu-id="584de-769">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-769">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="584de-770">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="584de-770">startMenuHideUserTile</span></span>|<span data-ttu-id="584de-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-771">Boolean</span></span>|<span data-ttu-id="584de-772">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="584de-772">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="584de-773">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="584de-773">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="584de-774">Binary</span><span class="sxs-lookup"><span data-stu-id="584de-774">Binary</span></span>|<span data-ttu-id="584de-775">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="584de-775">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="584de-776">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="584de-776">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="584de-777">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="584de-777">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="584de-778">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="584de-778">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="584de-779">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="584de-779">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="584de-780">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="584de-780">startMenuLayoutXml</span></span>|<span data-ttu-id="584de-781">Binary</span><span class="sxs-lookup"><span data-stu-id="584de-781">Binary</span></span>|<span data-ttu-id="584de-782">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="584de-782">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="584de-783">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="584de-783">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="584de-784">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="584de-784">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="584de-785">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="584de-785">startMenuMode</span></span>|[<span data-ttu-id="584de-786">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="584de-786">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="584de-787">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="584de-787">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="584de-788">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="584de-788">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="584de-789">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="584de-789">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="584de-790">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-790">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-791">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-791">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-792">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-792">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-793">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="584de-793">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="584de-794">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-794">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-795">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-795">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-796">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-796">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-797">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="584de-797">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="584de-798">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-798">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-799">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-799">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="584de-800">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-800">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-801">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="584de-801">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="584de-802">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-802">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-803">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-803">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-804">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-804">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-805">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="584de-805">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="584de-806">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-806">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-807">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-807">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-808">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-808">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-809">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="584de-809">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="584de-810">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-810">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-811">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-811">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-812">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-812">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-813">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="584de-813">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="584de-814">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-814">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-815">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-815">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-816">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-816">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-817">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="584de-817">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="584de-818">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-818">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-819">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-819">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-820">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-820">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-821">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="584de-821">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="584de-822">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-822">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-823">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-823">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-824">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-824">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-825">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="584de-825">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="584de-826">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="584de-826">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="584de-827">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="584de-827">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="584de-828">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="584de-828">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="584de-829">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="584de-829">settingsBlockSettingsApp</span></span>|<span data-ttu-id="584de-830">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-830">Boolean</span></span>|<span data-ttu-id="584de-831">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="584de-831">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="584de-832">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="584de-832">settingsBlockSystemPage</span></span>|<span data-ttu-id="584de-833">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-833">Boolean</span></span>|<span data-ttu-id="584de-834">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="584de-834">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="584de-835">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="584de-835">settingsBlockDevicesPage</span></span>|<span data-ttu-id="584de-836">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-836">Boolean</span></span>|<span data-ttu-id="584de-837">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="584de-837">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="584de-838">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="584de-838">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="584de-839">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-839">Boolean</span></span>|<span data-ttu-id="584de-840">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="584de-840">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="584de-841">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="584de-841">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="584de-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-842">Boolean</span></span>|<span data-ttu-id="584de-843">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="584de-843">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="584de-844">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="584de-844">settingsBlockAccountsPage</span></span>|<span data-ttu-id="584de-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-845">Boolean</span></span>|<span data-ttu-id="584de-846">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="584de-846">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="584de-847">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="584de-847">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="584de-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-848">Boolean</span></span>|<span data-ttu-id="584de-849">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="584de-849">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="584de-850">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="584de-850">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="584de-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-851">Boolean</span></span>|<span data-ttu-id="584de-852">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="584de-852">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="584de-853">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="584de-853">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="584de-854">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-854">Boolean</span></span>|<span data-ttu-id="584de-855">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="584de-855">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="584de-856">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="584de-856">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="584de-857">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-857">Boolean</span></span>|<span data-ttu-id="584de-858">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="584de-858">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="584de-859">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="584de-859">settingsBlockAppsPage</span></span>|<span data-ttu-id="584de-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-860">Boolean</span></span>|<span data-ttu-id="584de-861">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="584de-861">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="584de-862">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="584de-862">settingsBlockGamingPage</span></span>|<span data-ttu-id="584de-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-863">Boolean</span></span>|<span data-ttu-id="584de-864">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="584de-864">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="584de-865">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="584de-865">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="584de-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-866">Boolean</span></span>|<span data-ttu-id="584de-867">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="584de-867">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="584de-868">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-868">windowsSpotlightBlocked</span></span>|<span data-ttu-id="584de-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-869">Boolean</span></span>|<span data-ttu-id="584de-870">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="584de-870">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="584de-871">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="584de-871">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="584de-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-872">Boolean</span></span>|<span data-ttu-id="584de-873">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="584de-873">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="584de-874">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="584de-874">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="584de-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-875">Boolean</span></span>|<span data-ttu-id="584de-876">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="584de-876">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="584de-877">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="584de-877">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="584de-878">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-878">Boolean</span></span>|<span data-ttu-id="584de-879">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="584de-879">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="584de-880">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="584de-880">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="584de-881">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-881">Boolean</span></span>|<span data-ttu-id="584de-882">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="584de-882">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="584de-883">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="584de-883">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="584de-884">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-884">Boolean</span></span>|<span data-ttu-id="584de-885">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="584de-885">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="584de-886">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="584de-886">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="584de-887">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="584de-887">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="584de-888">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="584de-888">Specifies the type of Spotlight.</span></span> <span data-ttu-id="584de-889">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="584de-889">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="584de-890">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="584de-890">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="584de-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-891">Boolean</span></span>|<span data-ttu-id="584de-892">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="584de-892">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="584de-893">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="584de-893">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="584de-894">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="584de-894">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="584de-895">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-895">Boolean</span></span>|<span data-ttu-id="584de-896">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="584de-896">Disable automatic detection of settings.</span></span> <span data-ttu-id="584de-897">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="584de-897">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="584de-898">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="584de-898">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="584de-899">String</span><span class="sxs-lookup"><span data-stu-id="584de-899">String</span></span>|<span data-ttu-id="584de-900">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="584de-900">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="584de-901">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="584de-901">networkProxyServer</span></span>|[<span data-ttu-id="584de-902">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="584de-902">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="584de-903">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="584de-903">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="584de-904">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="584de-904">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="584de-905">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-905">Boolean</span></span>|<span data-ttu-id="584de-906">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="584de-906">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="584de-907">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-907">antiTheftModeBlocked</span></span>|<span data-ttu-id="584de-908">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-908">Boolean</span></span>|<span data-ttu-id="584de-909">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="584de-909">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="584de-910">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-910">bluetoothBlocked</span></span>|<span data-ttu-id="584de-911">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-911">Boolean</span></span>|<span data-ttu-id="584de-912">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="584de-912">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="584de-913">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-913">cameraBlocked</span></span>|<span data-ttu-id="584de-914">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-914">Boolean</span></span>|<span data-ttu-id="584de-915">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="584de-915">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="584de-916">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-916">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="584de-917">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-917">Boolean</span></span>|<span data-ttu-id="584de-918">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="584de-918">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="584de-919">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="584de-919">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="584de-920">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-920">Boolean</span></span>|<span data-ttu-id="584de-921">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="584de-921">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="584de-922">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-922">copyPasteBlocked</span></span>|<span data-ttu-id="584de-923">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-923">Boolean</span></span>|<span data-ttu-id="584de-924">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="584de-924">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="584de-925">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-925">cortanaBlocked</span></span>|<span data-ttu-id="584de-926">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-926">Boolean</span></span>|<span data-ttu-id="584de-927">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="584de-927">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="584de-928">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="584de-928">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="584de-929">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-929">Boolean</span></span>|<span data-ttu-id="584de-930">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="584de-930">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="584de-931">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="584de-931">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="584de-932">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-932">Boolean</span></span>|<span data-ttu-id="584de-933">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="584de-933">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="584de-934">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="584de-934">safeSearchFilter</span></span>|[<span data-ttu-id="584de-935">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="584de-935">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="584de-936">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="584de-936">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="584de-937">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="584de-937">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="584de-938">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="584de-938">edgeBlockPopups</span></span>|<span data-ttu-id="584de-939">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-939">Boolean</span></span>|<span data-ttu-id="584de-940">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="584de-940">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="584de-941">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="584de-941">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="584de-942">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-942">Boolean</span></span>|<span data-ttu-id="584de-943">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="584de-943">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="584de-944">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="584de-944">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="584de-945">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-945">Boolean</span></span>|<span data-ttu-id="584de-946">指示是否阻止用户添加新的搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="584de-946">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="584de-947">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="584de-947">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="584de-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-948">Boolean</span></span>|<span data-ttu-id="584de-949">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="584de-949">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="584de-950">注意：此属性的名称是误导性的;属性已过时，请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="584de-950">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="584de-951">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="584de-951">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="584de-952">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-952">Boolean</span></span>|<span data-ttu-id="584de-953">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="584de-953">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="584de-954">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="584de-954">edgeRequireSmartScreen</span></span>|<span data-ttu-id="584de-955">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-955">Boolean</span></span>|<span data-ttu-id="584de-956">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="584de-956">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="584de-957">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="584de-957">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="584de-958">字符串</span><span class="sxs-lookup"><span data-stu-id="584de-958">String</span></span>|<span data-ttu-id="584de-959">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="584de-959">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="584de-960">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="584de-960">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="584de-961">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="584de-961">edgeFirstRunUrl</span></span>|<span data-ttu-id="584de-962">String</span><span class="sxs-lookup"><span data-stu-id="584de-962">String</span></span>|<span data-ttu-id="584de-963">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="584de-963">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="584de-964">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="584de-964">edgeSearchEngine</span></span>|[<span data-ttu-id="584de-965">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="584de-965">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="584de-966">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="584de-966">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="584de-967">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="584de-967">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="584de-968">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="584de-968">edgeHomepageUrls</span></span>|<span data-ttu-id="584de-969">String 集合</span><span class="sxs-lookup"><span data-stu-id="584de-969">String collection</span></span>|<span data-ttu-id="584de-970">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="584de-970">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="584de-971">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="584de-971">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="584de-972">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-972">Boolean</span></span>|<span data-ttu-id="584de-973">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="584de-973">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="584de-974">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="584de-974">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="584de-975">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-975">Boolean</span></span>|<span data-ttu-id="584de-976">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="584de-976">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="584de-977">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="584de-977">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="584de-978">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-978">Boolean</span></span>|<span data-ttu-id="584de-979">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="584de-979">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="584de-980">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="584de-980">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="584de-981">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-981">Boolean</span></span>|<span data-ttu-id="584de-982">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="584de-982">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="584de-983">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-983">internetSharingBlocked</span></span>|<span data-ttu-id="584de-984">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-984">Boolean</span></span>|<span data-ttu-id="584de-985">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="584de-985">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="584de-986">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="584de-986">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="584de-987">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-987">Boolean</span></span>|<span data-ttu-id="584de-988">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="584de-988">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="584de-989">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="584de-989">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="584de-990">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-990">Boolean</span></span>|<span data-ttu-id="584de-991">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="584de-991">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="584de-992">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="584de-992">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="584de-993">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-993">Boolean</span></span>|<span data-ttu-id="584de-994">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="584de-994">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="584de-995">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="584de-995">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="584de-996">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-996">Boolean</span></span>|<span data-ttu-id="584de-997">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="584de-997">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="584de-998">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="584de-998">settingsBlockChangeRegion</span></span>|<span data-ttu-id="584de-999">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-999">Boolean</span></span>|<span data-ttu-id="584de-1000">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="584de-1000">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="584de-1001">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="584de-1001">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="584de-1002">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1002">Boolean</span></span>|<span data-ttu-id="584de-1003">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="584de-1003">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="584de-1004">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="584de-1004">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="584de-1005">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1005">Boolean</span></span>|<span data-ttu-id="584de-1006">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="584de-1006">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="584de-1007">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1007">locationServicesBlocked</span></span>|<span data-ttu-id="584de-1008">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1008">Boolean</span></span>|<span data-ttu-id="584de-1009">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="584de-1009">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="584de-1010">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1010">microsoftAccountBlocked</span></span>|<span data-ttu-id="584de-1011">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1011">Boolean</span></span>|<span data-ttu-id="584de-1012">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="584de-1012">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="584de-1013">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="584de-1013">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="584de-1014">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1014">Boolean</span></span>|<span data-ttu-id="584de-1015">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="584de-1015">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="584de-1016">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1016">nfcBlocked</span></span>|<span data-ttu-id="584de-1017">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1017">Boolean</span></span>|<span data-ttu-id="584de-1018">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="584de-1018">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="584de-1019">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1019">resetProtectionModeBlocked</span></span>|<span data-ttu-id="584de-1020">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1020">Boolean</span></span>|<span data-ttu-id="584de-1021">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="584de-1021">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="584de-1022">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1022">screenCaptureBlocked</span></span>|<span data-ttu-id="584de-1023">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1023">Boolean</span></span>|<span data-ttu-id="584de-1024">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="584de-1024">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="584de-1025">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="584de-1025">storageBlockRemovableStorage</span></span>|<span data-ttu-id="584de-1026">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1026">Boolean</span></span>|<span data-ttu-id="584de-1027">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="584de-1027">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="584de-1028">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="584de-1028">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="584de-1029">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1029">Boolean</span></span>|<span data-ttu-id="584de-1030">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="584de-1030">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="584de-1031">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1031">usbBlocked</span></span>|<span data-ttu-id="584de-1032">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1032">Boolean</span></span>|<span data-ttu-id="584de-1033">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="584de-1033">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="584de-1034">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1034">voiceRecordingBlocked</span></span>|<span data-ttu-id="584de-1035">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1035">Boolean</span></span>|<span data-ttu-id="584de-1036">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="584de-1036">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="584de-1037">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="584de-1037">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="584de-1038">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1038">Boolean</span></span>|<span data-ttu-id="584de-1039">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="584de-1039">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="584de-1040">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="584de-1040">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="584de-1041">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1041">wiFiBlocked</span></span>|<span data-ttu-id="584de-1042">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1042">Boolean</span></span>|<span data-ttu-id="584de-1043">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="584de-1043">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="584de-1044">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="584de-1044">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="584de-1045">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1045">Boolean</span></span>|<span data-ttu-id="584de-1046">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="584de-1046">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="584de-1047">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="584de-1047">wiFiScanInterval</span></span>|<span data-ttu-id="584de-1048">Int32</span><span class="sxs-lookup"><span data-stu-id="584de-1048">Int32</span></span>|<span data-ttu-id="584de-1049">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="584de-1049">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="584de-1050">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="584de-1050">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="584de-1051">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="584de-1051">Valid values 1 to 500</span></span>|
|<span data-ttu-id="584de-1052">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="584de-1052">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="584de-1053">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1053">Boolean</span></span>|<span data-ttu-id="584de-1054">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="584de-1054">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="584de-1055">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="584de-1055">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="584de-1056">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1056">Boolean</span></span>|<span data-ttu-id="584de-1057">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="584de-1057">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="584de-1058">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="584de-1058">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="584de-1059">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1059">Boolean</span></span>|<span data-ttu-id="584de-1060">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="584de-1060">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="584de-1061">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1061">windowsStoreBlocked</span></span>|<span data-ttu-id="584de-1062">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1062">Boolean</span></span>|<span data-ttu-id="584de-1063">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="584de-1063">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="584de-1064">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="584de-1064">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="584de-1065">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="584de-1065">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="584de-1066">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="584de-1066">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="584de-1067">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="584de-1067">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="584de-1068">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="584de-1068">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="584de-1069">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1069">Boolean</span></span>|<span data-ttu-id="584de-1070">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="584de-1070">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="584de-1071">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="584de-1071">developerUnlockSetting</span></span>|[<span data-ttu-id="584de-1072">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="584de-1072">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="584de-1073">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="584de-1073">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="584de-1074">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="584de-1074">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="584de-1075">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="584de-1075">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="584de-1076">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1076">Boolean</span></span>|<span data-ttu-id="584de-1077">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="584de-1077">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="584de-1078">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="584de-1078">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="584de-1079">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1079">Boolean</span></span>|<span data-ttu-id="584de-1080">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="584de-1080">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="584de-1081">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="584de-1081">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="584de-1082">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1082">Boolean</span></span>|<span data-ttu-id="584de-1083">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="584de-1083">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="584de-1084">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="584de-1084">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="584de-1085">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1085">Boolean</span></span>|<span data-ttu-id="584de-1086">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="584de-1086">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="584de-1087">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="584de-1087">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="584de-1088">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1088">Boolean</span></span>|<span data-ttu-id="584de-1089">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="584de-1089">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="584de-1090">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="584de-1090">gameDvrBlocked</span></span>|<span data-ttu-id="584de-1091">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1091">Boolean</span></span>|<span data-ttu-id="584de-1092">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="584de-1092">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="584de-1093">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="584de-1093">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="584de-1094">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1094">Boolean</span></span>|<span data-ttu-id="584de-1095">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="584de-1095">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="584de-1096">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="584de-1096">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="584de-1097">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1097">Boolean</span></span>|<span data-ttu-id="584de-1098">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="584de-1098">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="584de-1099">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="584de-1099">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="584de-1100">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1100">Boolean</span></span>|<span data-ttu-id="584de-1101">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="584de-1101">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="584de-1102">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="584de-1102">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="584de-1103">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1103">Boolean</span></span>|<span data-ttu-id="584de-1104">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="584de-1104">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="584de-1105">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="584de-1105">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="584de-1106">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1106">Boolean</span></span>|<span data-ttu-id="584de-1107">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="584de-1107">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="584de-1108">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="584de-1108">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="584de-1109">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1109">Boolean</span></span>|<span data-ttu-id="584de-1110">此策略设置允许用户更改通常仅供系统管理员使用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="584de-1110">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="584de-1111">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="584de-1111">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="584de-1112">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1112">Boolean</span></span>|<span data-ttu-id="584de-1113">此策略设置指示 Windows Installer 在系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="584de-1113">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="584de-1114">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="584de-1114">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="584de-1115">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1115">Boolean</span></span>|<span data-ttu-id="584de-1116">通过此策略设置，您可以阻止所有热插拔 PCI 下游端口的直接内存访问（DMA），直到用户登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="584de-1116">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="584de-1117">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="584de-1117">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="584de-1118">String collection</span><span class="sxs-lookup"><span data-stu-id="584de-1118">String collection</span></span>|<span data-ttu-id="584de-1119">Windows 应用的以分号分隔的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="584de-1119">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="584de-1120">登录后将启动列出的 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="584de-1120">Listed Windows apps are to be launched after logon.</span></span>|
|<span data-ttu-id="584de-1121">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="584de-1121">uninstallBuiltInApps</span></span>|<span data-ttu-id="584de-1122">Boolean</span><span class="sxs-lookup"><span data-stu-id="584de-1122">Boolean</span></span>|<span data-ttu-id="584de-1123">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="584de-1123">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="584de-1124">响应</span><span class="sxs-lookup"><span data-stu-id="584de-1124">Response</span></span>
<span data-ttu-id="584de-1125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="584de-1125">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="584de-1126">示例</span><span class="sxs-lookup"><span data-stu-id="584de-1126">Example</span></span>

### <a name="request"></a><span data-ttu-id="584de-1127">请求</span><span class="sxs-lookup"><span data-stu-id="584de-1127">Request</span></span>
<span data-ttu-id="584de-1128">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="584de-1128">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 14888

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
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
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
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="584de-1129">响应</span><span class="sxs-lookup"><span data-stu-id="584de-1129">Response</span></span>
<span data-ttu-id="584de-p196">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="584de-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 15060

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
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
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
  "uninstallBuiltInApps": true
}
```





