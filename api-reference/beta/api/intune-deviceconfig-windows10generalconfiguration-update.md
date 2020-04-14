---
title: 更新 windows10GeneralConfiguration
description: 更新 windows10GeneralConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34183918522e9036aba005bac0086cbbc396e527
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430960"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="08a8a-103">更新 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="08a8a-103">Update windows10GeneralConfiguration</span></span>

<span data-ttu-id="08a8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08a8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08a8a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08a8a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08a8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08a8a-107">更新 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="08a8a-107">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08a8a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08a8a-108">Prerequisites</span></span>
<span data-ttu-id="08a8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08a8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08a8a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08a8a-111">Permission type</span></span>|<span data-ttu-id="08a8a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08a8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08a8a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08a8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08a8a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a8a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08a8a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08a8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08a8a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08a8a-116">Not supported.</span></span>|
|<span data-ttu-id="08a8a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08a8a-117">Application</span></span>|<span data-ttu-id="08a8a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a8a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08a8a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08a8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="08a8a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08a8a-120">Request headers</span></span>
|<span data-ttu-id="08a8a-121">标头</span><span class="sxs-lookup"><span data-stu-id="08a8a-121">Header</span></span>|<span data-ttu-id="08a8a-122">值</span><span class="sxs-lookup"><span data-stu-id="08a8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08a8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08a8a-123">Authorization</span></span>|<span data-ttu-id="08a8a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08a8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08a8a-125">接受</span><span class="sxs-lookup"><span data-stu-id="08a8a-125">Accept</span></span>|<span data-ttu-id="08a8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08a8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08a8a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08a8a-127">Request body</span></span>
<span data-ttu-id="08a8a-128">在请求正文中，提供 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-128">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="08a8a-129">下表显示了创建 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08a8a-129">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="08a8a-130">属性</span><span class="sxs-lookup"><span data-stu-id="08a8a-130">Property</span></span>|<span data-ttu-id="08a8a-131">类型</span><span class="sxs-lookup"><span data-stu-id="08a8a-131">Type</span></span>|<span data-ttu-id="08a8a-132">说明</span><span class="sxs-lookup"><span data-stu-id="08a8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08a8a-133">id</span><span class="sxs-lookup"><span data-stu-id="08a8a-133">id</span></span>|<span data-ttu-id="08a8a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="08a8a-134">String</span></span>|<span data-ttu-id="08a8a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="08a8a-135">Key of the entity.</span></span> <span data-ttu-id="08a8a-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08a8a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="08a8a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08a8a-138">DateTimeOffset</span></span>|<span data-ttu-id="08a8a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="08a8a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="08a8a-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08a8a-141">roleScopeTagIds</span></span>|<span data-ttu-id="08a8a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-142">String collection</span></span>|<span data-ttu-id="08a8a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08a8a-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="08a8a-145">supportsScopeTags</span></span>|<span data-ttu-id="08a8a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-146">Boolean</span></span>|<span data-ttu-id="08a8a-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="08a8a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08a8a-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="08a8a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08a8a-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="08a8a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08a8a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="08a8a-150">This property is read-only.</span></span> <span data-ttu-id="08a8a-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08a8a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="08a8a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08a8a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="08a8a-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="08a8a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="08a8a-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08a8a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="08a8a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08a8a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="08a8a-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="08a8a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="08a8a-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="08a8a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="08a8a-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="08a8a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="08a8a-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08a8a-164">createdDateTime</span></span>|<span data-ttu-id="08a8a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08a8a-165">DateTimeOffset</span></span>|<span data-ttu-id="08a8a-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="08a8a-166">DateTime the object was created.</span></span> <span data-ttu-id="08a8a-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-168">description</span><span class="sxs-lookup"><span data-stu-id="08a8a-168">description</span></span>|<span data-ttu-id="08a8a-169">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-169">String</span></span>|<span data-ttu-id="08a8a-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="08a8a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08a8a-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="08a8a-172">displayName</span></span>|<span data-ttu-id="08a8a-173">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-173">String</span></span>|<span data-ttu-id="08a8a-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="08a8a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08a8a-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-176">version</span><span class="sxs-lookup"><span data-stu-id="08a8a-176">version</span></span>|<span data-ttu-id="08a8a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-177">Int32</span></span>|<span data-ttu-id="08a8a-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="08a8a-178">Version of the device configuration.</span></span> <span data-ttu-id="08a8a-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08a8a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08a8a-180">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="08a8a-180">taskManagerBlockEndTask</span></span>|<span data-ttu-id="08a8a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-181">Boolean</span></span>|<span data-ttu-id="08a8a-182">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="08a8a-182">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="08a8a-183">energySaverOnBatteryThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="08a8a-183">energySaverOnBatteryThresholdPercentage</span></span>|<span data-ttu-id="08a8a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-184">Int32</span></span>|<span data-ttu-id="08a8a-185">此设置允许您指定节能程序打开时的电池电量水平。</span><span class="sxs-lookup"><span data-stu-id="08a8a-185">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="08a8a-186">在使用电池时，将自动打开（和低于）指定电池电量级别的节能保护程序。</span><span class="sxs-lookup"><span data-stu-id="08a8a-186">While on battery, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="08a8a-187">有效的输入范围（0-100）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-187">Valid input range (0-100).</span></span> <span data-ttu-id="08a8a-188">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="08a8a-188">Valid values 0 to 100</span></span>|
|<span data-ttu-id="08a8a-189">energySaverPluggedInThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="08a8a-189">energySaverPluggedInThresholdPercentage</span></span>|<span data-ttu-id="08a8a-190">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-190">Int32</span></span>|<span data-ttu-id="08a8a-191">此设置允许您指定节能程序打开时的电池电量水平。</span><span class="sxs-lookup"><span data-stu-id="08a8a-191">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="08a8a-192">接通电源时，将自动打开（和低于）指定电池电量级别的节能保护程序。</span><span class="sxs-lookup"><span data-stu-id="08a8a-192">While plugged in, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="08a8a-193">有效的输入范围（0-100）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-193">Valid input range (0-100).</span></span> <span data-ttu-id="08a8a-194">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="08a8a-194">Valid values 0 to 100</span></span>|
|<span data-ttu-id="08a8a-195">powerLidCloseActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="08a8a-195">powerLidCloseActionOnBattery</span></span>|[<span data-ttu-id="08a8a-196">powerActionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-196">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="08a8a-197">此设置指定当用户在使用电池时关闭移动电脑上的盖子时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-197">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while on battery.</span></span> <span data-ttu-id="08a8a-198">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-198">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="08a8a-199">powerLidCloseActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="08a8a-199">powerLidCloseActionPluggedIn</span></span>|[<span data-ttu-id="08a8a-200">powerActionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-200">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="08a8a-201">此设置指定当用户在插入时关闭移动 PC 上的盖子时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-201">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while plugged in.</span></span> <span data-ttu-id="08a8a-202">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-202">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="08a8a-203">powerButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="08a8a-203">powerButtonActionOnBattery</span></span>|[<span data-ttu-id="08a8a-204">powerActionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-204">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="08a8a-205">此设置指定当用户在使用电池时按下电源按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-205">This setting specifies the action that Windows takes when a user presses the Power button while on battery.</span></span> <span data-ttu-id="08a8a-206">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-206">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="08a8a-207">powerButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="08a8a-207">powerButtonActionPluggedIn</span></span>|[<span data-ttu-id="08a8a-208">powerActionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-208">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="08a8a-209">此设置指定当用户在插入时按下电源按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-209">This setting specifies the action that Windows takes when a user presses the Power button while plugged in.</span></span> <span data-ttu-id="08a8a-210">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-210">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="08a8a-211">powerSleepButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="08a8a-211">powerSleepButtonActionOnBattery</span></span>|[<span data-ttu-id="08a8a-212">powerActionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-212">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="08a8a-213">此设置指定当用户在使用电池时按 "睡眠" 按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-213">This setting specifies the action that Windows takes when a user presses the Sleep button while on battery.</span></span> <span data-ttu-id="08a8a-214">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-214">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="08a8a-215">powerSleepButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="08a8a-215">powerSleepButtonActionPluggedIn</span></span>|[<span data-ttu-id="08a8a-216">powerActionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-216">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="08a8a-217">此设置指定当用户在插入时按 "睡眠" 按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-217">This setting specifies the action that Windows takes when a user presses the Sleep button while plugged in.</span></span> <span data-ttu-id="08a8a-218">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-218">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="08a8a-219">powerHybridSleepOnBattery</span><span class="sxs-lookup"><span data-stu-id="08a8a-219">powerHybridSleepOnBattery</span></span>|[<span data-ttu-id="08a8a-220">启用</span><span class="sxs-lookup"><span data-stu-id="08a8a-220">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="08a8a-221">通过此设置，可以在使用电池时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="08a8a-221">This setting allows you to turn off hybrid sleep while on battery.</span></span> <span data-ttu-id="08a8a-222">如果将此设置设置为禁用，则当系统转换为睡眠（待机）时不会生成 hiberfile。</span><span class="sxs-lookup"><span data-stu-id="08a8a-222">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="08a8a-223">如果将此设置设置为启用或未配置此策略设置，则用户将控制此设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-223">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="08a8a-224">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-224">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-225">powerHybridSleepPluggedIn</span><span class="sxs-lookup"><span data-stu-id="08a8a-225">powerHybridSleepPluggedIn</span></span>|[<span data-ttu-id="08a8a-226">启用</span><span class="sxs-lookup"><span data-stu-id="08a8a-226">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="08a8a-227">此设置允许你在接通电源时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="08a8a-227">This setting allows you to turn off hybrid sleep while plugged in.</span></span> <span data-ttu-id="08a8a-228">如果将此设置设置为禁用，则当系统转换为睡眠（待机）时不会生成 hiberfile。</span><span class="sxs-lookup"><span data-stu-id="08a8a-228">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="08a8a-229">如果将此设置设置为启用或未配置此策略设置，则用户将控制此设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-229">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="08a8a-230">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-230">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-231">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="08a8a-231">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="08a8a-232">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="08a8a-232">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="08a8a-233">应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="08a8a-233">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="08a8a-234">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="08a8a-234">enableAutomaticRedeployment</span></span>|<span data-ttu-id="08a8a-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-235">Boolean</span></span>|<span data-ttu-id="08a8a-236">允许具有管理权限的用户在设备锁屏的屏幕上使用 CTRL + Win + R 删除所有用户数据和设置，以便可以自动重新配置设备并将其重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="08a8a-236">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="08a8a-237">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="08a8a-237">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="08a8a-238">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="08a8a-238">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="08a8a-239">控制 Microsoft 帐户登录助手（wlidsvc） NT 服务。</span><span class="sxs-lookup"><span data-stu-id="08a8a-239">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="08a8a-240">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-240">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-241">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="08a8a-241">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="08a8a-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-242">Boolean</span></span>|<span data-ttu-id="08a8a-243">允许辅助身份验证设备使用 Windows。</span><span class="sxs-lookup"><span data-stu-id="08a8a-243">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="08a8a-244">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="08a8a-244">authenticationWebSignIn</span></span>|[<span data-ttu-id="08a8a-245">启用</span><span class="sxs-lookup"><span data-stu-id="08a8a-245">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="08a8a-246">指示是否将启用 Web 凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="08a8a-246">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="08a8a-247">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-247">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-248">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="08a8a-248">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="08a8a-249">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-249">String</span></span>|<span data-ttu-id="08a8a-250">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="08a8a-250">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="08a8a-251">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="08a8a-251">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="08a8a-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-252">Boolean</span></span>|<span data-ttu-id="08a8a-253">指定是否允许或禁止联邦信息处理标准（FIPS）策略。</span><span class="sxs-lookup"><span data-stu-id="08a8a-253">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="08a8a-254">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="08a8a-254">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="08a8a-255">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-255">String collection</span></span>|<span data-ttu-id="08a8a-256">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-256">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="08a8a-257">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="08a8a-257">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="08a8a-258">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-258">String collection</span></span>|<span data-ttu-id="08a8a-259">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-259">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="08a8a-260">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="08a8a-260">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="08a8a-261">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-261">String</span></span>|<span data-ttu-id="08a8a-262">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="08a8a-262">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="08a8a-263">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="08a8a-263">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="08a8a-264">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-264">String</span></span>|<span data-ttu-id="08a8a-265">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="08a8a-265">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="08a8a-266">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="08a8a-266">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="08a8a-267">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-267">String</span></span>|<span data-ttu-id="08a8a-268">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="08a8a-268">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="08a8a-269">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="08a8a-269">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="08a8a-270">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-270">String</span></span>|<span data-ttu-id="08a8a-271">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="08a8a-271">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="08a8a-272">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="08a8a-272">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="08a8a-273">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-273">Int32</span></span>|<span data-ttu-id="08a8a-274">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="08a8a-274">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="08a8a-275">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="08a8a-275">This is a mobile only setting.</span></span> <span data-ttu-id="08a8a-276">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="08a8a-276">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="08a8a-277">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="08a8a-277">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="08a8a-278">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-278">String</span></span>|<span data-ttu-id="08a8a-279">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="08a8a-279">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="08a8a-280">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="08a8a-280">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="08a8a-281">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-281">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="08a8a-282">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-282">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="08a8a-283">选项可供 IT 管理员阻止跨设备同步，但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="08a8a-283">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="08a8a-284">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-284">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="08a8a-285">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="08a8a-285">messagingBlockSync</span></span>|<span data-ttu-id="08a8a-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-286">Boolean</span></span>|<span data-ttu-id="08a8a-287">指示是否在所有位置阻止短信备份和还原和消息传递。</span><span class="sxs-lookup"><span data-stu-id="08a8a-287">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="08a8a-288">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="08a8a-288">messagingBlockMMS</span></span>|<span data-ttu-id="08a8a-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-289">Boolean</span></span>|<span data-ttu-id="08a8a-290">指示是否阻止设备上的 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="08a8a-290">Indicates whether or not to block the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="08a8a-291">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="08a8a-291">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="08a8a-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-292">Boolean</span></span>|<span data-ttu-id="08a8a-293">指示是否阻止设备上的 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="08a8a-293">Indicates whether or not to block the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="08a8a-294">printerNames</span><span class="sxs-lookup"><span data-stu-id="08a8a-294">printerNames</span></span>|<span data-ttu-id="08a8a-295">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-295">String collection</span></span>|<span data-ttu-id="08a8a-296">根据打印机的名称（网络主机名称）自动预配打印机。</span><span class="sxs-lookup"><span data-stu-id="08a8a-296">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="08a8a-297">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="08a8a-297">printerDefaultName</span></span>|<span data-ttu-id="08a8a-298">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-298">String</span></span>|<span data-ttu-id="08a8a-299">已安装的打印机的名称（网络主机名称）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-299">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="08a8a-300">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="08a8a-300">printerBlockAddition</span></span>|<span data-ttu-id="08a8a-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-301">Boolean</span></span>|<span data-ttu-id="08a8a-302">阻止用户安装来自打印机设置的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="08a8a-302">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="08a8a-303">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="08a8a-303">searchBlockDiacritics</span></span>|<span data-ttu-id="08a8a-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-304">Boolean</span></span>|<span data-ttu-id="08a8a-305">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="08a8a-305">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="08a8a-306">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="08a8a-306">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="08a8a-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-307">Boolean</span></span>|<span data-ttu-id="08a8a-308">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="08a8a-308">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="08a8a-309">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="08a8a-309">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="08a8a-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-310">Boolean</span></span>|<span data-ttu-id="08a8a-311">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="08a8a-311">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="08a8a-312">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="08a8a-312">searchEnableRemoteQueries</span></span>|<span data-ttu-id="08a8a-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-313">Boolean</span></span>|<span data-ttu-id="08a8a-314">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="08a8a-314">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="08a8a-315">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="08a8a-315">searchDisableUseLocation</span></span>|<span data-ttu-id="08a8a-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-316">Boolean</span></span>|<span data-ttu-id="08a8a-317">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="08a8a-317">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="08a8a-318">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="08a8a-318">searchDisableLocation</span></span>|<span data-ttu-id="08a8a-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-319">Boolean</span></span>|<span data-ttu-id="08a8a-320">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="08a8a-320">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="08a8a-321">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="08a8a-321">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="08a8a-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-322">Boolean</span></span>|<span data-ttu-id="08a8a-323">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="08a8a-323">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="08a8a-324">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="08a8a-324">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="08a8a-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-325">Boolean</span></span>|<span data-ttu-id="08a8a-326">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="08a8a-326">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="08a8a-327">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="08a8a-327">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="08a8a-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-328">Boolean</span></span>|<span data-ttu-id="08a8a-329">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="08a8a-329">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="08a8a-330">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="08a8a-330">searchBlockWebResults</span></span>|<span data-ttu-id="08a8a-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-331">Boolean</span></span>|<span data-ttu-id="08a8a-332">指示是否阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="08a8a-332">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="08a8a-333">findMyFiles</span><span class="sxs-lookup"><span data-stu-id="08a8a-333">findMyFiles</span></span>|[<span data-ttu-id="08a8a-334">启用</span><span class="sxs-lookup"><span data-stu-id="08a8a-334">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="08a8a-335">控制用户是否可以将搜索配置为 "查找我的文件" 模式，该模式在辅助硬盘和用户配置文件外部搜索文件。</span><span class="sxs-lookup"><span data-stu-id="08a8a-335">Controls if the user can configure search to Find My Files mode, which searches files in secondary hard drives and also outside of the user profile.</span></span> <span data-ttu-id="08a8a-336">"查找我的文件" 不允许用户搜索文件或其不具有访问权限的位置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-336">Find My Files does not allow users to search files or locations to which they do not have access.</span></span> <span data-ttu-id="08a8a-337">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-337">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-338">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="08a8a-338">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="08a8a-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-339">Boolean</span></span>|<span data-ttu-id="08a8a-340">在设备已加入 Azure AD 时，指定是否允许在 OOBE 期间自动设备加密（仅限桌面）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-340">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="08a8a-341">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-341">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="08a8a-342">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-342">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="08a8a-343">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="08a8a-343">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="08a8a-344">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-344">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="08a8a-345">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="08a8a-345">oneDriveDisableFileSync</span></span>|<span data-ttu-id="08a8a-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-346">Boolean</span></span>|<span data-ttu-id="08a8a-347">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="08a8a-347">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="08a8a-348">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="08a8a-348">systemTelemetryProxyServer</span></span>|<span data-ttu-id="08a8a-349">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-349">String</span></span>|<span data-ttu-id="08a8a-350">获取或设置代理服务器的完全限定域名（FQDN）或 IP 地址，以转发连接的用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="08a8a-350">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="08a8a-351">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="08a8a-351">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="08a8a-352">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-352">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="08a8a-353">指定将哪种类型的遥测数据（无、intranet、internet、两者）发送到 Microsoft 365 Analytics。</span><span class="sxs-lookup"><span data-stu-id="08a8a-353">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="08a8a-354">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-354">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="08a8a-355">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="08a8a-355">inkWorkspaceAccess</span></span>|[<span data-ttu-id="08a8a-356">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-356">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="08a8a-357">控制用户对墨迹工作区的访问权限，从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="08a8a-357">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="08a8a-358">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-358">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-359">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="08a8a-359">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="08a8a-360">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-360">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="08a8a-361">控制用户对墨迹工作区的访问权限，从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="08a8a-361">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="08a8a-362">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-362">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="08a8a-363">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="08a8a-363">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="08a8a-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-364">Boolean</span></span>|<span data-ttu-id="08a8a-365">指定是否在墨迹工作区中显示建议的应用建议。</span><span class="sxs-lookup"><span data-stu-id="08a8a-365">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="08a8a-366">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="08a8a-366">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="08a8a-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-367">Boolean</span></span>|<span data-ttu-id="08a8a-368">此属性将在7月2019中弃用，并将替换为属性 SmartScreenAppInstallControl。</span><span class="sxs-lookup"><span data-stu-id="08a8a-368">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="08a8a-369">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-369">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="08a8a-370">smartScreenAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="08a8a-370">smartScreenAppInstallControl</span></span>|[<span data-ttu-id="08a8a-371">appInstallControlType</span><span class="sxs-lookup"><span data-stu-id="08a8a-371">appInstallControlType</span></span>](../resources/intune-deviceconfig-appinstallcontroltype.md)|<span data-ttu-id="08a8a-372">在 Windows 10 版本1703中添加。</span><span class="sxs-lookup"><span data-stu-id="08a8a-372">Added in Windows 10, version 1703.</span></span> <span data-ttu-id="08a8a-373">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-373">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span> <span data-ttu-id="08a8a-374">可取值为：`notConfigured`、`anywhere`、`storeOnly`、`recommendations`、`preferStore`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-374">Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.</span></span>|
|<span data-ttu-id="08a8a-375">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="08a8a-375">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="08a8a-376">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-376">String</span></span>|<span data-ttu-id="08a8a-377">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="08a8a-377">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="08a8a-378">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="08a8a-378">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="08a8a-379">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-379">String</span></span>|<span data-ttu-id="08a8a-380">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="08a8a-380">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="08a8a-381">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="08a8a-381">bluetoothAllowedServices</span></span>|<span data-ttu-id="08a8a-382">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-382">String collection</span></span>|<span data-ttu-id="08a8a-383">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-383">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="08a8a-384">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="08a8a-384">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="08a8a-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-385">Boolean</span></span>|<span data-ttu-id="08a8a-386">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="08a8a-386">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="08a8a-387">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="08a8a-387">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="08a8a-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-388">Boolean</span></span>|<span data-ttu-id="08a8a-389">是否阻止用户使用 Swift 对和其他基于邻近的应用场景。</span><span class="sxs-lookup"><span data-stu-id="08a8a-389">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="08a8a-390">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-390">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="08a8a-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-391">Boolean</span></span>|<span data-ttu-id="08a8a-392">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-392">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="08a8a-393">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="08a8a-393">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="08a8a-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-394">Boolean</span></span>|<span data-ttu-id="08a8a-395">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="08a8a-395">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="08a8a-396">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="08a8a-396">edgeBlockAutofill</span></span>|<span data-ttu-id="08a8a-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-397">Boolean</span></span>|<span data-ttu-id="08a8a-398">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="08a8a-398">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="08a8a-399">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-399">edgeBlocked</span></span>|<span data-ttu-id="08a8a-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-400">Boolean</span></span>|<span data-ttu-id="08a8a-401">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-401">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="08a8a-402">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="08a8a-402">edgeCookiePolicy</span></span>|[<span data-ttu-id="08a8a-403">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="08a8a-403">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="08a8a-404">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="08a8a-404">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="08a8a-405">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-405">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="08a8a-406">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="08a8a-406">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="08a8a-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-407">Boolean</span></span>|<span data-ttu-id="08a8a-408">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="08a8a-408">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="08a8a-409">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="08a8a-409">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="08a8a-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-410">Boolean</span></span>|<span data-ttu-id="08a8a-411">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="08a8a-411">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="08a8a-412">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="08a8a-412">edgeBlockExtensions</span></span>|<span data-ttu-id="08a8a-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-413">Boolean</span></span>|<span data-ttu-id="08a8a-414">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="08a8a-414">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="08a8a-415">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="08a8a-415">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="08a8a-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-416">Boolean</span></span>|<span data-ttu-id="08a8a-417">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="08a8a-417">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="08a8a-418">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="08a8a-418">edgeBlockJavaScript</span></span>|<span data-ttu-id="08a8a-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-419">Boolean</span></span>|<span data-ttu-id="08a8a-420">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="08a8a-420">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="08a8a-421">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="08a8a-421">edgeBlockPasswordManager</span></span>|<span data-ttu-id="08a8a-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-422">Boolean</span></span>|<span data-ttu-id="08a8a-423">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-423">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="08a8a-424">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="08a8a-424">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="08a8a-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-425">Boolean</span></span>|<span data-ttu-id="08a8a-426">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="08a8a-426">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="08a8a-427">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="08a8a-427">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="08a8a-428">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="08a8a-428">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="08a8a-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-429">Boolean</span></span>|<span data-ttu-id="08a8a-430">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-430">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="08a8a-431">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="08a8a-431">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="08a8a-432">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="08a8a-432">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="08a8a-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-433">Boolean</span></span>|<span data-ttu-id="08a8a-434">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="08a8a-434">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="08a8a-435">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="08a8a-435">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="08a8a-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-436">Boolean</span></span>|<span data-ttu-id="08a8a-437">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="08a8a-437">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="08a8a-438">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="08a8a-438">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="08a8a-439">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-439">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="08a8a-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-440">Boolean</span></span>|<span data-ttu-id="08a8a-441">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="08a8a-441">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="08a8a-442">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="08a8a-442">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="08a8a-443">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="08a8a-443">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="08a8a-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-444">Boolean</span></span>|<span data-ttu-id="08a8a-445">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="08a8a-445">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="08a8a-446">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="08a8a-446">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="08a8a-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-447">Boolean</span></span>|<span data-ttu-id="08a8a-448">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="08a8a-448">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="08a8a-449">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="08a8a-449">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="08a8a-450">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="08a8a-450">edgeFavoritesListLocation</span></span>|<span data-ttu-id="08a8a-451">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-451">String</span></span>|<span data-ttu-id="08a8a-452">要设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-452">The location of the favorites list to provision.</span></span> <span data-ttu-id="08a8a-453">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-453">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="08a8a-454">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="08a8a-454">edgeBlockEditFavorites</span></span>|<span data-ttu-id="08a8a-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-455">Boolean</span></span>|<span data-ttu-id="08a8a-456">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="08a8a-456">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="08a8a-457">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="08a8a-457">edgeNewTabPageURL</span></span>|<span data-ttu-id="08a8a-458">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-458">String</span></span>|<span data-ttu-id="08a8a-459">指定在创建新选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="08a8a-459">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="08a8a-460">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="08a8a-460">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="08a8a-461">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="08a8a-461">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="08a8a-462">使 Home 按钮可以隐藏、加载默认起始页、加载新的选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="08a8a-462">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="08a8a-463">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="08a8a-463">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="08a8a-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-464">Boolean</span></span>|<span data-ttu-id="08a8a-465">启用 "主页" 按钮配置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-465">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="08a8a-466">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="08a8a-466">edgeOpensWith</span></span>|[<span data-ttu-id="08a8a-467">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="08a8a-467">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="08a8a-468">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="08a8a-468">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="08a8a-469">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-469">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="08a8a-470">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="08a8a-470">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="08a8a-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-471">Boolean</span></span>|<span data-ttu-id="08a8a-472">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="08a8a-472">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="08a8a-473">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="08a8a-473">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="08a8a-474">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-474">String collection</span></span>|<span data-ttu-id="08a8a-475">指定所需的浏览器扩展的程序包系列名称列表，用户无法关闭这些扩展。</span><span class="sxs-lookup"><span data-stu-id="08a8a-475">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="08a8a-476">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="08a8a-476">edgeBlockPrinting</span></span>|<span data-ttu-id="08a8a-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-477">Boolean</span></span>|<span data-ttu-id="08a8a-478">将 Edge 配置为允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="08a8a-478">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="08a8a-479">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="08a8a-479">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="08a8a-480">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-480">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-481">获取或设置一个值，该值指定是否将收藏夹栏设置为始终在任何页面上都可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-481">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="08a8a-482">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-482">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-483">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="08a8a-483">edgeBlockSavingHistory</span></span>|<span data-ttu-id="08a8a-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-484">Boolean</span></span>|<span data-ttu-id="08a8a-485">将 Edge 配置为允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="08a8a-485">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="08a8a-486">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-486">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="08a8a-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-487">Boolean</span></span>|<span data-ttu-id="08a8a-488">允许或阻止边缘进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-488">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="08a8a-489">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-489">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="08a8a-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-490">Boolean</span></span>|<span data-ttu-id="08a8a-491">将配置为在 Edge 中加载空白页面，而不是默认的新选项卡页面，并防止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="08a8a-491">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="08a8a-492">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="08a8a-492">edgeBlockTabPreloading</span></span>|<span data-ttu-id="08a8a-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-493">Boolean</span></span>|<span data-ttu-id="08a8a-494">配置边缘是否在 Windows 启动时预加载新的选项卡页。</span><span class="sxs-lookup"><span data-stu-id="08a8a-494">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="08a8a-495">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="08a8a-495">edgeBlockPrelaunch</span></span>|<span data-ttu-id="08a8a-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-496">Boolean</span></span>|<span data-ttu-id="08a8a-497">确定 Microsoft Edge 在 Windows 启动时是否为 prelaunched。</span><span class="sxs-lookup"><span data-stu-id="08a8a-497">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="08a8a-498">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="08a8a-498">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="08a8a-499">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-499">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="08a8a-500">控制边缘在切换到 Internet Explorer 之前显示的消息。</span><span class="sxs-lookup"><span data-stu-id="08a8a-500">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="08a8a-501">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-501">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="08a8a-502">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="08a8a-502">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="08a8a-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-503">Boolean</span></span>|<span data-ttu-id="08a8a-504">允许或阻止用户覆盖证书错误。</span><span class="sxs-lookup"><span data-stu-id="08a8a-504">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="08a8a-505">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="08a8a-505">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="08a8a-506">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-506">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="08a8a-507">根据配置展台模式，控制 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-507">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="08a8a-508">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-508">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="08a8a-509">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="08a8a-509">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="08a8a-510">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-510">Int32</span></span>|<span data-ttu-id="08a8a-511">指定在 Microsoft Edge 展台重置前的上次用户活动的时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-511">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="08a8a-512">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="08a8a-512">Valid values are 0-1440.</span></span> <span data-ttu-id="08a8a-513">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="08a8a-513">The default is 5.</span></span> <span data-ttu-id="08a8a-514">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-514">0 indicates no reset.</span></span> <span data-ttu-id="08a8a-515">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="08a8a-515">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="08a8a-516">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="08a8a-516">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="08a8a-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-517">Boolean</span></span>|<span data-ttu-id="08a8a-518">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="08a8a-518">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="08a8a-519">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="08a8a-519">cellularBlockVpn</span></span>|<span data-ttu-id="08a8a-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-520">Boolean</span></span>|<span data-ttu-id="08a8a-521">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="08a8a-521">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="08a8a-522">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="08a8a-522">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="08a8a-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-523">Boolean</span></span>|<span data-ttu-id="08a8a-524">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="08a8a-524">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="08a8a-525">cellularData</span><span class="sxs-lookup"><span data-stu-id="08a8a-525">cellularData</span></span>|[<span data-ttu-id="08a8a-526">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="08a8a-526">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="08a8a-527">是否允许设备上的手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="08a8a-527">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="08a8a-528">如果未配置，则允许手机网络数据通道，用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="08a8a-528">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="08a8a-529">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-529">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="08a8a-530">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="08a8a-530">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="08a8a-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-531">Boolean</span></span>|<span data-ttu-id="08a8a-532">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="08a8a-532">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="08a8a-533">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="08a8a-533">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="08a8a-534">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-534">Int32</span></span>|<span data-ttu-id="08a8a-535">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="08a8a-535">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="08a8a-536">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="08a8a-536">Valid values 0 to 90</span></span>|
|<span data-ttu-id="08a8a-537">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="08a8a-537">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="08a8a-538">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="08a8a-538">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="08a8a-539">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="08a8a-539">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="08a8a-540">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="08a8a-540">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="08a8a-541">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="08a8a-541">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="08a8a-542">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="08a8a-542">Defender day of the week for the system scan.</span></span> <span data-ttu-id="08a8a-543">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-543">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="08a8a-544">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="08a8a-544">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="08a8a-545">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-545">String collection</span></span>|<span data-ttu-id="08a8a-546">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="08a8a-546">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="08a8a-547">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="08a8a-547">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="08a8a-548">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-548">String collection</span></span>|<span data-ttu-id="08a8a-549">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="08a8a-549">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="08a8a-550">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="08a8a-550">defenderScanMaxCpu</span></span>|<span data-ttu-id="08a8a-551">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-551">Int32</span></span>|<span data-ttu-id="08a8a-552">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="08a8a-552">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="08a8a-553">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="08a8a-553">Valid values 0 to 100</span></span>|
|<span data-ttu-id="08a8a-554">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="08a8a-554">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="08a8a-555">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="08a8a-555">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="08a8a-556">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="08a8a-556">Value for monitoring file activity.</span></span> <span data-ttu-id="08a8a-557">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-557">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="08a8a-558">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="08a8a-558">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="08a8a-559">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="08a8a-559">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="08a8a-560">获取或设置要对可能有害的应用程序（PUA）执行的 Defender 操作，其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时，Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="08a8a-560">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="08a8a-561">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="08a8a-561">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="08a8a-562">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-562">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="08a8a-563">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-563">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="08a8a-564">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="08a8a-564">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="08a8a-565">获取或设置要对可能有害的应用程序（PUA）执行的 Defender 操作，其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时，Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="08a8a-565">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="08a8a-566">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="08a8a-566">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="08a8a-567">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-567">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="08a8a-568">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="08a8a-568">defenderProcessesToExclude</span></span>|<span data-ttu-id="08a8a-569">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-569">String collection</span></span>|<span data-ttu-id="08a8a-570">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="08a8a-570">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="08a8a-571">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="08a8a-571">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="08a8a-572">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="08a8a-572">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="08a8a-573">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-573">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="08a8a-574">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-574">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="08a8a-575">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="08a8a-575">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="08a8a-576">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-576">Boolean</span></span>|<span data-ttu-id="08a8a-577">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="08a8a-577">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="08a8a-578">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="08a8a-578">defenderRequireCloudProtection</span></span>|<span data-ttu-id="08a8a-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-579">Boolean</span></span>|<span data-ttu-id="08a8a-580">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="08a8a-580">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="08a8a-581">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="08a8a-581">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="08a8a-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-582">Boolean</span></span>|<span data-ttu-id="08a8a-583">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="08a8a-583">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="08a8a-584">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="08a8a-584">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="08a8a-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-585">Boolean</span></span>|<span data-ttu-id="08a8a-586">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="08a8a-586">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="08a8a-587">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="08a8a-587">defenderScanArchiveFiles</span></span>|<span data-ttu-id="08a8a-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-588">Boolean</span></span>|<span data-ttu-id="08a8a-589">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="08a8a-589">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="08a8a-590">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="08a8a-590">defenderScanDownloads</span></span>|<span data-ttu-id="08a8a-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-591">Boolean</span></span>|<span data-ttu-id="08a8a-592">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="08a8a-592">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="08a8a-593">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="08a8a-593">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="08a8a-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-594">Boolean</span></span>|<span data-ttu-id="08a8a-595">启用后，在计划扫描期间将使用较低的 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="08a8a-595">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="08a8a-596">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="08a8a-596">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="08a8a-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-597">Boolean</span></span>|<span data-ttu-id="08a8a-598">当被阻止时，将关闭计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="08a8a-598">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="08a8a-599">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="08a8a-599">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="08a8a-600">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-600">Boolean</span></span>|<span data-ttu-id="08a8a-601">当被阻止时，计划的完全扫描的追赶扫描将被禁用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-601">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="08a8a-602">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="08a8a-602">defenderScanNetworkFiles</span></span>|<span data-ttu-id="08a8a-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-603">Boolean</span></span>|<span data-ttu-id="08a8a-604">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="08a8a-604">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="08a8a-605">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="08a8a-605">defenderScanIncomingMail</span></span>|<span data-ttu-id="08a8a-606">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-606">Boolean</span></span>|<span data-ttu-id="08a8a-607">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="08a8a-607">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="08a8a-608">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="08a8a-608">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="08a8a-609">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-609">Boolean</span></span>|<span data-ttu-id="08a8a-610">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-610">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="08a8a-611">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="08a8a-611">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="08a8a-612">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-612">Boolean</span></span>|<span data-ttu-id="08a8a-613">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-613">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="08a8a-614">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="08a8a-614">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="08a8a-615">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-615">Boolean</span></span>|<span data-ttu-id="08a8a-616">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="08a8a-616">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="08a8a-617">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="08a8a-617">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="08a8a-618">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-618">Int32</span></span>|<span data-ttu-id="08a8a-619">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-619">The signature update interval in hours.</span></span> <span data-ttu-id="08a8a-620">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="08a8a-620">Specify 0 not to check.</span></span> <span data-ttu-id="08a8a-621">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="08a8a-621">Valid values 0 to 24</span></span>|
|<span data-ttu-id="08a8a-622">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="08a8a-622">defenderScanType</span></span>|[<span data-ttu-id="08a8a-623">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="08a8a-623">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="08a8a-624">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="08a8a-624">The defender system scan type.</span></span> <span data-ttu-id="08a8a-625">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-625">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="08a8a-626">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="08a8a-626">defenderScheduledScanTime</span></span>|<span data-ttu-id="08a8a-627">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="08a8a-627">TimeOfDay</span></span>|<span data-ttu-id="08a8a-628">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="08a8a-628">The defender time for the system scan.</span></span>|
|<span data-ttu-id="08a8a-629">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="08a8a-629">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="08a8a-630">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="08a8a-630">TimeOfDay</span></span>|<span data-ttu-id="08a8a-631">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="08a8a-631">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="08a8a-632">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="08a8a-632">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="08a8a-633">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="08a8a-633">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="08a8a-634">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="08a8a-634">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="08a8a-635">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-635">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="08a8a-636">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="08a8a-636">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="08a8a-637">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-637">Int32</span></span>|<span data-ttu-id="08a8a-638">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="08a8a-638">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="08a8a-639">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="08a8a-639">Valid values 0 to 50</span></span>|
|<span data-ttu-id="08a8a-640">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="08a8a-640">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="08a8a-641">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-641">Int32</span></span>|<span data-ttu-id="08a8a-642">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="08a8a-642">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="08a8a-643">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="08a8a-643">Valid values 0 to 50</span></span>|
|<span data-ttu-id="08a8a-644">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="08a8a-644">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="08a8a-645">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-645">Boolean</span></span>|<span data-ttu-id="08a8a-646">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="08a8a-646">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="08a8a-647">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="08a8a-647">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="08a8a-648">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="08a8a-648">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="08a8a-649">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="08a8a-649">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="08a8a-650">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-650">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="08a8a-651">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="08a8a-651">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="08a8a-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-652">Boolean</span></span>|<span data-ttu-id="08a8a-653">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="08a8a-653">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="08a8a-654">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="08a8a-654">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="08a8a-655">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="08a8a-655">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="08a8a-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-656">Boolean</span></span>|<span data-ttu-id="08a8a-657">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="08a8a-657">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="08a8a-658">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="08a8a-658">lockScreenBlockCortana</span></span>|<span data-ttu-id="08a8a-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-659">Boolean</span></span>|<span data-ttu-id="08a8a-660">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="08a8a-660">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="08a8a-661">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="08a8a-661">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="08a8a-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-662">Boolean</span></span>|<span data-ttu-id="08a8a-663">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="08a8a-663">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="08a8a-664">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="08a8a-664">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="08a8a-665">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-665">Int32</span></span>|<span data-ttu-id="08a8a-666">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-666">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="08a8a-667">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="08a8a-667">Supported values are 11-1800.</span></span> <span data-ttu-id="08a8a-668">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="08a8a-668">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="08a8a-669">lockScreenActivateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="08a8a-669">lockScreenActivateAppsWithVoice</span></span>|[<span data-ttu-id="08a8a-670">启用</span><span class="sxs-lookup"><span data-stu-id="08a8a-670">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="08a8a-671">此策略设置指定在系统处于锁定状态时，Windows 应用是否可以通过语音激活。</span><span class="sxs-lookup"><span data-stu-id="08a8a-671">This policy setting specifies whether Windows apps can be activated by voice while the system is locked.</span></span> <span data-ttu-id="08a8a-672">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-672">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-673">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="08a8a-673">passwordBlockSimple</span></span>|<span data-ttu-id="08a8a-674">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-674">Boolean</span></span>|<span data-ttu-id="08a8a-675">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-675">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="08a8a-676">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-676">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="08a8a-677">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="08a8a-677">passwordExpirationDays</span></span>|<span data-ttu-id="08a8a-678">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-678">Int32</span></span>|<span data-ttu-id="08a8a-679">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="08a8a-679">The password expiration in days.</span></span> <span data-ttu-id="08a8a-680">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="08a8a-680">Valid values 0 to 730</span></span>|
|<span data-ttu-id="08a8a-681">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="08a8a-681">passwordMinimumLength</span></span>|<span data-ttu-id="08a8a-682">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-682">Int32</span></span>|<span data-ttu-id="08a8a-683">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="08a8a-683">The minimum password length.</span></span> <span data-ttu-id="08a8a-684">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="08a8a-684">Valid values 4 to 16</span></span>|
|<span data-ttu-id="08a8a-685">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="08a8a-685">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="08a8a-686">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-686">Int32</span></span>|<span data-ttu-id="08a8a-687">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="08a8a-687">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="08a8a-688">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="08a8a-688">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="08a8a-689">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-689">Int32</span></span>|<span data-ttu-id="08a8a-690">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="08a8a-690">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="08a8a-691">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="08a8a-691">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="08a8a-692">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-692">Int32</span></span>|<span data-ttu-id="08a8a-693">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="08a8a-693">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="08a8a-694">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="08a8a-694">Valid values 0 to 50</span></span>|
|<span data-ttu-id="08a8a-695">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="08a8a-695">passwordRequired</span></span>|<span data-ttu-id="08a8a-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-696">Boolean</span></span>|<span data-ttu-id="08a8a-697">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="08a8a-697">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="08a8a-698">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="08a8a-698">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="08a8a-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-699">Boolean</span></span>|<span data-ttu-id="08a8a-700">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="08a8a-700">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="08a8a-701">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="08a8a-701">passwordRequiredType</span></span>|[<span data-ttu-id="08a8a-702">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="08a8a-702">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="08a8a-703">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="08a8a-703">The required password type.</span></span> <span data-ttu-id="08a8a-704">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-704">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="08a8a-705">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="08a8a-705">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="08a8a-706">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-706">Int32</span></span>|<span data-ttu-id="08a8a-707">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="08a8a-707">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="08a8a-708">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="08a8a-708">Valid values 0 to 999</span></span>|
|<span data-ttu-id="08a8a-709">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="08a8a-709">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="08a8a-710">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-710">Int32</span></span>|<span data-ttu-id="08a8a-711">此安全设置确定用户可以更改密码之前必须使用该密码的时间（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-711">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="08a8a-712">有效值为0至998</span><span class="sxs-lookup"><span data-stu-id="08a8a-712">Valid values 0 to 998</span></span>|
|<span data-ttu-id="08a8a-713">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="08a8a-713">privacyAdvertisingId</span></span>|[<span data-ttu-id="08a8a-714">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-714">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="08a8a-715">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-715">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="08a8a-716">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="08a8a-716">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="08a8a-717">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-717">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="08a8a-718">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="08a8a-718">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="08a8a-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-719">Boolean</span></span>|<span data-ttu-id="08a8a-720">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="08a8a-720">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="08a8a-721">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="08a8a-721">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="08a8a-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-722">Boolean</span></span>|<span data-ttu-id="08a8a-723">此策略可防止在用户登录时为新的和已升级的用户启动隐私体验。</span><span class="sxs-lookup"><span data-stu-id="08a8a-723">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="08a8a-724">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="08a8a-724">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="08a8a-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-725">Boolean</span></span>|<span data-ttu-id="08a8a-726">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="08a8a-726">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="08a8a-727">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="08a8a-727">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="08a8a-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-728">Boolean</span></span>|<span data-ttu-id="08a8a-729">阻止共享体验和发现任务切换器等中的最近使用的资源。</span><span class="sxs-lookup"><span data-stu-id="08a8a-729">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="08a8a-730">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="08a8a-730">privacyBlockActivityFeed</span></span>|<span data-ttu-id="08a8a-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-731">Boolean</span></span>|<span data-ttu-id="08a8a-732">阻止 Cortana、听写或存储应用程序的基于云的语音服务的使用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-732">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="08a8a-733">activateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="08a8a-733">activateAppsWithVoice</span></span>|[<span data-ttu-id="08a8a-734">启用</span><span class="sxs-lookup"><span data-stu-id="08a8a-734">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="08a8a-735">指定是否可以通过语音激活 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-735">Specifies if Windows apps can be activated by voice.</span></span> <span data-ttu-id="08a8a-736">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-736">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="08a8a-737">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="08a8a-737">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="08a8a-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-738">Boolean</span></span>|<span data-ttu-id="08a8a-739">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-739">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="08a8a-740">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="08a8a-740">startMenuAppListVisibility</span></span>|[<span data-ttu-id="08a8a-741">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="08a8a-741">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="08a8a-742">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="08a8a-742">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="08a8a-743">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-743">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="08a8a-744">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="08a8a-744">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="08a8a-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-745">Boolean</span></span>|<span data-ttu-id="08a8a-746">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-746">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="08a8a-747">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="08a8a-747">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="08a8a-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-748">Boolean</span></span>|<span data-ttu-id="08a8a-749">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="08a8a-749">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="08a8a-750">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="08a8a-750">startMenuHideHibernate</span></span>|<span data-ttu-id="08a8a-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-751">Boolean</span></span>|<span data-ttu-id="08a8a-752">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-752">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="08a8a-753">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="08a8a-753">startMenuHideLock</span></span>|<span data-ttu-id="08a8a-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-754">Boolean</span></span>|<span data-ttu-id="08a8a-755">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-755">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="08a8a-756">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="08a8a-756">startMenuHidePowerButton</span></span>|<span data-ttu-id="08a8a-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-757">Boolean</span></span>|<span data-ttu-id="08a8a-758">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-758">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="08a8a-759">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="08a8a-759">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="08a8a-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-760">Boolean</span></span>|<span data-ttu-id="08a8a-761">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="08a8a-761">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="08a8a-762">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="08a8a-762">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="08a8a-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-763">Boolean</span></span>|<span data-ttu-id="08a8a-764">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="08a8a-764">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="08a8a-765">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="08a8a-765">startMenuHideRestartOptions</span></span>|<span data-ttu-id="08a8a-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-766">Boolean</span></span>|<span data-ttu-id="08a8a-767">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-767">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="08a8a-768">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="08a8a-768">startMenuHideShutDown</span></span>|<span data-ttu-id="08a8a-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-769">Boolean</span></span>|<span data-ttu-id="08a8a-770">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-770">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="08a8a-771">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="08a8a-771">startMenuHideSignOut</span></span>|<span data-ttu-id="08a8a-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-772">Boolean</span></span>|<span data-ttu-id="08a8a-773">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-773">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="08a8a-774">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="08a8a-774">startMenuHideSleep</span></span>|<span data-ttu-id="08a8a-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-775">Boolean</span></span>|<span data-ttu-id="08a8a-776">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-776">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="08a8a-777">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="08a8a-777">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="08a8a-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-778">Boolean</span></span>|<span data-ttu-id="08a8a-779">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-779">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="08a8a-780">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="08a8a-780">startMenuHideUserTile</span></span>|<span data-ttu-id="08a8a-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-781">Boolean</span></span>|<span data-ttu-id="08a8a-782">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="08a8a-782">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="08a8a-783">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="08a8a-783">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="08a8a-784">Binary</span><span class="sxs-lookup"><span data-stu-id="08a8a-784">Binary</span></span>|<span data-ttu-id="08a8a-785">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-785">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="08a8a-786">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="08a8a-786">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="08a8a-787">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="08a8a-787">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="08a8a-788">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="08a8a-788">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="08a8a-789">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="08a8a-789">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="08a8a-790">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="08a8a-790">startMenuLayoutXml</span></span>|<span data-ttu-id="08a8a-791">Binary</span><span class="sxs-lookup"><span data-stu-id="08a8a-791">Binary</span></span>|<span data-ttu-id="08a8a-792">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="08a8a-792">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="08a8a-793">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="08a8a-793">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="08a8a-794">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-794">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="08a8a-795">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="08a8a-795">startMenuMode</span></span>|[<span data-ttu-id="08a8a-796">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="08a8a-796">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="08a8a-797">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-797">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="08a8a-798">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-798">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="08a8a-799">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="08a8a-799">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="08a8a-800">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-800">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-801">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-801">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-802">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-802">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-803">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="08a8a-803">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="08a8a-804">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-804">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-805">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-805">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-806">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-806">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-807">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="08a8a-807">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="08a8a-808">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-808">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-809">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-809">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-810">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-810">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-811">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="08a8a-811">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="08a8a-812">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-812">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-813">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-813">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-814">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-814">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-815">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="08a8a-815">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="08a8a-816">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-816">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-817">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-817">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-818">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-818">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-819">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="08a8a-819">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="08a8a-820">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-820">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-821">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-821">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-822">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-822">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-823">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="08a8a-823">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="08a8a-824">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-824">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-825">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-825">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-826">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-826">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-827">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="08a8a-827">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="08a8a-828">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-828">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-829">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-829">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-830">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-830">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-831">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="08a8a-831">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="08a8a-832">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-832">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-833">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-833">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-834">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-834">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-835">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="08a8a-835">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="08a8a-836">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-836">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="08a8a-837">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-837">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="08a8a-838">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-838">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="08a8a-839">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="08a8a-839">settingsBlockSettingsApp</span></span>|<span data-ttu-id="08a8a-840">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-840">Boolean</span></span>|<span data-ttu-id="08a8a-841">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-841">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="08a8a-842">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-842">settingsBlockSystemPage</span></span>|<span data-ttu-id="08a8a-843">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-843">Boolean</span></span>|<span data-ttu-id="08a8a-844">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="08a8a-844">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="08a8a-845">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-845">settingsBlockDevicesPage</span></span>|<span data-ttu-id="08a8a-846">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-846">Boolean</span></span>|<span data-ttu-id="08a8a-847">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="08a8a-847">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="08a8a-848">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-848">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="08a8a-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-849">Boolean</span></span>|<span data-ttu-id="08a8a-850">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-850">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="08a8a-851">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-851">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="08a8a-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-852">Boolean</span></span>|<span data-ttu-id="08a8a-853">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-853">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="08a8a-854">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-854">settingsBlockAccountsPage</span></span>|<span data-ttu-id="08a8a-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-855">Boolean</span></span>|<span data-ttu-id="08a8a-856">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-856">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="08a8a-857">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="08a8a-857">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="08a8a-858">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-858">Boolean</span></span>|<span data-ttu-id="08a8a-859">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-859">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="08a8a-860">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-860">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="08a8a-861">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-861">Boolean</span></span>|<span data-ttu-id="08a8a-862">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-862">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="08a8a-863">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-863">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="08a8a-864">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-864">Boolean</span></span>|<span data-ttu-id="08a8a-865">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-865">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="08a8a-866">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-866">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="08a8a-867">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-867">Boolean</span></span>|<span data-ttu-id="08a8a-868">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-868">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="08a8a-869">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-869">settingsBlockAppsPage</span></span>|<span data-ttu-id="08a8a-870">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-870">Boolean</span></span>|<span data-ttu-id="08a8a-871">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-871">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="08a8a-872">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="08a8a-872">settingsBlockGamingPage</span></span>|<span data-ttu-id="08a8a-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-873">Boolean</span></span>|<span data-ttu-id="08a8a-874">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-874">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="08a8a-875">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="08a8a-875">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="08a8a-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-876">Boolean</span></span>|<span data-ttu-id="08a8a-877">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="08a8a-877">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="08a8a-878">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-878">windowsSpotlightBlocked</span></span>|<span data-ttu-id="08a8a-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-879">Boolean</span></span>|<span data-ttu-id="08a8a-880">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="08a8a-880">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="08a8a-881">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="08a8a-881">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="08a8a-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-882">Boolean</span></span>|<span data-ttu-id="08a8a-883">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="08a8a-883">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="08a8a-884">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="08a8a-884">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="08a8a-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-885">Boolean</span></span>|<span data-ttu-id="08a8a-886">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="08a8a-886">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="08a8a-887">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="08a8a-887">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="08a8a-888">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-888">Boolean</span></span>|<span data-ttu-id="08a8a-889">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="08a8a-889">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="08a8a-890">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="08a8a-890">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="08a8a-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-891">Boolean</span></span>|<span data-ttu-id="08a8a-892">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="08a8a-892">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="08a8a-893">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="08a8a-893">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="08a8a-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-894">Boolean</span></span>|<span data-ttu-id="08a8a-895">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="08a8a-895">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="08a8a-896">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="08a8a-896">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="08a8a-897">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="08a8a-897">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="08a8a-898">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="08a8a-898">Specifies the type of Spotlight.</span></span> <span data-ttu-id="08a8a-899">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-899">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="08a8a-900">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="08a8a-900">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="08a8a-901">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-901">Boolean</span></span>|<span data-ttu-id="08a8a-902">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="08a8a-902">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="08a8a-903">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="08a8a-903">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="08a8a-904">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="08a8a-904">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="08a8a-905">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-905">Boolean</span></span>|<span data-ttu-id="08a8a-906">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-906">Disable automatic detection of settings.</span></span> <span data-ttu-id="08a8a-907">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="08a8a-907">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="08a8a-908">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="08a8a-908">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="08a8a-909">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-909">String</span></span>|<span data-ttu-id="08a8a-910">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="08a8a-910">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="08a8a-911">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="08a8a-911">networkProxyServer</span></span>|[<span data-ttu-id="08a8a-912">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="08a8a-912">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="08a8a-913">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-913">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="08a8a-914">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="08a8a-914">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="08a8a-915">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-915">Boolean</span></span>|<span data-ttu-id="08a8a-916">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="08a8a-916">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="08a8a-917">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-917">antiTheftModeBlocked</span></span>|<span data-ttu-id="08a8a-918">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-918">Boolean</span></span>|<span data-ttu-id="08a8a-919">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="08a8a-919">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="08a8a-920">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-920">bluetoothBlocked</span></span>|<span data-ttu-id="08a8a-921">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-921">Boolean</span></span>|<span data-ttu-id="08a8a-922">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="08a8a-922">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="08a8a-923">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-923">cameraBlocked</span></span>|<span data-ttu-id="08a8a-924">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-924">Boolean</span></span>|<span data-ttu-id="08a8a-925">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="08a8a-925">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="08a8a-926">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-926">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="08a8a-927">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-927">Boolean</span></span>|<span data-ttu-id="08a8a-928">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="08a8a-928">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="08a8a-929">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="08a8a-929">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="08a8a-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-930">Boolean</span></span>|<span data-ttu-id="08a8a-931">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="08a8a-931">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="08a8a-932">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-932">copyPasteBlocked</span></span>|<span data-ttu-id="08a8a-933">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-933">Boolean</span></span>|<span data-ttu-id="08a8a-934">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="08a8a-934">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="08a8a-935">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-935">cortanaBlocked</span></span>|<span data-ttu-id="08a8a-936">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-936">Boolean</span></span>|<span data-ttu-id="08a8a-937">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="08a8a-937">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="08a8a-938">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="08a8a-938">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="08a8a-939">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-939">Boolean</span></span>|<span data-ttu-id="08a8a-940">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="08a8a-940">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="08a8a-941">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="08a8a-941">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="08a8a-942">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-942">Boolean</span></span>|<span data-ttu-id="08a8a-943">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="08a8a-943">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="08a8a-944">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="08a8a-944">safeSearchFilter</span></span>|[<span data-ttu-id="08a8a-945">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="08a8a-945">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="08a8a-946">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="08a8a-946">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="08a8a-947">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-947">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="08a8a-948">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="08a8a-948">edgeBlockPopups</span></span>|<span data-ttu-id="08a8a-949">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-949">Boolean</span></span>|<span data-ttu-id="08a8a-950">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="08a8a-950">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="08a8a-951">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="08a8a-951">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="08a8a-952">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-952">Boolean</span></span>|<span data-ttu-id="08a8a-953">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="08a8a-953">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="08a8a-954">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="08a8a-954">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="08a8a-955">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-955">Boolean</span></span>|<span data-ttu-id="08a8a-956">指示是否阻止用户添加新的搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="08a8a-956">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="08a8a-957">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="08a8a-957">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="08a8a-958">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-958">Boolean</span></span>|<span data-ttu-id="08a8a-959">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="08a8a-959">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="08a8a-960">注意：此属性的名称是误导性的;属性已过时，请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="08a8a-960">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="08a8a-961">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="08a8a-961">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="08a8a-962">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-962">Boolean</span></span>|<span data-ttu-id="08a8a-963">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="08a8a-963">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="08a8a-964">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="08a8a-964">edgeRequireSmartScreen</span></span>|<span data-ttu-id="08a8a-965">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-965">Boolean</span></span>|<span data-ttu-id="08a8a-966">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-966">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="08a8a-967">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="08a8a-967">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="08a8a-968">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-968">String</span></span>|<span data-ttu-id="08a8a-969">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-969">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="08a8a-970">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-970">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="08a8a-971">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="08a8a-971">edgeFirstRunUrl</span></span>|<span data-ttu-id="08a8a-972">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-972">String</span></span>|<span data-ttu-id="08a8a-973">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="08a8a-973">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="08a8a-974">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="08a8a-974">edgeSearchEngine</span></span>|[<span data-ttu-id="08a8a-975">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="08a8a-975">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="08a8a-976">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="08a8a-976">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="08a8a-977">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="08a8a-977">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="08a8a-978">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="08a8a-978">edgeHomepageUrls</span></span>|<span data-ttu-id="08a8a-979">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-979">String collection</span></span>|<span data-ttu-id="08a8a-980">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-980">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="08a8a-981">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="08a8a-981">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="08a8a-982">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-982">Boolean</span></span>|<span data-ttu-id="08a8a-983">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="08a8a-983">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="08a8a-984">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="08a8a-984">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="08a8a-985">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-985">Boolean</span></span>|<span data-ttu-id="08a8a-986">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="08a8a-986">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="08a8a-987">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="08a8a-987">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="08a8a-988">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-988">Boolean</span></span>|<span data-ttu-id="08a8a-989">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="08a8a-989">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="08a8a-990">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="08a8a-990">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="08a8a-991">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-991">Boolean</span></span>|<span data-ttu-id="08a8a-992">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="08a8a-992">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="08a8a-993">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-993">internetSharingBlocked</span></span>|<span data-ttu-id="08a8a-994">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-994">Boolean</span></span>|<span data-ttu-id="08a8a-995">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="08a8a-995">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="08a8a-996">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="08a8a-996">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="08a8a-997">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-997">Boolean</span></span>|<span data-ttu-id="08a8a-998">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="08a8a-998">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="08a8a-999">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="08a8a-999">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="08a8a-1000">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1000">Boolean</span></span>|<span data-ttu-id="08a8a-1001">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1001">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="08a8a-1002">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="08a8a-1002">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="08a8a-1003">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1003">Boolean</span></span>|<span data-ttu-id="08a8a-1004">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1004">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="08a8a-1005">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="08a8a-1005">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="08a8a-1006">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1006">Boolean</span></span>|<span data-ttu-id="08a8a-1007">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1007">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="08a8a-1008">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="08a8a-1008">settingsBlockChangeRegion</span></span>|<span data-ttu-id="08a8a-1009">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1009">Boolean</span></span>|<span data-ttu-id="08a8a-1010">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1010">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="08a8a-1011">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="08a8a-1011">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="08a8a-1012">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1012">Boolean</span></span>|<span data-ttu-id="08a8a-1013">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1013">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="08a8a-1014">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="08a8a-1014">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="08a8a-1015">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1015">Boolean</span></span>|<span data-ttu-id="08a8a-1016">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1016">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="08a8a-1017">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1017">locationServicesBlocked</span></span>|<span data-ttu-id="08a8a-1018">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1018">Boolean</span></span>|<span data-ttu-id="08a8a-1019">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1019">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="08a8a-1020">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1020">microsoftAccountBlocked</span></span>|<span data-ttu-id="08a8a-1021">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1021">Boolean</span></span>|<span data-ttu-id="08a8a-1022">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1022">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="08a8a-1023">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="08a8a-1023">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="08a8a-1024">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1024">Boolean</span></span>|<span data-ttu-id="08a8a-1025">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1025">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="08a8a-1026">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1026">nfcBlocked</span></span>|<span data-ttu-id="08a8a-1027">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1027">Boolean</span></span>|<span data-ttu-id="08a8a-1028">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1028">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="08a8a-1029">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1029">resetProtectionModeBlocked</span></span>|<span data-ttu-id="08a8a-1030">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1030">Boolean</span></span>|<span data-ttu-id="08a8a-1031">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1031">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="08a8a-1032">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1032">screenCaptureBlocked</span></span>|<span data-ttu-id="08a8a-1033">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1033">Boolean</span></span>|<span data-ttu-id="08a8a-1034">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1034">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="08a8a-1035">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="08a8a-1035">storageBlockRemovableStorage</span></span>|<span data-ttu-id="08a8a-1036">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1036">Boolean</span></span>|<span data-ttu-id="08a8a-1037">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1037">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="08a8a-1038">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="08a8a-1038">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="08a8a-1039">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1039">Boolean</span></span>|<span data-ttu-id="08a8a-1040">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1040">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="08a8a-1041">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1041">usbBlocked</span></span>|<span data-ttu-id="08a8a-1042">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1042">Boolean</span></span>|<span data-ttu-id="08a8a-1043">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1043">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="08a8a-1044">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1044">voiceRecordingBlocked</span></span>|<span data-ttu-id="08a8a-1045">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1045">Boolean</span></span>|<span data-ttu-id="08a8a-1046">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1046">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="08a8a-1047">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="08a8a-1047">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="08a8a-1048">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1048">Boolean</span></span>|<span data-ttu-id="08a8a-1049">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1049">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="08a8a-1050">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1050">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="08a8a-1051">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1051">wiFiBlocked</span></span>|<span data-ttu-id="08a8a-1052">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1052">Boolean</span></span>|<span data-ttu-id="08a8a-1053">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1053">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="08a8a-1054">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="08a8a-1054">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="08a8a-1055">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1055">Boolean</span></span>|<span data-ttu-id="08a8a-1056">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1056">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="08a8a-1057">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="08a8a-1057">wiFiScanInterval</span></span>|<span data-ttu-id="08a8a-1058">Int32</span><span class="sxs-lookup"><span data-stu-id="08a8a-1058">Int32</span></span>|<span data-ttu-id="08a8a-1059">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1059">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="08a8a-1060">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1060">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="08a8a-1061">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="08a8a-1061">Valid values 1 to 500</span></span>|
|<span data-ttu-id="08a8a-1062">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="08a8a-1062">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="08a8a-1063">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1063">Boolean</span></span>|<span data-ttu-id="08a8a-1064">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1064">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="08a8a-1065">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="08a8a-1065">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="08a8a-1066">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1066">Boolean</span></span>|<span data-ttu-id="08a8a-1067">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1067">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="08a8a-1068">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="08a8a-1068">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="08a8a-1069">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1069">Boolean</span></span>|<span data-ttu-id="08a8a-1070">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1070">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="08a8a-1071">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1071">windowsStoreBlocked</span></span>|<span data-ttu-id="08a8a-1072">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1072">Boolean</span></span>|<span data-ttu-id="08a8a-1073">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1073">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="08a8a-1074">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="08a8a-1074">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="08a8a-1075">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-1075">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="08a8a-1076">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1076">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="08a8a-1077">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1077">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="08a8a-1078">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="08a8a-1078">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="08a8a-1079">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1079">Boolean</span></span>|<span data-ttu-id="08a8a-1080">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1080">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="08a8a-1081">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-1081">developerUnlockSetting</span></span>|[<span data-ttu-id="08a8a-1082">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="08a8a-1082">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="08a8a-1083">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1083">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="08a8a-1084">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1084">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="08a8a-1085">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="08a8a-1085">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="08a8a-1086">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1086">Boolean</span></span>|<span data-ttu-id="08a8a-1087">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1087">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="08a8a-1088">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="08a8a-1088">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="08a8a-1089">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1089">Boolean</span></span>|<span data-ttu-id="08a8a-1090">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1090">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="08a8a-1091">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="08a8a-1091">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="08a8a-1092">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1092">Boolean</span></span>|<span data-ttu-id="08a8a-1093">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1093">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="08a8a-1094">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="08a8a-1094">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="08a8a-1095">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1095">Boolean</span></span>|<span data-ttu-id="08a8a-1096">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1096">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="08a8a-1097">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="08a8a-1097">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="08a8a-1098">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1098">Boolean</span></span>|<span data-ttu-id="08a8a-1099">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1099">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="08a8a-1100">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="08a8a-1100">gameDvrBlocked</span></span>|<span data-ttu-id="08a8a-1101">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1101">Boolean</span></span>|<span data-ttu-id="08a8a-1102">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1102">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="08a8a-1103">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="08a8a-1103">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="08a8a-1104">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1104">Boolean</span></span>|<span data-ttu-id="08a8a-1105">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1105">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="08a8a-1106">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="08a8a-1106">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="08a8a-1107">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1107">Boolean</span></span>|<span data-ttu-id="08a8a-1108">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1108">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="08a8a-1109">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="08a8a-1109">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="08a8a-1110">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1110">Boolean</span></span>|<span data-ttu-id="08a8a-1111">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1111">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="08a8a-1112">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="08a8a-1112">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="08a8a-1113">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1113">Boolean</span></span>|<span data-ttu-id="08a8a-1114">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1114">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="08a8a-1115">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="08a8a-1115">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="08a8a-1116">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1116">Boolean</span></span>|<span data-ttu-id="08a8a-1117">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1117">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="08a8a-1118">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="08a8a-1118">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="08a8a-1119">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1119">Boolean</span></span>|<span data-ttu-id="08a8a-1120">此策略设置允许用户更改通常仅供系统管理员使用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1120">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="08a8a-1121">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="08a8a-1121">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="08a8a-1122">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1122">Boolean</span></span>|<span data-ttu-id="08a8a-1123">此策略设置指示 Windows Installer 在系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1123">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="08a8a-1124">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="08a8a-1124">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="08a8a-1125">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1125">Boolean</span></span>|<span data-ttu-id="08a8a-1126">通过此策略设置，您可以阻止所有热插拔 PCI 下游端口的直接内存访问（DMA），直到用户登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1126">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="08a8a-1127">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="08a8a-1127">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="08a8a-1128">String 集合</span><span class="sxs-lookup"><span data-stu-id="08a8a-1128">String collection</span></span>|<span data-ttu-id="08a8a-1129">Windows 应用的以分号分隔的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1129">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="08a8a-1130">登录后将启动列出的 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1130">Listed Windows apps are to be launched after logon.</span></span>|
|<span data-ttu-id="08a8a-1131">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="08a8a-1131">uninstallBuiltInApps</span></span>|<span data-ttu-id="08a8a-1132">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a8a-1132">Boolean</span></span>|<span data-ttu-id="08a8a-1133">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1133">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|
|<span data-ttu-id="08a8a-1134">configureTimeZone</span><span class="sxs-lookup"><span data-stu-id="08a8a-1134">configureTimeZone</span></span>|<span data-ttu-id="08a8a-1135">String</span><span class="sxs-lookup"><span data-stu-id="08a8a-1135">String</span></span>|<span data-ttu-id="08a8a-1136">指定要应用于设备的时区。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1136">Specifies the time zone to be applied to the device.</span></span> <span data-ttu-id="08a8a-1137">这是目标时区的标准 Windows 名称。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1137">This is the standard Windows name for the target time zone.</span></span>|



## <a name="response"></a><span data-ttu-id="08a8a-1138">响应</span><span class="sxs-lookup"><span data-stu-id="08a8a-1138">Response</span></span>
<span data-ttu-id="08a8a-1139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1139">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08a8a-1140">示例</span><span class="sxs-lookup"><span data-stu-id="08a8a-1140">Example</span></span>

### <a name="request"></a><span data-ttu-id="08a8a-1141">请求</span><span class="sxs-lookup"><span data-stu-id="08a8a-1141">Request</span></span>
<span data-ttu-id="08a8a-1142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08a8a-1142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="08a8a-1143">响应</span><span class="sxs-lookup"><span data-stu-id="08a8a-1143">Response</span></span>
<span data-ttu-id="08a8a-p199">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08a8a-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



