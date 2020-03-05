---
title: 创建 iosUpdateConfiguration
description: 创建新的 iosUpdateConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07696492fcbc38a3b042d1c6490bdf027d16e5e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442640"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="efcb1-103">创建 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="efcb1-103">Create iosUpdateConfiguration</span></span>

<span data-ttu-id="efcb1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="efcb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efcb1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efcb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efcb1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efcb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efcb1-107">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efcb1-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efcb1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="efcb1-108">Prerequisites</span></span>
<span data-ttu-id="efcb1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efcb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efcb1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="efcb1-111">Permission type</span></span>|<span data-ttu-id="efcb1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efcb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efcb1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efcb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efcb1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcb1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efcb1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efcb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efcb1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="efcb1-116">Not supported.</span></span>|
|<span data-ttu-id="efcb1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="efcb1-117">Application</span></span>|<span data-ttu-id="efcb1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcb1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efcb1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efcb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="efcb1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="efcb1-120">Request headers</span></span>
|<span data-ttu-id="efcb1-121">标头</span><span class="sxs-lookup"><span data-stu-id="efcb1-121">Header</span></span>|<span data-ttu-id="efcb1-122">值</span><span class="sxs-lookup"><span data-stu-id="efcb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efcb1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="efcb1-123">Authorization</span></span>|<span data-ttu-id="efcb1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efcb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efcb1-125">接受</span><span class="sxs-lookup"><span data-stu-id="efcb1-125">Accept</span></span>|<span data-ttu-id="efcb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efcb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efcb1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="efcb1-127">Request body</span></span>
<span data-ttu-id="efcb1-128">在请求正文中，提供 iosUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efcb1-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="efcb1-129">下表显示创建 iosUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="efcb1-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="efcb1-130">属性</span><span class="sxs-lookup"><span data-stu-id="efcb1-130">Property</span></span>|<span data-ttu-id="efcb1-131">类型</span><span class="sxs-lookup"><span data-stu-id="efcb1-131">Type</span></span>|<span data-ttu-id="efcb1-132">说明</span><span class="sxs-lookup"><span data-stu-id="efcb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efcb1-133">id</span><span class="sxs-lookup"><span data-stu-id="efcb1-133">id</span></span>|<span data-ttu-id="efcb1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="efcb1-134">String</span></span>|<span data-ttu-id="efcb1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="efcb1-135">Key of the entity.</span></span> <span data-ttu-id="efcb1-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efcb1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="efcb1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcb1-138">DateTimeOffset</span></span>|<span data-ttu-id="efcb1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="efcb1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="efcb1-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efcb1-141">roleScopeTagIds</span></span>|<span data-ttu-id="efcb1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="efcb1-142">String collection</span></span>|<span data-ttu-id="efcb1-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="efcb1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="efcb1-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="efcb1-145">supportsScopeTags</span></span>|<span data-ttu-id="efcb1-146">布尔</span><span class="sxs-lookup"><span data-stu-id="efcb1-146">Boolean</span></span>|<span data-ttu-id="efcb1-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="efcb1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="efcb1-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="efcb1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="efcb1-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="efcb1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="efcb1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="efcb1-150">This property is read-only.</span></span> <span data-ttu-id="efcb1-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="efcb1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="efcb1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="efcb1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="efcb1-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="efcb1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="efcb1-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="efcb1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="efcb1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="efcb1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="efcb1-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="efcb1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="efcb1-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="efcb1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="efcb1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="efcb1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="efcb1-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="efcb1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="efcb1-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efcb1-164">createdDateTime</span></span>|<span data-ttu-id="efcb1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcb1-165">DateTimeOffset</span></span>|<span data-ttu-id="efcb1-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="efcb1-166">DateTime the object was created.</span></span> <span data-ttu-id="efcb1-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-168">说明</span><span class="sxs-lookup"><span data-stu-id="efcb1-168">description</span></span>|<span data-ttu-id="efcb1-169">String</span><span class="sxs-lookup"><span data-stu-id="efcb1-169">String</span></span>|<span data-ttu-id="efcb1-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="efcb1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="efcb1-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="efcb1-172">displayName</span></span>|<span data-ttu-id="efcb1-173">String</span><span class="sxs-lookup"><span data-stu-id="efcb1-173">String</span></span>|<span data-ttu-id="efcb1-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="efcb1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="efcb1-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-176">version</span><span class="sxs-lookup"><span data-stu-id="efcb1-176">version</span></span>|<span data-ttu-id="efcb1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="efcb1-177">Int32</span></span>|<span data-ttu-id="efcb1-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="efcb1-178">Version of the device configuration.</span></span> <span data-ttu-id="efcb1-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efcb1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efcb1-180">isEnabled</span><span class="sxs-lookup"><span data-stu-id="efcb1-180">isEnabled</span></span>|<span data-ttu-id="efcb1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="efcb1-181">Boolean</span></span>|<span data-ttu-id="efcb1-182">在 UI 中是否启用了设置</span><span class="sxs-lookup"><span data-stu-id="efcb1-182">Is setting enabled in UI</span></span>|
|<span data-ttu-id="efcb1-183">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="efcb1-183">activeHoursStart</span></span>|<span data-ttu-id="efcb1-184">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="efcb1-184">TimeOfDay</span></span>|<span data-ttu-id="efcb1-185">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="efcb1-185">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="efcb1-186">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="efcb1-186">activeHoursEnd</span></span>|<span data-ttu-id="efcb1-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="efcb1-187">TimeOfDay</span></span>|<span data-ttu-id="efcb1-188">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="efcb1-188">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="efcb1-189">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="efcb1-189">desiredOsVersion</span></span>|<span data-ttu-id="efcb1-190">String</span><span class="sxs-lookup"><span data-stu-id="efcb1-190">String</span></span>|<span data-ttu-id="efcb1-191">如果未指定，设备将更新到最新版本的操作系统。</span><span class="sxs-lookup"><span data-stu-id="efcb1-191">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="efcb1-192">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="efcb1-192">scheduledInstallDays</span></span>|<span data-ttu-id="efcb1-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="efcb1-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="efcb1-194">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="efcb1-194">Days in week for which active hours are configured.</span></span> <span data-ttu-id="efcb1-195">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="efcb1-195">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="efcb1-196">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="efcb1-196">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="efcb1-197">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="efcb1-197">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="efcb1-198">Int32</span><span class="sxs-lookup"><span data-stu-id="efcb1-198">Int32</span></span>|<span data-ttu-id="efcb1-199">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="efcb1-199">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="efcb1-200">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="efcb1-200">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="efcb1-201">Int32</span><span class="sxs-lookup"><span data-stu-id="efcb1-201">Int32</span></span>|<span data-ttu-id="efcb1-202">软件更新在 iOS 设备中可见的天数，范围从0到90（含0到）</span><span class="sxs-lookup"><span data-stu-id="efcb1-202">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="efcb1-203">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="efcb1-203">updateScheduleType</span></span>|[<span data-ttu-id="efcb1-204">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="efcb1-204">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="efcb1-205">更新计划类型。</span><span class="sxs-lookup"><span data-stu-id="efcb1-205">Update schedule type.</span></span> <span data-ttu-id="efcb1-206">可取值为：`updateOutsideOfActiveHours`、`alwaysUpdate`、`updateDuringTimeWindows`、`updateOutsideOfTimeWindows`。</span><span class="sxs-lookup"><span data-stu-id="efcb1-206">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="efcb1-207">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="efcb1-207">customUpdateTimeWindows</span></span>|<span data-ttu-id="efcb1-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)集合</span><span class="sxs-lookup"><span data-stu-id="efcb1-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="efcb1-209">如果将 "更新计划类型" 设置为 "使用时间窗口计划"，则将计划更新的自定义时间窗口。</span><span class="sxs-lookup"><span data-stu-id="efcb1-209">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="efcb1-210">此集合最多可包含20个元素。</span><span class="sxs-lookup"><span data-stu-id="efcb1-210">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="efcb1-211">响应</span><span class="sxs-lookup"><span data-stu-id="efcb1-211">Response</span></span>
<span data-ttu-id="efcb1-212">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efcb1-212">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efcb1-213">示例</span><span class="sxs-lookup"><span data-stu-id="efcb1-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="efcb1-214">请求</span><span class="sxs-lookup"><span data-stu-id="efcb1-214">Request</span></span>
<span data-ttu-id="efcb1-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efcb1-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1596

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="efcb1-216">响应</span><span class="sxs-lookup"><span data-stu-id="efcb1-216">Response</span></span>
<span data-ttu-id="efcb1-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efcb1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1768

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```





