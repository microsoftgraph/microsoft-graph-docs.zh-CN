---
title: 创建 macOSSoftwareUpdateConfiguration
description: 创建新的 macOSSoftwareUpdateConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60213d720d1229f14d4b83d83dc5c0da52fbea86
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704970"
---
# <a name="create-macossoftwareupdateconfiguration"></a><span data-ttu-id="be17a-103">创建 macOSSoftwareUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="be17a-103">Create macOSSoftwareUpdateConfiguration</span></span>

<span data-ttu-id="be17a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be17a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be17a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be17a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be17a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be17a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be17a-107">创建新的 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be17a-107">Create a new [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be17a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="be17a-108">Prerequisites</span></span>
<span data-ttu-id="be17a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be17a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be17a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="be17a-111">Permission type</span></span>|<span data-ttu-id="be17a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be17a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be17a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be17a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be17a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be17a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be17a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be17a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be17a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be17a-116">Not supported.</span></span>|
|<span data-ttu-id="be17a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="be17a-117">Application</span></span>|<span data-ttu-id="be17a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be17a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be17a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be17a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="be17a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="be17a-120">Request headers</span></span>
|<span data-ttu-id="be17a-121">标头</span><span class="sxs-lookup"><span data-stu-id="be17a-121">Header</span></span>|<span data-ttu-id="be17a-122">值</span><span class="sxs-lookup"><span data-stu-id="be17a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be17a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be17a-123">Authorization</span></span>|<span data-ttu-id="be17a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be17a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be17a-125">接受</span><span class="sxs-lookup"><span data-stu-id="be17a-125">Accept</span></span>|<span data-ttu-id="be17a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be17a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be17a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="be17a-127">Request body</span></span>
<span data-ttu-id="be17a-128">在请求正文中，提供 macOSSoftwareUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be17a-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateConfiguration object.</span></span>

<span data-ttu-id="be17a-129">下表显示创建 macOSSoftwareUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be17a-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateConfiguration.</span></span>

