---
title: 更新 windowsPhone81GeneralConfiguration
description: 更新 windowsPhone81GeneralConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59099489349d7a9f3e874f8e5b1005d192f3e895
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961628"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="93eb9-103">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="93eb9-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="93eb9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93eb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93eb9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93eb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93eb9-106">更新 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93eb9-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93eb9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="93eb9-107">Prerequisites</span></span>
<span data-ttu-id="93eb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93eb9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="93eb9-110">Permission type</span></span>|<span data-ttu-id="93eb9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93eb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93eb9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93eb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93eb9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93eb9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93eb9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93eb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93eb9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93eb9-115">Not supported.</span></span>|
|<span data-ttu-id="93eb9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="93eb9-116">Application</span></span>|<span data-ttu-id="93eb9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="93eb9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93eb9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93eb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="93eb9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93eb9-119">Request headers</span></span>
|<span data-ttu-id="93eb9-120">标头</span><span class="sxs-lookup"><span data-stu-id="93eb9-120">Header</span></span>|<span data-ttu-id="93eb9-121">值</span><span class="sxs-lookup"><span data-stu-id="93eb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93eb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93eb9-122">Authorization</span></span>|<span data-ttu-id="93eb9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93eb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93eb9-124">接受</span><span class="sxs-lookup"><span data-stu-id="93eb9-124">Accept</span></span>|<span data-ttu-id="93eb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93eb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93eb9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="93eb9-126">Request body</span></span>
<span data-ttu-id="93eb9-127">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93eb9-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="93eb9-128">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93eb9-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="93eb9-129">属性</span><span class="sxs-lookup"><span data-stu-id="93eb9-129">Property</span></span>|<span data-ttu-id="93eb9-130">类型</span><span class="sxs-lookup"><span data-stu-id="93eb9-130">Type</span></span>|<span data-ttu-id="93eb9-131">说明</span><span class="sxs-lookup"><span data-stu-id="93eb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93eb9-132">id</span><span class="sxs-lookup"><span data-stu-id="93eb9-132">id</span></span>|<span data-ttu-id="93eb9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="93eb9-133">String</span></span>|<span data-ttu-id="93eb9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="93eb9-134">Key of the entity.</span></span> <span data-ttu-id="93eb9-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93eb9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="93eb9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93eb9-137">DateTimeOffset</span></span>|<span data-ttu-id="93eb9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93eb9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="93eb9-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93eb9-140">roleScopeTagIds</span></span>|<span data-ttu-id="93eb9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="93eb9-141">String collection</span></span>|<span data-ttu-id="93eb9-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="93eb9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93eb9-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="93eb9-144">supportsScopeTags</span></span>|<span data-ttu-id="93eb9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-145">Boolean</span></span>|<span data-ttu-id="93eb9-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="93eb9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="93eb9-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="93eb9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="93eb9-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="93eb9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="93eb9-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="93eb9-149">This property is read-only.</span></span> <span data-ttu-id="93eb9-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="93eb9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="93eb9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="93eb9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="93eb9-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="93eb9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="93eb9-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="93eb9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="93eb9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="93eb9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="93eb9-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="93eb9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="93eb9-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="93eb9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="93eb9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="93eb9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="93eb9-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="93eb9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="93eb9-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93eb9-163">createdDateTime</span></span>|<span data-ttu-id="93eb9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93eb9-164">DateTimeOffset</span></span>|<span data-ttu-id="93eb9-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93eb9-165">DateTime the object was created.</span></span> <span data-ttu-id="93eb9-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-167">说明</span><span class="sxs-lookup"><span data-stu-id="93eb9-167">description</span></span>|<span data-ttu-id="93eb9-168">String</span><span class="sxs-lookup"><span data-stu-id="93eb9-168">String</span></span>|<span data-ttu-id="93eb9-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="93eb9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93eb9-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="93eb9-171">displayName</span></span>|<span data-ttu-id="93eb9-172">String</span><span class="sxs-lookup"><span data-stu-id="93eb9-172">String</span></span>|<span data-ttu-id="93eb9-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="93eb9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93eb9-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-175">version</span><span class="sxs-lookup"><span data-stu-id="93eb9-175">version</span></span>|<span data-ttu-id="93eb9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-176">Int32</span></span>|<span data-ttu-id="93eb9-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="93eb9-177">Version of the device configuration.</span></span> <span data-ttu-id="93eb9-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93eb9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93eb9-179">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="93eb9-179">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="93eb9-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-180">Boolean</span></span>|<span data-ttu-id="93eb9-181">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="93eb9-181">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="93eb9-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="93eb9-182">This property is read-only.</span></span>|
|<span data-ttu-id="93eb9-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="93eb9-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="93eb9-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-184">Boolean</span></span>|<span data-ttu-id="93eb9-185">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="93eb9-185">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="93eb9-186">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-186">bluetoothBlocked</span></span>|<span data-ttu-id="93eb9-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-187">Boolean</span></span>|<span data-ttu-id="93eb9-188">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="93eb9-188">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="93eb9-189">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-189">cameraBlocked</span></span>|<span data-ttu-id="93eb9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-190">Boolean</span></span>|<span data-ttu-id="93eb9-191">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="93eb9-191">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="93eb9-192">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="93eb9-192">cellularBlockWifiTethering</span></span>|<span data-ttu-id="93eb9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-193">Boolean</span></span>|<span data-ttu-id="93eb9-194">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="93eb9-194">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="93eb9-195">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="93eb9-195">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="93eb9-196">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="93eb9-196">compliantAppsList</span></span>|<span data-ttu-id="93eb9-197">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93eb9-197">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="93eb9-198">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="93eb9-198">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="93eb9-199">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="93eb9-199">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="93eb9-200">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="93eb9-200">compliantAppListType</span></span>|[<span data-ttu-id="93eb9-201">appListType</span><span class="sxs-lookup"><span data-stu-id="93eb9-201">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="93eb9-202">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="93eb9-202">List that is in the AppComplianceList.</span></span> <span data-ttu-id="93eb9-203">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="93eb9-203">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="93eb9-204">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="93eb9-204">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="93eb9-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-205">Boolean</span></span>|<span data-ttu-id="93eb9-206">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="93eb9-206">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="93eb9-207">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="93eb9-207">emailBlockAddingAccounts</span></span>|<span data-ttu-id="93eb9-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-208">Boolean</span></span>|<span data-ttu-id="93eb9-209">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="93eb9-209">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="93eb9-210">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-210">locationServicesBlocked</span></span>|<span data-ttu-id="93eb9-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-211">Boolean</span></span>|<span data-ttu-id="93eb9-212">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="93eb9-212">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="93eb9-213">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-213">microsoftAccountBlocked</span></span>|<span data-ttu-id="93eb9-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-214">Boolean</span></span>|<span data-ttu-id="93eb9-215">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="93eb9-215">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="93eb9-216">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-216">nfcBlocked</span></span>|<span data-ttu-id="93eb9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-217">Boolean</span></span>|<span data-ttu-id="93eb9-218">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="93eb9-218">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="93eb9-219">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="93eb9-219">passwordBlockSimple</span></span>|<span data-ttu-id="93eb9-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-220">Boolean</span></span>|<span data-ttu-id="93eb9-221">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="93eb9-221">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="93eb9-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="93eb9-222">passwordExpirationDays</span></span>|<span data-ttu-id="93eb9-223">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-223">Int32</span></span>|<span data-ttu-id="93eb9-224">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="93eb9-224">Number of days before the password expires.</span></span>|
|<span data-ttu-id="93eb9-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="93eb9-225">passwordMinimumLength</span></span>|<span data-ttu-id="93eb9-226">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-226">Int32</span></span>|<span data-ttu-id="93eb9-227">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="93eb9-227">Minimum length of passwords.</span></span>|
|<span data-ttu-id="93eb9-228">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="93eb9-228">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="93eb9-229">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-229">Int32</span></span>|<span data-ttu-id="93eb9-230">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="93eb9-230">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="93eb9-231">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="93eb9-231">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="93eb9-232">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-232">Int32</span></span>|<span data-ttu-id="93eb9-233">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="93eb9-233">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="93eb9-234">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="93eb9-234">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="93eb9-235">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-235">Int32</span></span>|<span data-ttu-id="93eb9-236">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="93eb9-236">Number of previous passwords to block.</span></span> <span data-ttu-id="93eb9-237">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="93eb9-237">Valid values 0 to 24</span></span>|
|<span data-ttu-id="93eb9-238">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="93eb9-238">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="93eb9-239">Int32</span><span class="sxs-lookup"><span data-stu-id="93eb9-239">Int32</span></span>|<span data-ttu-id="93eb9-240">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="93eb9-240">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="93eb9-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="93eb9-241">passwordRequiredType</span></span>|[<span data-ttu-id="93eb9-242">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="93eb9-242">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="93eb9-243">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="93eb9-243">Password type that is required.</span></span> <span data-ttu-id="93eb9-244">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="93eb9-244">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="93eb9-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="93eb9-245">passwordRequired</span></span>|<span data-ttu-id="93eb9-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-246">Boolean</span></span>|<span data-ttu-id="93eb9-247">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="93eb9-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="93eb9-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-248">screenCaptureBlocked</span></span>|<span data-ttu-id="93eb9-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-249">Boolean</span></span>|<span data-ttu-id="93eb9-250">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="93eb9-250">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="93eb9-251">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="93eb9-251">storageBlockRemovableStorage</span></span>|<span data-ttu-id="93eb9-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-252">Boolean</span></span>|<span data-ttu-id="93eb9-253">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="93eb9-253">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="93eb9-254">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="93eb9-254">storageRequireEncryption</span></span>|<span data-ttu-id="93eb9-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-255">Boolean</span></span>|<span data-ttu-id="93eb9-256">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="93eb9-256">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="93eb9-257">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-257">webBrowserBlocked</span></span>|<span data-ttu-id="93eb9-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-258">Boolean</span></span>|<span data-ttu-id="93eb9-259">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="93eb9-259">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="93eb9-260">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-260">wifiBlocked</span></span>|<span data-ttu-id="93eb9-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-261">Boolean</span></span>|<span data-ttu-id="93eb9-262">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="93eb9-262">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="93eb9-263">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="93eb9-263">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="93eb9-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-264">Boolean</span></span>|<span data-ttu-id="93eb9-265">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="93eb9-265">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="93eb9-266">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="93eb9-266">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="93eb9-267">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="93eb9-267">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="93eb9-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-268">Boolean</span></span>|<span data-ttu-id="93eb9-269">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="93eb9-269">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="93eb9-270">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="93eb9-270">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="93eb9-271">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="93eb9-271">windowsStoreBlocked</span></span>|<span data-ttu-id="93eb9-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="93eb9-272">Boolean</span></span>|<span data-ttu-id="93eb9-273">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="93eb9-273">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="93eb9-274">响应</span><span class="sxs-lookup"><span data-stu-id="93eb9-274">Response</span></span>
<span data-ttu-id="93eb9-275">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93eb9-275">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93eb9-276">示例</span><span class="sxs-lookup"><span data-stu-id="93eb9-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="93eb9-277">请求</span><span class="sxs-lookup"><span data-stu-id="93eb9-277">Request</span></span>
<span data-ttu-id="93eb9-278">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93eb9-278">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2326

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="93eb9-279">响应</span><span class="sxs-lookup"><span data-stu-id="93eb9-279">Response</span></span>
<span data-ttu-id="93eb9-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93eb9-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2498

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





