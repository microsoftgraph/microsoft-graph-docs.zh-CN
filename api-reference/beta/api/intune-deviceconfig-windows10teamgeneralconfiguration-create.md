---
title: 创建 windows10TeamGeneralConfiguration
description: 创建新的 windows10TeamGeneralConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1d343e9b654234c9ededd7713be787c4f58d62e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977952"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="b1788-103">创建 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1788-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="b1788-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1788-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1788-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1788-106">创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1788-106">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1788-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1788-107">Prerequisites</span></span>
<span data-ttu-id="b1788-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1788-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1788-110">Permission type</span></span>|<span data-ttu-id="b1788-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1788-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1788-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1788-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1788-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1788-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1788-115">Not supported.</span></span>|
|<span data-ttu-id="b1788-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1788-116">Application</span></span>|<span data-ttu-id="b1788-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1788-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1788-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b1788-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1788-119">Request headers</span></span>
|<span data-ttu-id="b1788-120">标头</span><span class="sxs-lookup"><span data-stu-id="b1788-120">Header</span></span>|<span data-ttu-id="b1788-121">值</span><span class="sxs-lookup"><span data-stu-id="b1788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1788-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1788-122">Authorization</span></span>|<span data-ttu-id="b1788-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1788-124">接受</span><span class="sxs-lookup"><span data-stu-id="b1788-124">Accept</span></span>|<span data-ttu-id="b1788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1788-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1788-126">Request body</span></span>
<span data-ttu-id="b1788-127">在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1788-127">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="b1788-128">下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1788-128">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="b1788-129">属性</span><span class="sxs-lookup"><span data-stu-id="b1788-129">Property</span></span>|<span data-ttu-id="b1788-130">类型</span><span class="sxs-lookup"><span data-stu-id="b1788-130">Type</span></span>|<span data-ttu-id="b1788-131">说明</span><span class="sxs-lookup"><span data-stu-id="b1788-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1788-132">id</span><span class="sxs-lookup"><span data-stu-id="b1788-132">id</span></span>|<span data-ttu-id="b1788-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b1788-133">String</span></span>|<span data-ttu-id="b1788-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1788-134">Key of the entity.</span></span> <span data-ttu-id="b1788-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1788-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b1788-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1788-137">DateTimeOffset</span></span>|<span data-ttu-id="b1788-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1788-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b1788-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1788-140">roleScopeTagIds</span></span>|<span data-ttu-id="b1788-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b1788-141">String collection</span></span>|<span data-ttu-id="b1788-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b1788-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1788-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b1788-144">supportsScopeTags</span></span>|<span data-ttu-id="b1788-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-145">Boolean</span></span>|<span data-ttu-id="b1788-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b1788-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b1788-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b1788-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b1788-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b1788-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b1788-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b1788-149">This property is read-only.</span></span> <span data-ttu-id="b1788-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1788-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b1788-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1788-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b1788-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b1788-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b1788-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1788-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b1788-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1788-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b1788-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b1788-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b1788-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1788-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b1788-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1788-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b1788-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b1788-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b1788-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1788-163">createdDateTime</span></span>|<span data-ttu-id="b1788-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1788-164">DateTimeOffset</span></span>|<span data-ttu-id="b1788-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1788-165">DateTime the object was created.</span></span> <span data-ttu-id="b1788-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-167">说明</span><span class="sxs-lookup"><span data-stu-id="b1788-167">description</span></span>|<span data-ttu-id="b1788-168">String</span><span class="sxs-lookup"><span data-stu-id="b1788-168">String</span></span>|<span data-ttu-id="b1788-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b1788-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1788-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b1788-171">displayName</span></span>|<span data-ttu-id="b1788-172">字符串</span><span class="sxs-lookup"><span data-stu-id="b1788-172">String</span></span>|<span data-ttu-id="b1788-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b1788-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1788-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-175">version</span><span class="sxs-lookup"><span data-stu-id="b1788-175">version</span></span>|<span data-ttu-id="b1788-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b1788-176">Int32</span></span>|<span data-ttu-id="b1788-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b1788-177">Version of the device configuration.</span></span> <span data-ttu-id="b1788-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1788-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1788-179">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="b1788-179">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="b1788-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-180">Boolean</span></span>|<span data-ttu-id="b1788-181">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="b1788-181">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="b1788-182">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="b1788-182">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="b1788-183">String</span><span class="sxs-lookup"><span data-stu-id="b1788-183">String</span></span>|<span data-ttu-id="b1788-184">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="b1788-184">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="b1788-185">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="b1788-185">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="b1788-186">String</span><span class="sxs-lookup"><span data-stu-id="b1788-186">String</span></span>|<span data-ttu-id="b1788-187">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="b1788-187">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="b1788-188">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="b1788-188">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="b1788-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-189">Boolean</span></span>|<span data-ttu-id="b1788-190">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="b1788-190">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="b1788-191">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="b1788-191">maintenanceWindowBlocked</span></span>|<span data-ttu-id="b1788-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-192">Boolean</span></span>|<span data-ttu-id="b1788-193">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="b1788-193">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="b1788-194">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="b1788-194">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="b1788-195">Int32</span><span class="sxs-lookup"><span data-stu-id="b1788-195">Int32</span></span>|<span data-ttu-id="b1788-196">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="b1788-196">Maintenance window duration for device updates.</span></span> <span data-ttu-id="b1788-197">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="b1788-197">Valid values 0 to 5</span></span>|
|<span data-ttu-id="b1788-198">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="b1788-198">maintenanceWindowStartTime</span></span>|<span data-ttu-id="b1788-199">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b1788-199">TimeOfDay</span></span>|<span data-ttu-id="b1788-200">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="b1788-200">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="b1788-201">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="b1788-201">miracastChannel</span></span>|[<span data-ttu-id="b1788-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="b1788-202">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="b1788-203">频道。</span><span class="sxs-lookup"><span data-stu-id="b1788-203">The channel.</span></span> <span data-ttu-id="b1788-204">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="b1788-204">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="b1788-205">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="b1788-205">miracastBlocked</span></span>|<span data-ttu-id="b1788-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-206">Boolean</span></span>|<span data-ttu-id="b1788-207">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="b1788-207">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="b1788-208">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="b1788-208">miracastRequirePin</span></span>|<span data-ttu-id="b1788-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-209">Boolean</span></span>|<span data-ttu-id="b1788-210">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="b1788-210">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="b1788-211">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="b1788-211">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="b1788-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-212">Boolean</span></span>|<span data-ttu-id="b1788-213">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="b1788-213">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="b1788-214">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="b1788-214">settingsBlockSessionResume</span></span>|<span data-ttu-id="b1788-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-215">Boolean</span></span>|<span data-ttu-id="b1788-216">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="b1788-216">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="b1788-217">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="b1788-217">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="b1788-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-218">Boolean</span></span>|<span data-ttu-id="b1788-219">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="b1788-219">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="b1788-220">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="b1788-220">settingsDefaultVolume</span></span>|<span data-ttu-id="b1788-221">Int32</span><span class="sxs-lookup"><span data-stu-id="b1788-221">Int32</span></span>|<span data-ttu-id="b1788-222">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="b1788-222">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="b1788-223">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="b1788-223">Permitted values are 0-100.</span></span> <span data-ttu-id="b1788-224">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="b1788-224">The default is 45.</span></span> <span data-ttu-id="b1788-225">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="b1788-225">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b1788-226">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b1788-226">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="b1788-227">Int32</span><span class="sxs-lookup"><span data-stu-id="b1788-227">Int32</span></span>|<span data-ttu-id="b1788-228">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b1788-228">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="b1788-229">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b1788-229">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="b1788-230">Int32</span><span class="sxs-lookup"><span data-stu-id="b1788-230">Int32</span></span>|<span data-ttu-id="b1788-231">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b1788-231">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="b1788-232">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b1788-232">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="b1788-233">Int32</span><span class="sxs-lookup"><span data-stu-id="b1788-233">Int32</span></span>|<span data-ttu-id="b1788-234">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b1788-234">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="b1788-235">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="b1788-235">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="b1788-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1788-236">Boolean</span></span>|<span data-ttu-id="b1788-237">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="b1788-237">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="b1788-238">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="b1788-238">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="b1788-239">String</span><span class="sxs-lookup"><span data-stu-id="b1788-239">String</span></span>|<span data-ttu-id="b1788-240">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="b1788-240">The welcome screen background image URL.</span></span> <span data-ttu-id="b1788-241">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="b1788-241">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="b1788-242">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="b1788-242">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="b1788-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="b1788-243">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="b1788-244">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="b1788-244">The welcome screen meeting information shown.</span></span> <span data-ttu-id="b1788-245">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="b1788-245">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="b1788-246">响应</span><span class="sxs-lookup"><span data-stu-id="b1788-246">Response</span></span>
<span data-ttu-id="b1788-247">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1788-247">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1788-248">示例</span><span class="sxs-lookup"><span data-stu-id="b1788-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1788-249">请求</span><span class="sxs-lookup"><span data-stu-id="b1788-249">Request</span></span>
<span data-ttu-id="b1788-250">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1788-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2015

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="b1788-251">响应</span><span class="sxs-lookup"><span data-stu-id="b1788-251">Response</span></span>
<span data-ttu-id="b1788-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1788-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2187

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```