|<span data-ttu-id="be17a-130">属性</span><span class="sxs-lookup"><span data-stu-id="be17a-130">Property</span></span>|<span data-ttu-id="be17a-131">类型</span><span class="sxs-lookup"><span data-stu-id="be17a-131">Type</span></span>|<span data-ttu-id="be17a-132">说明</span><span class="sxs-lookup"><span data-stu-id="be17a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be17a-133">id</span><span class="sxs-lookup"><span data-stu-id="be17a-133">id</span></span>|<span data-ttu-id="be17a-134">String</span><span class="sxs-lookup"><span data-stu-id="be17a-134">String</span></span>|<span data-ttu-id="be17a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be17a-135">Key of the entity.</span></span> <span data-ttu-id="be17a-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be17a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="be17a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be17a-138">DateTimeOffset</span></span>|<span data-ttu-id="be17a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="be17a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="be17a-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be17a-141">roleScopeTagIds</span></span>|<span data-ttu-id="be17a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="be17a-142">String collection</span></span>|<span data-ttu-id="be17a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="be17a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="be17a-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="be17a-145">supportsScopeTags</span></span>|<span data-ttu-id="be17a-146">布尔</span><span class="sxs-lookup"><span data-stu-id="be17a-146">Boolean</span></span>|<span data-ttu-id="be17a-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="be17a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="be17a-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="be17a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="be17a-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="be17a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="be17a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="be17a-150">This property is read-only.</span></span> <span data-ttu-id="be17a-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be17a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="be17a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be17a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="be17a-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="be17a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="be17a-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="be17a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="be17a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="be17a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="be17a-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="be17a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="be17a-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="be17a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="be17a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="be17a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="be17a-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="be17a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="be17a-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be17a-164">createdDateTime</span></span>|<span data-ttu-id="be17a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be17a-165">DateTimeOffset</span></span>|<span data-ttu-id="be17a-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="be17a-166">DateTime the object was created.</span></span> <span data-ttu-id="be17a-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-168">说明</span><span class="sxs-lookup"><span data-stu-id="be17a-168">description</span></span>|<span data-ttu-id="be17a-169">String</span><span class="sxs-lookup"><span data-stu-id="be17a-169">String</span></span>|<span data-ttu-id="be17a-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="be17a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be17a-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="be17a-172">displayName</span></span>|<span data-ttu-id="be17a-173">String</span><span class="sxs-lookup"><span data-stu-id="be17a-173">String</span></span>|<span data-ttu-id="be17a-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="be17a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be17a-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-176">version</span><span class="sxs-lookup"><span data-stu-id="be17a-176">version</span></span>|<span data-ttu-id="be17a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="be17a-177">Int32</span></span>|<span data-ttu-id="be17a-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="be17a-178">Version of the device configuration.</span></span> <span data-ttu-id="be17a-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be17a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be17a-180">criticalUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-180">criticalUpdateBehavior</span></span>|[<span data-ttu-id="be17a-181">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-181">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="be17a-182">更新关键更新的行为。</span><span class="sxs-lookup"><span data-stu-id="be17a-182">Update behavior for critical updates.</span></span> <span data-ttu-id="be17a-183">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="be17a-183">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="be17a-184">configDataUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-184">configDataUpdateBehavior</span></span>|[<span data-ttu-id="be17a-185">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-185">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="be17a-186">更新配置数据文件更新的行为。</span><span class="sxs-lookup"><span data-stu-id="be17a-186">Update behavior for configuration data file updates.</span></span> <span data-ttu-id="be17a-187">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="be17a-187">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="be17a-188">firmwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-188">firmwareUpdateBehavior</span></span>|[<span data-ttu-id="be17a-189">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-189">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="be17a-190">更新固件更新的行为。</span><span class="sxs-lookup"><span data-stu-id="be17a-190">Update behavior for firmware updates.</span></span> <span data-ttu-id="be17a-191">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="be17a-191">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="be17a-192">allOtherUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-192">allOtherUpdateBehavior</span></span>|[<span data-ttu-id="be17a-193">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="be17a-193">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="be17a-194">更新所有其他更新的行为。</span><span class="sxs-lookup"><span data-stu-id="be17a-194">Update behavior for all other updates.</span></span> <span data-ttu-id="be17a-195">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="be17a-195">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="be17a-196">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="be17a-196">updateScheduleType</span></span>|[<span data-ttu-id="be17a-197">macOSSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="be17a-197">macOSSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|<span data-ttu-id="be17a-198">更新计划类型。</span><span class="sxs-lookup"><span data-stu-id="be17a-198">Update schedule type.</span></span> <span data-ttu-id="be17a-199">可取值为：`alwaysUpdate`、`updateDuringTimeWindows`、`updateOutsideOfTimeWindows`。</span><span class="sxs-lookup"><span data-stu-id="be17a-199">Possible values are: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="be17a-200">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="be17a-200">customUpdateTimeWindows</span></span>|<span data-ttu-id="be17a-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be17a-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="be17a-202">将允许或阻止更新时的自定义时间窗口。</span><span class="sxs-lookup"><span data-stu-id="be17a-202">Custom Time windows when updates will be allowed or blocked.</span></span> <span data-ttu-id="be17a-203">此集合最多可包含20个元素。</span><span class="sxs-lookup"><span data-stu-id="be17a-203">This collection can contain a maximum of 20 elements.</span></span>|
|<span data-ttu-id="be17a-204">updateTimeWindowUtcOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="be17a-204">updateTimeWindowUtcOffsetInMinutes</span></span>|<span data-ttu-id="be17a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="be17a-205">Int32</span></span>|<span data-ttu-id="be17a-206">表示每个更新时间窗口的 UTC 偏移量的分钟数</span><span class="sxs-lookup"><span data-stu-id="be17a-206">Minutes indicating UTC offset for each update time window</span></span>|



## <a name="response"></a><span data-ttu-id="be17a-207">响应</span><span class="sxs-lookup"><span data-stu-id="be17a-207">Response</span></span>
<span data-ttu-id="be17a-208">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be17a-208">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be17a-209">示例</span><span class="sxs-lookup"><span data-stu-id="be17a-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="be17a-210">请求</span><span class="sxs-lookup"><span data-stu-id="be17a-210">Request</span></span>
<span data-ttu-id="be17a-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be17a-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1542

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```

### <a name="response"></a><span data-ttu-id="be17a-212">响应</span><span class="sxs-lookup"><span data-stu-id="be17a-212">Response</span></span>
<span data-ttu-id="be17a-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be17a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1714

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
  "id": "b8e467ac-67ac-b8e4-ac67-e4b8ac67e4b8",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```





