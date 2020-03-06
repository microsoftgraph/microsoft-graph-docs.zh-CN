---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f97e5a4fbea34b4256f8b5aee4bb5b281586815
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42479973"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="bd5a3-103">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5a3-103">Create windows10GeneralConfiguration</span></span>

<span data-ttu-id="bd5a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd5a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd5a3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd5a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd5a3-107">创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-107">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd5a3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd5a3-108">Prerequisites</span></span>
<span data-ttu-id="bd5a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd5a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd5a3-111">Permission type</span></span>|<span data-ttu-id="bd5a3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd5a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd5a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd5a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd5a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd5a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd5a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd5a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd5a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-116">Not supported.</span></span>|
|<span data-ttu-id="bd5a3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd5a3-117">Application</span></span>|<span data-ttu-id="bd5a3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd5a3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd5a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd5a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd5a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd5a3-120">Request headers</span></span>
|<span data-ttu-id="bd5a3-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd5a3-121">Header</span></span>|<span data-ttu-id="bd5a3-122">值</span><span class="sxs-lookup"><span data-stu-id="bd5a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd5a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd5a3-123">Authorization</span></span>|<span data-ttu-id="bd5a3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd5a3-125">接受</span><span class="sxs-lookup"><span data-stu-id="bd5a3-125">Accept</span></span>|<span data-ttu-id="bd5a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd5a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd5a3-127">Request body</span></span>
<span data-ttu-id="bd5a3-128">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-128">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="bd5a3-129">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-129">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="bd5a3-130">属性</span><span class="sxs-lookup"><span data-stu-id="bd5a3-130">Property</span></span>|<span data-ttu-id="bd5a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="bd5a3-131">Type</span></span>|<span data-ttu-id="bd5a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="bd5a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd5a3-133">id</span><span class="sxs-lookup"><span data-stu-id="bd5a3-133">id</span></span>|<span data-ttu-id="bd5a3-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-134">String</span></span>|<span data-ttu-id="bd5a3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-135">Key of the entity.</span></span> <span data-ttu-id="bd5a3-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5a3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bd5a3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5a3-138">DateTimeOffset</span></span>|<span data-ttu-id="bd5a3-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bd5a3-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd5a3-141">roleScopeTagIds</span></span>|<span data-ttu-id="bd5a3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-142">String collection</span></span>|<span data-ttu-id="bd5a3-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd5a3-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bd5a3-145">supportsScopeTags</span></span>|<span data-ttu-id="bd5a3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-146">Boolean</span></span>|<span data-ttu-id="bd5a3-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bd5a3-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bd5a3-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bd5a3-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-150">This property is read-only.</span></span> <span data-ttu-id="bd5a3-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bd5a3-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bd5a3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bd5a3-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bd5a3-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bd5a3-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bd5a3-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bd5a3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bd5a3-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bd5a3-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bd5a3-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bd5a3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bd5a3-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bd5a3-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5a3-164">createdDateTime</span></span>|<span data-ttu-id="bd5a3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5a3-165">DateTimeOffset</span></span>|<span data-ttu-id="bd5a3-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-166">DateTime the object was created.</span></span> <span data-ttu-id="bd5a3-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-168">说明</span><span class="sxs-lookup"><span data-stu-id="bd5a3-168">description</span></span>|<span data-ttu-id="bd5a3-169">String</span><span class="sxs-lookup"><span data-stu-id="bd5a3-169">String</span></span>|<span data-ttu-id="bd5a3-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd5a3-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bd5a3-172">displayName</span></span>|<span data-ttu-id="bd5a3-173">String</span><span class="sxs-lookup"><span data-stu-id="bd5a3-173">String</span></span>|<span data-ttu-id="bd5a3-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd5a3-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-176">version</span><span class="sxs-lookup"><span data-stu-id="bd5a3-176">version</span></span>|<span data-ttu-id="bd5a3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-177">Int32</span></span>|<span data-ttu-id="bd5a3-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-178">Version of the device configuration.</span></span> <span data-ttu-id="bd5a3-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd5a3-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5a3-180">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="bd5a3-180">taskManagerBlockEndTask</span></span>|<span data-ttu-id="bd5a3-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-181">Boolean</span></span>|<span data-ttu-id="bd5a3-182">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-182">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="bd5a3-183">energySaverOnBatteryThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-183">energySaverOnBatteryThresholdPercentage</span></span>|<span data-ttu-id="bd5a3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-184">Int32</span></span>|<span data-ttu-id="bd5a3-185">此设置允许您指定节能程序打开时的电池电量水平。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-185">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="bd5a3-186">在使用电池时，将自动打开（和低于）指定电池电量级别的节能保护程序。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-186">While on battery, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="bd5a3-187">有效的输入范围（0-100）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-187">Valid input range (0-100).</span></span> <span data-ttu-id="bd5a3-188">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="bd5a3-188">Valid values 0 to 100</span></span>|
|<span data-ttu-id="bd5a3-189">energySaverPluggedInThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-189">energySaverPluggedInThresholdPercentage</span></span>|<span data-ttu-id="bd5a3-190">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-190">Int32</span></span>|<span data-ttu-id="bd5a3-191">此设置允许您指定节能程序打开时的电池电量水平。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-191">This setting allows you to specify battery charge level at which Energy Saver is turned on.</span></span> <span data-ttu-id="bd5a3-192">接通电源时，将自动打开（和低于）指定电池电量级别的节能保护程序。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-192">While plugged in, Energy Saver is automatically turned on at (and below) the specified battery charge level.</span></span> <span data-ttu-id="bd5a3-193">有效的输入范围（0-100）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-193">Valid input range (0-100).</span></span> <span data-ttu-id="bd5a3-194">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="bd5a3-194">Valid values 0 to 100</span></span>|
|<span data-ttu-id="bd5a3-195">powerLidCloseActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="bd5a3-195">powerLidCloseActionOnBattery</span></span>|[<span data-ttu-id="bd5a3-196">powerActionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-196">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="bd5a3-197">此设置指定当用户在使用电池时关闭移动电脑上的盖子时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-197">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while on battery.</span></span> <span data-ttu-id="bd5a3-198">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-198">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="bd5a3-199">powerLidCloseActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-199">powerLidCloseActionPluggedIn</span></span>|[<span data-ttu-id="bd5a3-200">powerActionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-200">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="bd5a3-201">此设置指定当用户在插入时关闭移动 PC 上的盖子时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-201">This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while plugged in.</span></span> <span data-ttu-id="bd5a3-202">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-202">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="bd5a3-203">powerButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="bd5a3-203">powerButtonActionOnBattery</span></span>|[<span data-ttu-id="bd5a3-204">powerActionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-204">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="bd5a3-205">此设置指定当用户在使用电池时按下电源按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-205">This setting specifies the action that Windows takes when a user presses the Power button while on battery.</span></span> <span data-ttu-id="bd5a3-206">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-206">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="bd5a3-207">powerButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-207">powerButtonActionPluggedIn</span></span>|[<span data-ttu-id="bd5a3-208">powerActionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-208">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="bd5a3-209">此设置指定当用户在插入时按下电源按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-209">This setting specifies the action that Windows takes when a user presses the Power button while plugged in.</span></span> <span data-ttu-id="bd5a3-210">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-210">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="bd5a3-211">powerSleepButtonActionOnBattery</span><span class="sxs-lookup"><span data-stu-id="bd5a3-211">powerSleepButtonActionOnBattery</span></span>|[<span data-ttu-id="bd5a3-212">powerActionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-212">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="bd5a3-213">此设置指定当用户在使用电池时按 "睡眠" 按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-213">This setting specifies the action that Windows takes when a user presses the Sleep button while on battery.</span></span> <span data-ttu-id="bd5a3-214">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-214">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="bd5a3-215">powerSleepButtonActionPluggedIn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-215">powerSleepButtonActionPluggedIn</span></span>|[<span data-ttu-id="bd5a3-216">powerActionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-216">powerActionType</span></span>](../resources/intune-deviceconfig-poweractiontype.md)|<span data-ttu-id="bd5a3-217">此设置指定当用户在插入时按 "睡眠" 按钮时 Windows 采取的操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-217">This setting specifies the action that Windows takes when a user presses the Sleep button while plugged in.</span></span> <span data-ttu-id="bd5a3-218">可取值为：`notConfigured`、`noAction`、`sleep`、`hibernate`、`shutdown`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-218">Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.</span></span>|
|<span data-ttu-id="bd5a3-219">powerHybridSleepOnBattery</span><span class="sxs-lookup"><span data-stu-id="bd5a3-219">powerHybridSleepOnBattery</span></span>|[<span data-ttu-id="bd5a3-220">启用</span><span class="sxs-lookup"><span data-stu-id="bd5a3-220">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd5a3-221">通过此设置，可以在使用电池时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-221">This setting allows you to turn off hybrid sleep while on battery.</span></span> <span data-ttu-id="bd5a3-222">如果将此设置设置为禁用，则当系统转换为睡眠（待机）时不会生成 hiberfile。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-222">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="bd5a3-223">如果将此设置设置为启用或未配置此策略设置，则用户将控制此设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-223">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="bd5a3-224">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-224">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd5a3-225">powerHybridSleepPluggedIn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-225">powerHybridSleepPluggedIn</span></span>|[<span data-ttu-id="bd5a3-226">启用</span><span class="sxs-lookup"><span data-stu-id="bd5a3-226">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd5a3-227">此设置允许你在接通电源时关闭混合睡眠。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-227">This setting allows you to turn off hybrid sleep while plugged in.</span></span> <span data-ttu-id="bd5a3-228">如果将此设置设置为禁用，则当系统转换为睡眠（待机）时不会生成 hiberfile。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-228">If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By).</span></span> <span data-ttu-id="bd5a3-229">如果将此设置设置为启用或未配置此策略设置，则用户将控制此设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-229">If you set this setting to enable or do not configure this policy setting, users control this setting.</span></span> <span data-ttu-id="bd5a3-230">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-230">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd5a3-231">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="bd5a3-231">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="bd5a3-232">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="bd5a3-232">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="bd5a3-233">应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-233">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="bd5a3-234">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="bd5a3-234">enableAutomaticRedeployment</span></span>|<span data-ttu-id="bd5a3-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-235">Boolean</span></span>|<span data-ttu-id="bd5a3-236">允许具有管理权限的用户在设备锁屏的屏幕上使用 CTRL + Win + R 删除所有用户数据和设置，以便可以自动重新配置设备并将其重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-236">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="bd5a3-237">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="bd5a3-237">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="bd5a3-238">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-238">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="bd5a3-239">控制 Microsoft 帐户登录助手（wlidsvc） NT 服务。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-239">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="bd5a3-240">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-240">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="bd5a3-241">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="bd5a3-241">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="bd5a3-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-242">Boolean</span></span>|<span data-ttu-id="bd5a3-243">允许辅助身份验证设备使用 Windows。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-243">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="bd5a3-244">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-244">authenticationWebSignIn</span></span>|[<span data-ttu-id="bd5a3-245">启用</span><span class="sxs-lookup"><span data-stu-id="bd5a3-245">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd5a3-246">指示是否将启用 Web 凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-246">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="bd5a3-247">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-247">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd5a3-248">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="bd5a3-248">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="bd5a3-249">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-249">String</span></span>|<span data-ttu-id="bd5a3-250">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-250">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="bd5a3-251">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="bd5a3-251">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="bd5a3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-252">Boolean</span></span>|<span data-ttu-id="bd5a3-253">指定是否允许或禁止联邦信息处理标准（FIPS）策略。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-253">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="bd5a3-254">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-254">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="bd5a3-255">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-255">String collection</span></span>|<span data-ttu-id="bd5a3-256">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-256">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="bd5a3-257">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="bd5a3-257">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="bd5a3-258">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-258">String collection</span></span>|<span data-ttu-id="bd5a3-259">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-259">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="bd5a3-260">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="bd5a3-260">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="bd5a3-261">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-261">String</span></span>|<span data-ttu-id="bd5a3-262">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-262">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="bd5a3-263">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="bd5a3-263">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="bd5a3-264">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-264">String</span></span>|<span data-ttu-id="bd5a3-265">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-265">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="bd5a3-266">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="bd5a3-266">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="bd5a3-267">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-267">String</span></span>|<span data-ttu-id="bd5a3-268">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-268">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="bd5a3-269">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bd5a3-269">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="bd5a3-270">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-270">String</span></span>|<span data-ttu-id="bd5a3-271">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-271">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="bd5a3-272">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="bd5a3-272">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="bd5a3-273">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-273">Int32</span></span>|<span data-ttu-id="bd5a3-274">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-274">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="bd5a3-275">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-275">This is a mobile only setting.</span></span> <span data-ttu-id="bd5a3-276">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="bd5a3-276">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="bd5a3-277">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bd5a3-277">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="bd5a3-278">String</span><span class="sxs-lookup"><span data-stu-id="bd5a3-278">String</span></span>|<span data-ttu-id="bd5a3-279">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-279">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="bd5a3-280">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="bd5a3-280">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="bd5a3-281">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-281">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="bd5a3-282">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-282">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="bd5a3-283">选项可供 IT 管理员阻止跨设备同步，但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-283">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="bd5a3-284">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-284">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="bd5a3-285">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="bd5a3-285">messagingBlockSync</span></span>|<span data-ttu-id="bd5a3-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-286">Boolean</span></span>|<span data-ttu-id="bd5a3-287">指示是否在所有位置阻止短信备份和还原和消息传递。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-287">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="bd5a3-288">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="bd5a3-288">messagingBlockMMS</span></span>|<span data-ttu-id="bd5a3-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-289">Boolean</span></span>|<span data-ttu-id="bd5a3-290">指示是否阻止设备上的 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-290">Indicates whether or not to block the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="bd5a3-291">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="bd5a3-291">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="bd5a3-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-292">Boolean</span></span>|<span data-ttu-id="bd5a3-293">指示是否阻止设备上的 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-293">Indicates whether or not to block the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="bd5a3-294">printerNames</span><span class="sxs-lookup"><span data-stu-id="bd5a3-294">printerNames</span></span>|<span data-ttu-id="bd5a3-295">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-295">String collection</span></span>|<span data-ttu-id="bd5a3-296">根据打印机的名称（网络主机名称）自动预配打印机。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-296">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="bd5a3-297">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="bd5a3-297">printerDefaultName</span></span>|<span data-ttu-id="bd5a3-298">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-298">String</span></span>|<span data-ttu-id="bd5a3-299">已安装的打印机的名称（网络主机名称）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-299">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="bd5a3-300">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="bd5a3-300">printerBlockAddition</span></span>|<span data-ttu-id="bd5a3-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-301">Boolean</span></span>|<span data-ttu-id="bd5a3-302">阻止用户安装来自打印机设置的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-302">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="bd5a3-303">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="bd5a3-303">searchBlockDiacritics</span></span>|<span data-ttu-id="bd5a3-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-304">Boolean</span></span>|<span data-ttu-id="bd5a3-305">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-305">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="bd5a3-306">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-306">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="bd5a3-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-307">Boolean</span></span>|<span data-ttu-id="bd5a3-308">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-308">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="bd5a3-309">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="bd5a3-309">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="bd5a3-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-310">Boolean</span></span>|<span data-ttu-id="bd5a3-311">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-311">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="bd5a3-312">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="bd5a3-312">searchEnableRemoteQueries</span></span>|<span data-ttu-id="bd5a3-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-313">Boolean</span></span>|<span data-ttu-id="bd5a3-314">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-314">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="bd5a3-315">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="bd5a3-315">searchDisableUseLocation</span></span>|<span data-ttu-id="bd5a3-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-316">Boolean</span></span>|<span data-ttu-id="bd5a3-317">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-317">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="bd5a3-318">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="bd5a3-318">searchDisableLocation</span></span>|<span data-ttu-id="bd5a3-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-319">Boolean</span></span>|<span data-ttu-id="bd5a3-320">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-320">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="bd5a3-321">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="bd5a3-321">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="bd5a3-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-322">Boolean</span></span>|<span data-ttu-id="bd5a3-323">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-323">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="bd5a3-324">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="bd5a3-324">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="bd5a3-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-325">Boolean</span></span>|<span data-ttu-id="bd5a3-326">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-326">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="bd5a3-327">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="bd5a3-327">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="bd5a3-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-328">Boolean</span></span>|<span data-ttu-id="bd5a3-329">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-329">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="bd5a3-330">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="bd5a3-330">searchBlockWebResults</span></span>|<span data-ttu-id="bd5a3-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-331">Boolean</span></span>|<span data-ttu-id="bd5a3-332">指示是否阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-332">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="bd5a3-333">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="bd5a3-333">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="bd5a3-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-334">Boolean</span></span>|<span data-ttu-id="bd5a3-335">在设备已加入 Azure AD 时，指定是否允许在 OOBE 期间自动设备加密（仅限桌面）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-335">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="bd5a3-336">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-336">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="bd5a3-337">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-337">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="bd5a3-338">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-338">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="bd5a3-339">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-339">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="bd5a3-340">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="bd5a3-340">oneDriveDisableFileSync</span></span>|<span data-ttu-id="bd5a3-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-341">Boolean</span></span>|<span data-ttu-id="bd5a3-342">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-342">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="bd5a3-343">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-343">systemTelemetryProxyServer</span></span>|<span data-ttu-id="bd5a3-344">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-344">String</span></span>|<span data-ttu-id="bd5a3-345">获取或设置代理服务器的完全限定域名（FQDN）或 IP 地址，以转发连接的用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-345">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="bd5a3-346">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="bd5a3-346">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="bd5a3-347">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-347">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="bd5a3-348">指定将哪种类型的遥测数据（无、intranet、internet、两者）发送到 Microsoft 365 Analytics。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-348">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="bd5a3-349">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-349">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="bd5a3-350">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="bd5a3-350">inkWorkspaceAccess</span></span>|[<span data-ttu-id="bd5a3-351">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-351">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="bd5a3-352">控制用户对墨迹工作区的访问权限，从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-352">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="bd5a3-353">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-353">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd5a3-354">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="bd5a3-354">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="bd5a3-355">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-355">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="bd5a3-356">控制用户对墨迹工作区的访问权限，从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-356">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="bd5a3-357">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-357">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="bd5a3-358">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="bd5a3-358">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="bd5a3-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-359">Boolean</span></span>|<span data-ttu-id="bd5a3-360">指定是否在墨迹工作区中显示建议的应用建议。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-360">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="bd5a3-361">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="bd5a3-361">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="bd5a3-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-362">Boolean</span></span>|<span data-ttu-id="bd5a3-363">此属性将在7月2019中弃用，并将替换为属性 SmartScreenAppInstallControl。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-363">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="bd5a3-364">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-364">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="bd5a3-365">smartScreenAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="bd5a3-365">smartScreenAppInstallControl</span></span>|[<span data-ttu-id="bd5a3-366">appInstallControlType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-366">appInstallControlType</span></span>](../resources/intune-deviceconfig-appinstallcontroltype.md)|<span data-ttu-id="bd5a3-367">在 Windows 10 版本1703中添加。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-367">Added in Windows 10, version 1703.</span></span> <span data-ttu-id="bd5a3-368">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-368">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span> <span data-ttu-id="bd5a3-369">可取值为：`notConfigured`、`anywhere`、`storeOnly`、`recommendations`、`preferStore`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-369">Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.</span></span>|
|<span data-ttu-id="bd5a3-370">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="bd5a3-370">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="bd5a3-371">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-371">String</span></span>|<span data-ttu-id="bd5a3-372">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-372">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="bd5a3-373">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="bd5a3-373">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="bd5a3-374">String</span><span class="sxs-lookup"><span data-stu-id="bd5a3-374">String</span></span>|<span data-ttu-id="bd5a3-375">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-375">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="bd5a3-376">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="bd5a3-376">bluetoothAllowedServices</span></span>|<span data-ttu-id="bd5a3-377">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd5a3-377">String collection</span></span>|<span data-ttu-id="bd5a3-378">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-378">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="bd5a3-379">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="bd5a3-379">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="bd5a3-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-380">Boolean</span></span>|<span data-ttu-id="bd5a3-381">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-381">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="bd5a3-382">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="bd5a3-382">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="bd5a3-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-383">Boolean</span></span>|<span data-ttu-id="bd5a3-384">是否阻止用户使用 Swift 对和其他基于邻近的应用场景。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-384">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="bd5a3-385">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-385">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="bd5a3-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-386">Boolean</span></span>|<span data-ttu-id="bd5a3-387">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-387">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="bd5a3-388">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="bd5a3-388">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="bd5a3-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-389">Boolean</span></span>|<span data-ttu-id="bd5a3-390">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-390">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="bd5a3-391">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="bd5a3-391">edgeBlockAutofill</span></span>|<span data-ttu-id="bd5a3-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-392">Boolean</span></span>|<span data-ttu-id="bd5a3-393">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-393">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="bd5a3-394">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-394">edgeBlocked</span></span>|<span data-ttu-id="bd5a3-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-395">Boolean</span></span>|<span data-ttu-id="bd5a3-396">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-396">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="bd5a3-397">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="bd5a3-397">edgeCookiePolicy</span></span>|[<span data-ttu-id="bd5a3-398">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="bd5a3-398">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="bd5a3-399">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-399">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="bd5a3-400">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-400">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="bd5a3-401">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="bd5a3-401">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="bd5a3-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-402">Boolean</span></span>|<span data-ttu-id="bd5a3-403">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-403">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="bd5a3-404">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="bd5a3-404">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="bd5a3-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-405">Boolean</span></span>|<span data-ttu-id="bd5a3-406">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-406">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="bd5a3-407">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-407">edgeBlockExtensions</span></span>|<span data-ttu-id="bd5a3-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-408">Boolean</span></span>|<span data-ttu-id="bd5a3-409">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-409">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="bd5a3-410">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="bd5a3-410">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="bd5a3-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-411">Boolean</span></span>|<span data-ttu-id="bd5a3-412">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-412">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="bd5a3-413">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="bd5a3-413">edgeBlockJavaScript</span></span>|<span data-ttu-id="bd5a3-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-414">Boolean</span></span>|<span data-ttu-id="bd5a3-415">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-415">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="bd5a3-416">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="bd5a3-416">edgeBlockPasswordManager</span></span>|<span data-ttu-id="bd5a3-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-417">Boolean</span></span>|<span data-ttu-id="bd5a3-418">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-418">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="bd5a3-419">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="bd5a3-419">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="bd5a3-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-420">Boolean</span></span>|<span data-ttu-id="bd5a3-421">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-421">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="bd5a3-422">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-422">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="bd5a3-423">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="bd5a3-423">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="bd5a3-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-424">Boolean</span></span>|<span data-ttu-id="bd5a3-425">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-425">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="bd5a3-426">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-426">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="bd5a3-427">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="bd5a3-427">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="bd5a3-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-428">Boolean</span></span>|<span data-ttu-id="bd5a3-429">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-429">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="bd5a3-430">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="bd5a3-430">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="bd5a3-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-431">Boolean</span></span>|<span data-ttu-id="bd5a3-432">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-432">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="bd5a3-433">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-433">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="bd5a3-434">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-434">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="bd5a3-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-435">Boolean</span></span>|<span data-ttu-id="bd5a3-436">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-436">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="bd5a3-437">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-437">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="bd5a3-438">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-438">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="bd5a3-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-439">Boolean</span></span>|<span data-ttu-id="bd5a3-440">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-440">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="bd5a3-441">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-441">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="bd5a3-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-442">Boolean</span></span>|<span data-ttu-id="bd5a3-443">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-443">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="bd5a3-444">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-444">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="bd5a3-445">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="bd5a3-445">edgeFavoritesListLocation</span></span>|<span data-ttu-id="bd5a3-446">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-446">String</span></span>|<span data-ttu-id="bd5a3-447">要设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-447">The location of the favorites list to provision.</span></span> <span data-ttu-id="bd5a3-448">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-448">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="bd5a3-449">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="bd5a3-449">edgeBlockEditFavorites</span></span>|<span data-ttu-id="bd5a3-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-450">Boolean</span></span>|<span data-ttu-id="bd5a3-451">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-451">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="bd5a3-452">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="bd5a3-452">edgeNewTabPageURL</span></span>|<span data-ttu-id="bd5a3-453">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-453">String</span></span>|<span data-ttu-id="bd5a3-454">指定在创建新选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-454">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="bd5a3-455">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5a3-455">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="bd5a3-456">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5a3-456">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="bd5a3-457">使 Home 按钮可以隐藏、加载默认起始页、加载新的选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="bd5a3-457">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="bd5a3-458">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="bd5a3-458">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="bd5a3-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-459">Boolean</span></span>|<span data-ttu-id="bd5a3-460">启用 "主页" 按钮配置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-460">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="bd5a3-461">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="bd5a3-461">edgeOpensWith</span></span>|[<span data-ttu-id="bd5a3-462">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-462">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="bd5a3-463">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-463">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="bd5a3-464">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-464">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="bd5a3-465">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-465">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="bd5a3-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-466">Boolean</span></span>|<span data-ttu-id="bd5a3-467">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-467">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="bd5a3-468">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="bd5a3-468">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="bd5a3-469">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-469">String collection</span></span>|<span data-ttu-id="bd5a3-470">指定所需的浏览器扩展的程序包系列名称列表，用户无法关闭这些扩展。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-470">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="bd5a3-471">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-471">edgeBlockPrinting</span></span>|<span data-ttu-id="bd5a3-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-472">Boolean</span></span>|<span data-ttu-id="bd5a3-473">将 Edge 配置为允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-473">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="bd5a3-474">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="bd5a3-474">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="bd5a3-475">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-475">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-476">获取或设置一个值，该值指定是否将收藏夹栏设置为始终在任何页面上都可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-476">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="bd5a3-477">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-477">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-478">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="bd5a3-478">edgeBlockSavingHistory</span></span>|<span data-ttu-id="bd5a3-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-479">Boolean</span></span>|<span data-ttu-id="bd5a3-480">将 Edge 配置为允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-480">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="bd5a3-481">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-481">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="bd5a3-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-482">Boolean</span></span>|<span data-ttu-id="bd5a3-483">允许或阻止边缘进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-483">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="bd5a3-484">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-484">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="bd5a3-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-485">Boolean</span></span>|<span data-ttu-id="bd5a3-486">将配置为在 Edge 中加载空白页面，而不是默认的新选项卡页面，并防止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-486">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="bd5a3-487">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="bd5a3-487">edgeBlockTabPreloading</span></span>|<span data-ttu-id="bd5a3-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-488">Boolean</span></span>|<span data-ttu-id="bd5a3-489">配置边缘是否在 Windows 启动时预加载新的选项卡页。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-489">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="bd5a3-490">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="bd5a3-490">edgeBlockPrelaunch</span></span>|<span data-ttu-id="bd5a3-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-491">Boolean</span></span>|<span data-ttu-id="bd5a3-492">确定 Microsoft Edge 在 Windows 启动时是否为 prelaunched。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-492">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="bd5a3-493">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="bd5a3-493">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="bd5a3-494">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-494">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="bd5a3-495">控制边缘在切换到 Internet Explorer 之前显示的消息。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-495">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="bd5a3-496">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-496">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="bd5a3-497">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="bd5a3-497">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="bd5a3-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-498">Boolean</span></span>|<span data-ttu-id="bd5a3-499">允许或阻止用户覆盖证书错误。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-499">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="bd5a3-500">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="bd5a3-500">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="bd5a3-501">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-501">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="bd5a3-502">根据配置展台模式，控制 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-502">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="bd5a3-503">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-503">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="bd5a3-504">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="bd5a3-504">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="bd5a3-505">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-505">Int32</span></span>|<span data-ttu-id="bd5a3-506">指定在 Microsoft Edge 展台重置前的上次用户活动的时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-506">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="bd5a3-507">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-507">Valid values are 0-1440.</span></span> <span data-ttu-id="bd5a3-508">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-508">The default is 5.</span></span> <span data-ttu-id="bd5a3-509">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-509">0 indicates no reset.</span></span> <span data-ttu-id="bd5a3-510">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="bd5a3-510">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="bd5a3-511">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="bd5a3-511">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="bd5a3-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-512">Boolean</span></span>|<span data-ttu-id="bd5a3-513">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-513">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="bd5a3-514">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-514">cellularBlockVpn</span></span>|<span data-ttu-id="bd5a3-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-515">Boolean</span></span>|<span data-ttu-id="bd5a3-516">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-516">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="bd5a3-517">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="bd5a3-517">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="bd5a3-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-518">Boolean</span></span>|<span data-ttu-id="bd5a3-519">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-519">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="bd5a3-520">cellularData</span><span class="sxs-lookup"><span data-stu-id="bd5a3-520">cellularData</span></span>|[<span data-ttu-id="bd5a3-521">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-521">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="bd5a3-522">是否允许设备上的手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-522">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="bd5a3-523">如果未配置，则允许手机网络数据通道，用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-523">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="bd5a3-524">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-524">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="bd5a3-525">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="bd5a3-525">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="bd5a3-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-526">Boolean</span></span>|<span data-ttu-id="bd5a3-527">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-527">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="bd5a3-528">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="bd5a3-528">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="bd5a3-529">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-529">Int32</span></span>|<span data-ttu-id="bd5a3-530">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-530">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="bd5a3-531">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="bd5a3-531">Valid values 0 to 90</span></span>|
|<span data-ttu-id="bd5a3-532">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-532">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="bd5a3-533">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-533">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="bd5a3-534">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-534">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="bd5a3-535">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="bd5a3-535">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="bd5a3-536">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="bd5a3-536">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="bd5a3-537">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-537">Defender day of the week for the system scan.</span></span> <span data-ttu-id="bd5a3-538">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-538">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="bd5a3-539">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="bd5a3-539">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="bd5a3-540">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-540">String collection</span></span>|<span data-ttu-id="bd5a3-541">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-541">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="bd5a3-542">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="bd5a3-542">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="bd5a3-543">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-543">String collection</span></span>|<span data-ttu-id="bd5a3-544">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-544">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="bd5a3-545">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="bd5a3-545">defenderScanMaxCpu</span></span>|<span data-ttu-id="bd5a3-546">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-546">Int32</span></span>|<span data-ttu-id="bd5a3-547">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-547">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="bd5a3-548">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="bd5a3-548">Valid values 0 to 100</span></span>|
|<span data-ttu-id="bd5a3-549">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="bd5a3-549">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="bd5a3-550">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="bd5a3-550">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="bd5a3-551">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-551">Value for monitoring file activity.</span></span> <span data-ttu-id="bd5a3-552">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-552">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="bd5a3-553">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="bd5a3-553">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="bd5a3-554">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="bd5a3-554">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="bd5a3-555">获取或设置要对可能有害的应用程序（PUA）执行的 Defender 操作，其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时，Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-555">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="bd5a3-556">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-556">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="bd5a3-557">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-557">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="bd5a3-558">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-558">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="bd5a3-559">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-559">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bd5a3-560">获取或设置要对可能有害的应用程序（PUA）执行的 Defender 操作，其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时，Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-560">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="bd5a3-561">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-561">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="bd5a3-562">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-562">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bd5a3-563">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="bd5a3-563">defenderProcessesToExclude</span></span>|<span data-ttu-id="bd5a3-564">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd5a3-564">String collection</span></span>|<span data-ttu-id="bd5a3-565">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-565">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="bd5a3-566">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="bd5a3-566">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="bd5a3-567">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="bd5a3-567">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="bd5a3-568">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-568">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="bd5a3-569">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-569">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="bd5a3-570">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="bd5a3-570">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="bd5a3-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-571">Boolean</span></span>|<span data-ttu-id="bd5a3-572">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-572">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="bd5a3-573">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-573">defenderRequireCloudProtection</span></span>|<span data-ttu-id="bd5a3-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-574">Boolean</span></span>|<span data-ttu-id="bd5a3-575">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-575">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="bd5a3-576">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="bd5a3-576">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="bd5a3-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-577">Boolean</span></span>|<span data-ttu-id="bd5a3-578">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-578">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="bd5a3-579">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="bd5a3-579">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="bd5a3-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-580">Boolean</span></span>|<span data-ttu-id="bd5a3-581">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-581">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="bd5a3-582">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="bd5a3-582">defenderScanArchiveFiles</span></span>|<span data-ttu-id="bd5a3-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-583">Boolean</span></span>|<span data-ttu-id="bd5a3-584">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-584">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="bd5a3-585">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="bd5a3-585">defenderScanDownloads</span></span>|<span data-ttu-id="bd5a3-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-586">Boolean</span></span>|<span data-ttu-id="bd5a3-587">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-587">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="bd5a3-588">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="bd5a3-588">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="bd5a3-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-589">Boolean</span></span>|<span data-ttu-id="bd5a3-590">启用后，在计划扫描期间将使用较低的 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-590">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="bd5a3-591">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="bd5a3-591">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="bd5a3-592">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-592">Boolean</span></span>|<span data-ttu-id="bd5a3-593">当被阻止时，将关闭计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-593">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="bd5a3-594">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="bd5a3-594">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="bd5a3-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-595">Boolean</span></span>|<span data-ttu-id="bd5a3-596">当被阻止时，计划的完全扫描的追赶扫描将被禁用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-596">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="bd5a3-597">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="bd5a3-597">defenderScanNetworkFiles</span></span>|<span data-ttu-id="bd5a3-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-598">Boolean</span></span>|<span data-ttu-id="bd5a3-599">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-599">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="bd5a3-600">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="bd5a3-600">defenderScanIncomingMail</span></span>|<span data-ttu-id="bd5a3-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-601">Boolean</span></span>|<span data-ttu-id="bd5a3-602">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-602">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="bd5a3-603">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="bd5a3-603">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="bd5a3-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-604">Boolean</span></span>|<span data-ttu-id="bd5a3-605">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-605">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="bd5a3-606">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="bd5a3-606">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="bd5a3-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-607">Boolean</span></span>|<span data-ttu-id="bd5a3-608">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-608">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="bd5a3-609">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-609">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="bd5a3-610">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-610">Boolean</span></span>|<span data-ttu-id="bd5a3-611">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-611">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="bd5a3-612">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="bd5a3-612">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="bd5a3-613">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-613">Int32</span></span>|<span data-ttu-id="bd5a3-614">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-614">The signature update interval in hours.</span></span> <span data-ttu-id="bd5a3-615">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-615">Specify 0 not to check.</span></span> <span data-ttu-id="bd5a3-616">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="bd5a3-616">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bd5a3-617">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-617">defenderScanType</span></span>|[<span data-ttu-id="bd5a3-618">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-618">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="bd5a3-619">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-619">The defender system scan type.</span></span> <span data-ttu-id="bd5a3-620">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-620">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="bd5a3-621">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="bd5a3-621">defenderScheduledScanTime</span></span>|<span data-ttu-id="bd5a3-622">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bd5a3-622">TimeOfDay</span></span>|<span data-ttu-id="bd5a3-623">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-623">The defender time for the system scan.</span></span>|
|<span data-ttu-id="bd5a3-624">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="bd5a3-624">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="bd5a3-625">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bd5a3-625">TimeOfDay</span></span>|<span data-ttu-id="bd5a3-626">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-626">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="bd5a3-627">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="bd5a3-627">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="bd5a3-628">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-628">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="bd5a3-629">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-629">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="bd5a3-630">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-630">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="bd5a3-631">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="bd5a3-631">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="bd5a3-632">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-632">Int32</span></span>|<span data-ttu-id="bd5a3-633">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-633">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="bd5a3-634">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="bd5a3-634">Valid values 0 to 50</span></span>|
|<span data-ttu-id="bd5a3-635">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="bd5a3-635">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="bd5a3-636">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-636">Int32</span></span>|<span data-ttu-id="bd5a3-637">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-637">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="bd5a3-638">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="bd5a3-638">Valid values 0 to 50</span></span>|
|<span data-ttu-id="bd5a3-639">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-639">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="bd5a3-640">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-640">Boolean</span></span>|<span data-ttu-id="bd5a3-641">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-641">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="bd5a3-642">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-642">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="bd5a3-643">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-643">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="bd5a3-644">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-644">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="bd5a3-645">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-645">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="bd5a3-646">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5a3-646">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="bd5a3-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-647">Boolean</span></span>|<span data-ttu-id="bd5a3-648">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-648">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="bd5a3-649">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-649">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="bd5a3-650">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="bd5a3-650">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="bd5a3-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-651">Boolean</span></span>|<span data-ttu-id="bd5a3-652">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-652">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="bd5a3-653">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="bd5a3-653">lockScreenBlockCortana</span></span>|<span data-ttu-id="bd5a3-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-654">Boolean</span></span>|<span data-ttu-id="bd5a3-655">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-655">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="bd5a3-656">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="bd5a3-656">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="bd5a3-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-657">Boolean</span></span>|<span data-ttu-id="bd5a3-658">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-658">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="bd5a3-659">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="bd5a3-659">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="bd5a3-660">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-660">Int32</span></span>|<span data-ttu-id="bd5a3-661">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-661">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="bd5a3-662">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-662">Supported values are 11-1800.</span></span> <span data-ttu-id="bd5a3-663">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="bd5a3-663">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="bd5a3-664">lockScreenActivateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="bd5a3-664">lockScreenActivateAppsWithVoice</span></span>|[<span data-ttu-id="bd5a3-665">启用</span><span class="sxs-lookup"><span data-stu-id="bd5a3-665">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd5a3-666">此策略设置指定在系统处于锁定状态时，Windows 应用是否可以通过语音激活。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-666">This policy setting specifies whether Windows apps can be activated by voice while the system is locked.</span></span> <span data-ttu-id="bd5a3-667">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-667">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd5a3-668">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bd5a3-668">passwordBlockSimple</span></span>|<span data-ttu-id="bd5a3-669">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-669">Boolean</span></span>|<span data-ttu-id="bd5a3-670">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-670">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="bd5a3-671">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-671">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="bd5a3-672">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bd5a3-672">passwordExpirationDays</span></span>|<span data-ttu-id="bd5a3-673">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-673">Int32</span></span>|<span data-ttu-id="bd5a3-674">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-674">The password expiration in days.</span></span> <span data-ttu-id="bd5a3-675">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="bd5a3-675">Valid values 0 to 730</span></span>|
|<span data-ttu-id="bd5a3-676">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bd5a3-676">passwordMinimumLength</span></span>|<span data-ttu-id="bd5a3-677">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-677">Int32</span></span>|<span data-ttu-id="bd5a3-678">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-678">The minimum password length.</span></span> <span data-ttu-id="bd5a3-679">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="bd5a3-679">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bd5a3-680">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bd5a3-680">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bd5a3-681">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-681">Int32</span></span>|<span data-ttu-id="bd5a3-682">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-682">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bd5a3-683">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bd5a3-683">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bd5a3-684">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-684">Int32</span></span>|<span data-ttu-id="bd5a3-685">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-685">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bd5a3-686">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bd5a3-686">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bd5a3-687">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-687">Int32</span></span>|<span data-ttu-id="bd5a3-688">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-688">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="bd5a3-689">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="bd5a3-689">Valid values 0 to 50</span></span>|
|<span data-ttu-id="bd5a3-690">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bd5a3-690">passwordRequired</span></span>|<span data-ttu-id="bd5a3-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-691">Boolean</span></span>|<span data-ttu-id="bd5a3-692">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-692">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="bd5a3-693">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="bd5a3-693">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="bd5a3-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-694">Boolean</span></span>|<span data-ttu-id="bd5a3-695">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-695">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="bd5a3-696">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-696">passwordRequiredType</span></span>|[<span data-ttu-id="bd5a3-697">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-697">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bd5a3-698">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-698">The required password type.</span></span> <span data-ttu-id="bd5a3-699">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-699">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bd5a3-700">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bd5a3-700">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bd5a3-701">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-701">Int32</span></span>|<span data-ttu-id="bd5a3-702">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-702">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="bd5a3-703">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="bd5a3-703">Valid values 0 to 999</span></span>|
|<span data-ttu-id="bd5a3-704">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="bd5a3-704">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="bd5a3-705">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-705">Int32</span></span>|<span data-ttu-id="bd5a3-706">此安全设置确定用户可以更改密码之前必须使用该密码的时间（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-706">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="bd5a3-707">有效值为0至998</span><span class="sxs-lookup"><span data-stu-id="bd5a3-707">Valid values 0 to 998</span></span>|
|<span data-ttu-id="bd5a3-708">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="bd5a3-708">privacyAdvertisingId</span></span>|[<span data-ttu-id="bd5a3-709">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-709">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="bd5a3-710">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-710">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="bd5a3-711">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-711">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="bd5a3-712">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-712">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="bd5a3-713">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="bd5a3-713">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="bd5a3-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-714">Boolean</span></span>|<span data-ttu-id="bd5a3-715">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-715">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="bd5a3-716">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="bd5a3-716">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="bd5a3-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-717">Boolean</span></span>|<span data-ttu-id="bd5a3-718">此策略可防止在用户登录时为新的和已升级的用户启动隐私体验。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-718">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="bd5a3-719">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="bd5a3-719">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="bd5a3-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-720">Boolean</span></span>|<span data-ttu-id="bd5a3-721">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-721">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="bd5a3-722">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="bd5a3-722">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="bd5a3-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-723">Boolean</span></span>|<span data-ttu-id="bd5a3-724">阻止共享体验和发现任务切换器等中的最近使用的资源。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-724">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="bd5a3-725">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="bd5a3-725">privacyBlockActivityFeed</span></span>|<span data-ttu-id="bd5a3-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-726">Boolean</span></span>|<span data-ttu-id="bd5a3-727">阻止 Cortana、听写或存储应用程序的基于云的语音服务的使用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-727">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="bd5a3-728">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="bd5a3-728">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="bd5a3-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-729">Boolean</span></span>|<span data-ttu-id="bd5a3-730">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-730">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="bd5a3-731">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="bd5a3-731">startMenuAppListVisibility</span></span>|[<span data-ttu-id="bd5a3-732">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-732">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="bd5a3-733">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-733">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="bd5a3-734">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-734">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="bd5a3-735">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="bd5a3-735">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="bd5a3-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-736">Boolean</span></span>|<span data-ttu-id="bd5a3-737">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-737">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-738">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="bd5a3-738">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="bd5a3-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-739">Boolean</span></span>|<span data-ttu-id="bd5a3-740">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-740">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="bd5a3-741">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="bd5a3-741">startMenuHideHibernate</span></span>|<span data-ttu-id="bd5a3-742">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-742">Boolean</span></span>|<span data-ttu-id="bd5a3-743">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-743">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-744">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="bd5a3-744">startMenuHideLock</span></span>|<span data-ttu-id="bd5a3-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-745">Boolean</span></span>|<span data-ttu-id="bd5a3-746">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-746">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-747">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="bd5a3-747">startMenuHidePowerButton</span></span>|<span data-ttu-id="bd5a3-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-748">Boolean</span></span>|<span data-ttu-id="bd5a3-749">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-749">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-750">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="bd5a3-750">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="bd5a3-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-751">Boolean</span></span>|<span data-ttu-id="bd5a3-752">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-752">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="bd5a3-753">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="bd5a3-753">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="bd5a3-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-754">Boolean</span></span>|<span data-ttu-id="bd5a3-755">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-755">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="bd5a3-756">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-756">startMenuHideRestartOptions</span></span>|<span data-ttu-id="bd5a3-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-757">Boolean</span></span>|<span data-ttu-id="bd5a3-758">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-758">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-759">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="bd5a3-759">startMenuHideShutDown</span></span>|<span data-ttu-id="bd5a3-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-760">Boolean</span></span>|<span data-ttu-id="bd5a3-761">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-761">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-762">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="bd5a3-762">startMenuHideSignOut</span></span>|<span data-ttu-id="bd5a3-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-763">Boolean</span></span>|<span data-ttu-id="bd5a3-764">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-764">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-765">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="bd5a3-765">startMenuHideSleep</span></span>|<span data-ttu-id="bd5a3-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-766">Boolean</span></span>|<span data-ttu-id="bd5a3-767">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-767">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-768">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="bd5a3-768">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="bd5a3-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-769">Boolean</span></span>|<span data-ttu-id="bd5a3-770">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-770">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-771">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="bd5a3-771">startMenuHideUserTile</span></span>|<span data-ttu-id="bd5a3-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-772">Boolean</span></span>|<span data-ttu-id="bd5a3-773">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-773">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="bd5a3-774">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="bd5a3-774">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="bd5a3-775">Binary</span><span class="sxs-lookup"><span data-stu-id="bd5a3-775">Binary</span></span>|<span data-ttu-id="bd5a3-776">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-776">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="bd5a3-777">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-777">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="bd5a3-778">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-778">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="bd5a3-779">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-779">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="bd5a3-780">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-780">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="bd5a3-781">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="bd5a3-781">startMenuLayoutXml</span></span>|<span data-ttu-id="bd5a3-782">Binary</span><span class="sxs-lookup"><span data-stu-id="bd5a3-782">Binary</span></span>|<span data-ttu-id="bd5a3-783">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-783">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="bd5a3-784">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-784">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="bd5a3-785">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-785">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="bd5a3-786">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="bd5a3-786">startMenuMode</span></span>|[<span data-ttu-id="bd5a3-787">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-787">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="bd5a3-788">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-788">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="bd5a3-789">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-789">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="bd5a3-790">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="bd5a3-790">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="bd5a3-791">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-791">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-792">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-792">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-793">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-793">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-794">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="bd5a3-794">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="bd5a3-795">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-795">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-796">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-796">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-797">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-797">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-798">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-798">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="bd5a3-799">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-799">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-800">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-800">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-801">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-801">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-802">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="bd5a3-802">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="bd5a3-803">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-803">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-804">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-804">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-805">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-805">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-806">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="bd5a3-806">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="bd5a3-807">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-807">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-808">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-808">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-809">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-809">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-810">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="bd5a3-810">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="bd5a3-811">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-811">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-812">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-812">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-813">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-813">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-814">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="bd5a3-814">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="bd5a3-815">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-815">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-816">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-816">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-817">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-817">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-818">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="bd5a3-818">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="bd5a3-819">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-819">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-820">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-820">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-821">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-821">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-822">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="bd5a3-822">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="bd5a3-823">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-823">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-824">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-824">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-825">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-825">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-826">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="bd5a3-826">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="bd5a3-827">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-827">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="bd5a3-828">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-828">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="bd5a3-829">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-829">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="bd5a3-830">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="bd5a3-830">settingsBlockSettingsApp</span></span>|<span data-ttu-id="bd5a3-831">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-831">Boolean</span></span>|<span data-ttu-id="bd5a3-832">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-832">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="bd5a3-833">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-833">settingsBlockSystemPage</span></span>|<span data-ttu-id="bd5a3-834">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-834">Boolean</span></span>|<span data-ttu-id="bd5a3-835">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-835">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-836">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-836">settingsBlockDevicesPage</span></span>|<span data-ttu-id="bd5a3-837">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-837">Boolean</span></span>|<span data-ttu-id="bd5a3-838">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-838">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-839">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-839">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="bd5a3-840">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-840">Boolean</span></span>|<span data-ttu-id="bd5a3-841">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-841">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-842">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-842">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="bd5a3-843">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-843">Boolean</span></span>|<span data-ttu-id="bd5a3-844">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-844">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-845">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-845">settingsBlockAccountsPage</span></span>|<span data-ttu-id="bd5a3-846">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-846">Boolean</span></span>|<span data-ttu-id="bd5a3-847">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-847">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-848">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-848">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="bd5a3-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-849">Boolean</span></span>|<span data-ttu-id="bd5a3-850">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-850">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-851">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-851">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="bd5a3-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-852">Boolean</span></span>|<span data-ttu-id="bd5a3-853">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-853">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-854">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-854">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="bd5a3-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-855">Boolean</span></span>|<span data-ttu-id="bd5a3-856">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-856">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-857">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-857">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="bd5a3-858">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-858">Boolean</span></span>|<span data-ttu-id="bd5a3-859">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-859">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-860">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-860">settingsBlockAppsPage</span></span>|<span data-ttu-id="bd5a3-861">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-861">Boolean</span></span>|<span data-ttu-id="bd5a3-862">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-862">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-863">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-863">settingsBlockGamingPage</span></span>|<span data-ttu-id="bd5a3-864">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-864">Boolean</span></span>|<span data-ttu-id="bd5a3-865">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-865">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="bd5a3-866">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="bd5a3-866">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="bd5a3-867">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-867">Boolean</span></span>|<span data-ttu-id="bd5a3-868">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-868">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="bd5a3-869">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-869">windowsSpotlightBlocked</span></span>|<span data-ttu-id="bd5a3-870">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-870">Boolean</span></span>|<span data-ttu-id="bd5a3-871">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="bd5a3-871">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="bd5a3-872">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="bd5a3-872">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="bd5a3-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-873">Boolean</span></span>|<span data-ttu-id="bd5a3-874">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="bd5a3-874">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="bd5a3-875">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="bd5a3-875">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="bd5a3-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-876">Boolean</span></span>|<span data-ttu-id="bd5a3-877">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-877">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="bd5a3-878">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="bd5a3-878">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="bd5a3-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-879">Boolean</span></span>|<span data-ttu-id="bd5a3-880">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="bd5a3-880">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="bd5a3-881">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="bd5a3-881">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="bd5a3-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-882">Boolean</span></span>|<span data-ttu-id="bd5a3-883">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="bd5a3-883">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="bd5a3-884">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="bd5a3-884">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="bd5a3-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-885">Boolean</span></span>|<span data-ttu-id="bd5a3-886">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-886">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="bd5a3-887">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="bd5a3-887">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="bd5a3-888">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="bd5a3-888">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="bd5a3-889">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-889">Specifies the type of Spotlight.</span></span> <span data-ttu-id="bd5a3-890">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-890">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="bd5a3-891">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="bd5a3-891">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="bd5a3-892">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-892">Boolean</span></span>|<span data-ttu-id="bd5a3-893">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-893">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="bd5a3-894">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-894">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="bd5a3-895">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="bd5a3-895">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="bd5a3-896">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-896">Boolean</span></span>|<span data-ttu-id="bd5a3-897">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-897">Disable automatic detection of settings.</span></span> <span data-ttu-id="bd5a3-898">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-898">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="bd5a3-899">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="bd5a3-899">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="bd5a3-900">String</span><span class="sxs-lookup"><span data-stu-id="bd5a3-900">String</span></span>|<span data-ttu-id="bd5a3-901">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-901">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="bd5a3-902">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-902">networkProxyServer</span></span>|[<span data-ttu-id="bd5a3-903">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-903">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="bd5a3-904">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-904">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="bd5a3-905">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="bd5a3-905">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="bd5a3-906">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-906">Boolean</span></span>|<span data-ttu-id="bd5a3-907">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-907">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="bd5a3-908">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-908">antiTheftModeBlocked</span></span>|<span data-ttu-id="bd5a3-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-909">Boolean</span></span>|<span data-ttu-id="bd5a3-910">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-910">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="bd5a3-911">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-911">bluetoothBlocked</span></span>|<span data-ttu-id="bd5a3-912">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-912">Boolean</span></span>|<span data-ttu-id="bd5a3-913">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-913">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="bd5a3-914">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-914">cameraBlocked</span></span>|<span data-ttu-id="bd5a3-915">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-915">Boolean</span></span>|<span data-ttu-id="bd5a3-916">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-916">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="bd5a3-917">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-917">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="bd5a3-918">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-918">Boolean</span></span>|<span data-ttu-id="bd5a3-919">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-919">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="bd5a3-920">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="bd5a3-920">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="bd5a3-921">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-921">Boolean</span></span>|<span data-ttu-id="bd5a3-922">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-922">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="bd5a3-923">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-923">copyPasteBlocked</span></span>|<span data-ttu-id="bd5a3-924">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-924">Boolean</span></span>|<span data-ttu-id="bd5a3-925">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-925">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="bd5a3-926">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-926">cortanaBlocked</span></span>|<span data-ttu-id="bd5a3-927">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-927">Boolean</span></span>|<span data-ttu-id="bd5a3-928">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-928">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="bd5a3-929">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="bd5a3-929">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="bd5a3-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-930">Boolean</span></span>|<span data-ttu-id="bd5a3-931">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-931">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="bd5a3-932">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="bd5a3-932">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="bd5a3-933">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-933">Boolean</span></span>|<span data-ttu-id="bd5a3-934">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-934">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="bd5a3-935">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="bd5a3-935">safeSearchFilter</span></span>|[<span data-ttu-id="bd5a3-936">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="bd5a3-936">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="bd5a3-937">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-937">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="bd5a3-938">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-938">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="bd5a3-939">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="bd5a3-939">edgeBlockPopups</span></span>|<span data-ttu-id="bd5a3-940">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-940">Boolean</span></span>|<span data-ttu-id="bd5a3-941">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-941">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="bd5a3-942">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="bd5a3-942">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="bd5a3-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-943">Boolean</span></span>|<span data-ttu-id="bd5a3-944">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-944">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="bd5a3-945">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="bd5a3-945">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="bd5a3-946">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-946">Boolean</span></span>|<span data-ttu-id="bd5a3-947">指示是否阻止用户添加新的搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-947">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="bd5a3-948">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-948">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="bd5a3-949">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-949">Boolean</span></span>|<span data-ttu-id="bd5a3-950">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-950">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="bd5a3-951">注意：此属性的名称是误导性的;属性已过时，请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-951">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="bd5a3-952">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="bd5a3-952">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="bd5a3-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-953">Boolean</span></span>|<span data-ttu-id="bd5a3-954">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-954">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="bd5a3-955">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="bd5a3-955">edgeRequireSmartScreen</span></span>|<span data-ttu-id="bd5a3-956">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-956">Boolean</span></span>|<span data-ttu-id="bd5a3-957">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-957">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="bd5a3-958">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="bd5a3-958">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="bd5a3-959">字符串</span><span class="sxs-lookup"><span data-stu-id="bd5a3-959">String</span></span>|<span data-ttu-id="bd5a3-960">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-960">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="bd5a3-961">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-961">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="bd5a3-962">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="bd5a3-962">edgeFirstRunUrl</span></span>|<span data-ttu-id="bd5a3-963">String</span><span class="sxs-lookup"><span data-stu-id="bd5a3-963">String</span></span>|<span data-ttu-id="bd5a3-964">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-964">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="bd5a3-965">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="bd5a3-965">edgeSearchEngine</span></span>|[<span data-ttu-id="bd5a3-966">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="bd5a3-966">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="bd5a3-967">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-967">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="bd5a3-968">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-968">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="bd5a3-969">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="bd5a3-969">edgeHomepageUrls</span></span>|<span data-ttu-id="bd5a3-970">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd5a3-970">String collection</span></span>|<span data-ttu-id="bd5a3-971">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-971">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="bd5a3-972">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="bd5a3-972">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="bd5a3-973">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-973">Boolean</span></span>|<span data-ttu-id="bd5a3-974">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-974">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="bd5a3-975">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="bd5a3-975">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="bd5a3-976">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-976">Boolean</span></span>|<span data-ttu-id="bd5a3-977">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-977">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="bd5a3-978">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="bd5a3-978">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="bd5a3-979">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-979">Boolean</span></span>|<span data-ttu-id="bd5a3-980">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="bd5a3-980">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="bd5a3-981">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="bd5a3-981">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="bd5a3-982">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-982">Boolean</span></span>|<span data-ttu-id="bd5a3-983">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="bd5a3-983">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="bd5a3-984">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-984">internetSharingBlocked</span></span>|<span data-ttu-id="bd5a3-985">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-985">Boolean</span></span>|<span data-ttu-id="bd5a3-986">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-986">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="bd5a3-987">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-987">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="bd5a3-988">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-988">Boolean</span></span>|<span data-ttu-id="bd5a3-989">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-989">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="bd5a3-990">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-990">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="bd5a3-991">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-991">Boolean</span></span>|<span data-ttu-id="bd5a3-992">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-992">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="bd5a3-993">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="bd5a3-993">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="bd5a3-994">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-994">Boolean</span></span>|<span data-ttu-id="bd5a3-995">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-995">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="bd5a3-996">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="bd5a3-996">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="bd5a3-997">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-997">Boolean</span></span>|<span data-ttu-id="bd5a3-998">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-998">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="bd5a3-999">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="bd5a3-999">settingsBlockChangeRegion</span></span>|<span data-ttu-id="bd5a3-1000">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1000">Boolean</span></span>|<span data-ttu-id="bd5a3-1001">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1001">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="bd5a3-1002">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1002">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="bd5a3-1003">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1003">Boolean</span></span>|<span data-ttu-id="bd5a3-1004">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1004">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="bd5a3-1005">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1005">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="bd5a3-1006">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1006">Boolean</span></span>|<span data-ttu-id="bd5a3-1007">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1007">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="bd5a3-1008">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1008">locationServicesBlocked</span></span>|<span data-ttu-id="bd5a3-1009">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1009">Boolean</span></span>|<span data-ttu-id="bd5a3-1010">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1010">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="bd5a3-1011">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1011">microsoftAccountBlocked</span></span>|<span data-ttu-id="bd5a3-1012">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1012">Boolean</span></span>|<span data-ttu-id="bd5a3-1013">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1013">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="bd5a3-1014">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1014">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="bd5a3-1015">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1015">Boolean</span></span>|<span data-ttu-id="bd5a3-1016">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1016">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="bd5a3-1017">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1017">nfcBlocked</span></span>|<span data-ttu-id="bd5a3-1018">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1018">Boolean</span></span>|<span data-ttu-id="bd5a3-1019">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1019">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="bd5a3-1020">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1020">resetProtectionModeBlocked</span></span>|<span data-ttu-id="bd5a3-1021">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1021">Boolean</span></span>|<span data-ttu-id="bd5a3-1022">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1022">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="bd5a3-1023">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1023">screenCaptureBlocked</span></span>|<span data-ttu-id="bd5a3-1024">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1024">Boolean</span></span>|<span data-ttu-id="bd5a3-1025">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1025">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="bd5a3-1026">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1026">storageBlockRemovableStorage</span></span>|<span data-ttu-id="bd5a3-1027">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1027">Boolean</span></span>|<span data-ttu-id="bd5a3-1028">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1028">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="bd5a3-1029">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1029">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="bd5a3-1030">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1030">Boolean</span></span>|<span data-ttu-id="bd5a3-1031">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1031">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="bd5a3-1032">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1032">usbBlocked</span></span>|<span data-ttu-id="bd5a3-1033">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1033">Boolean</span></span>|<span data-ttu-id="bd5a3-1034">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1034">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="bd5a3-1035">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1035">voiceRecordingBlocked</span></span>|<span data-ttu-id="bd5a3-1036">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1036">Boolean</span></span>|<span data-ttu-id="bd5a3-1037">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1037">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="bd5a3-1038">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1038">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="bd5a3-1039">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1039">Boolean</span></span>|<span data-ttu-id="bd5a3-1040">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1040">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="bd5a3-1041">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1041">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="bd5a3-1042">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1042">wiFiBlocked</span></span>|<span data-ttu-id="bd5a3-1043">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1043">Boolean</span></span>|<span data-ttu-id="bd5a3-1044">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1044">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="bd5a3-1045">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1045">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="bd5a3-1046">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1046">Boolean</span></span>|<span data-ttu-id="bd5a3-1047">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1047">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="bd5a3-1048">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1048">wiFiScanInterval</span></span>|<span data-ttu-id="bd5a3-1049">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1049">Int32</span></span>|<span data-ttu-id="bd5a3-1050">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1050">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="bd5a3-1051">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1051">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="bd5a3-1052">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1052">Valid values 1 to 500</span></span>|
|<span data-ttu-id="bd5a3-1053">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1053">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="bd5a3-1054">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1054">Boolean</span></span>|<span data-ttu-id="bd5a3-1055">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1055">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="bd5a3-1056">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1056">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="bd5a3-1057">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1057">Boolean</span></span>|<span data-ttu-id="bd5a3-1058">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1058">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="bd5a3-1059">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1059">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="bd5a3-1060">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1060">Boolean</span></span>|<span data-ttu-id="bd5a3-1061">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1061">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="bd5a3-1062">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1062">windowsStoreBlocked</span></span>|<span data-ttu-id="bd5a3-1063">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1063">Boolean</span></span>|<span data-ttu-id="bd5a3-1064">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1064">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="bd5a3-1065">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1065">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="bd5a3-1066">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1066">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="bd5a3-1067">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1067">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="bd5a3-1068">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1068">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="bd5a3-1069">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1069">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="bd5a3-1070">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1070">Boolean</span></span>|<span data-ttu-id="bd5a3-1071">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1071">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="bd5a3-1072">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1072">developerUnlockSetting</span></span>|[<span data-ttu-id="bd5a3-1073">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1073">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="bd5a3-1074">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1074">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="bd5a3-1075">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1075">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="bd5a3-1076">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1076">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="bd5a3-1077">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1077">Boolean</span></span>|<span data-ttu-id="bd5a3-1078">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1078">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="bd5a3-1079">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1079">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="bd5a3-1080">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1080">Boolean</span></span>|<span data-ttu-id="bd5a3-1081">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1081">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="bd5a3-1082">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1082">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="bd5a3-1083">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1083">Boolean</span></span>|<span data-ttu-id="bd5a3-1084">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1084">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="bd5a3-1085">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1085">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="bd5a3-1086">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1086">Boolean</span></span>|<span data-ttu-id="bd5a3-1087">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1087">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="bd5a3-1088">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1088">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="bd5a3-1089">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1089">Boolean</span></span>|<span data-ttu-id="bd5a3-1090">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1090">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="bd5a3-1091">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1091">gameDvrBlocked</span></span>|<span data-ttu-id="bd5a3-1092">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1092">Boolean</span></span>|<span data-ttu-id="bd5a3-1093">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1093">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="bd5a3-1094">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1094">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="bd5a3-1095">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1095">Boolean</span></span>|<span data-ttu-id="bd5a3-1096">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1096">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="bd5a3-1097">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1097">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="bd5a3-1098">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1098">Boolean</span></span>|<span data-ttu-id="bd5a3-1099">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1099">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="bd5a3-1100">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1100">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="bd5a3-1101">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1101">Boolean</span></span>|<span data-ttu-id="bd5a3-1102">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1102">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="bd5a3-1103">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1103">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="bd5a3-1104">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1104">Boolean</span></span>|<span data-ttu-id="bd5a3-1105">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1105">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="bd5a3-1106">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1106">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="bd5a3-1107">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1107">Boolean</span></span>|<span data-ttu-id="bd5a3-1108">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1108">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="bd5a3-1109">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1109">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="bd5a3-1110">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1110">Boolean</span></span>|<span data-ttu-id="bd5a3-1111">此策略设置允许用户更改通常仅供系统管理员使用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1111">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="bd5a3-1112">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1112">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="bd5a3-1113">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1113">Boolean</span></span>|<span data-ttu-id="bd5a3-1114">此策略设置指示 Windows Installer 在系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1114">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="bd5a3-1115">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1115">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="bd5a3-1116">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1116">Boolean</span></span>|<span data-ttu-id="bd5a3-1117">通过此策略设置，您可以阻止所有热插拔 PCI 下游端口的直接内存访问（DMA），直到用户登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1117">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="bd5a3-1118">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1118">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="bd5a3-1119">String collection</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1119">String collection</span></span>|<span data-ttu-id="bd5a3-1120">Windows 应用的以分号分隔的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1120">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="bd5a3-1121">登录后将启动列出的 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1121">Listed Windows apps are to be launched after logon.</span></span>|
|<span data-ttu-id="bd5a3-1122">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1122">uninstallBuiltInApps</span></span>|<span data-ttu-id="bd5a3-1123">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1123">Boolean</span></span>|<span data-ttu-id="bd5a3-1124">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1124">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="bd5a3-1125">响应</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1125">Response</span></span>
<span data-ttu-id="bd5a3-1126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1126">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd5a3-1127">示例</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1127">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd5a3-1128">请求</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1128">Request</span></span>
<span data-ttu-id="bd5a3-1129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="bd5a3-1130">响应</span><span class="sxs-lookup"><span data-stu-id="bd5a3-1130">Response</span></span>
<span data-ttu-id="bd5a3-p196">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd5a3-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





