---
title: 更新 windowsPhone81GeneralConfiguration
description: 更新 windowsPhone81GeneralConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 041b94000581af0145daadd58abff760a3f14366
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693421"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="f4978-103">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4978-103">Update windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="f4978-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4978-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4978-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4978-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4978-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4978-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4978-107">更新 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4978-107">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4978-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4978-108">Prerequisites</span></span>
<span data-ttu-id="f4978-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4978-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4978-111">Permission type</span></span>|<span data-ttu-id="f4978-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4978-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4978-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4978-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4978-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4978-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4978-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4978-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4978-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4978-116">Not supported.</span></span>|
|<span data-ttu-id="f4978-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4978-117">Application</span></span>|<span data-ttu-id="f4978-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4978-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4978-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4978-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4978-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4978-120">Request headers</span></span>
|<span data-ttu-id="f4978-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4978-121">Header</span></span>|<span data-ttu-id="f4978-122">值</span><span class="sxs-lookup"><span data-stu-id="f4978-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4978-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4978-123">Authorization</span></span>|<span data-ttu-id="f4978-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4978-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4978-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4978-125">Accept</span></span>|<span data-ttu-id="f4978-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4978-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4978-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4978-127">Request body</span></span>
<span data-ttu-id="f4978-128">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4978-128">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="f4978-129">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4978-129">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="f4978-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4978-130">Property</span></span>|<span data-ttu-id="f4978-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4978-131">Type</span></span>|<span data-ttu-id="f4978-132">说明</span><span class="sxs-lookup"><span data-stu-id="f4978-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4978-133">id</span><span class="sxs-lookup"><span data-stu-id="f4978-133">id</span></span>|<span data-ttu-id="f4978-134">String</span><span class="sxs-lookup"><span data-stu-id="f4978-134">String</span></span>|<span data-ttu-id="f4978-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4978-135">Key of the entity.</span></span> <span data-ttu-id="f4978-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4978-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4978-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4978-138">DateTimeOffset</span></span>|<span data-ttu-id="f4978-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4978-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4978-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4978-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4978-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f4978-142">String collection</span></span>|<span data-ttu-id="f4978-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f4978-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4978-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4978-145">supportsScopeTags</span></span>|<span data-ttu-id="f4978-146">布尔</span><span class="sxs-lookup"><span data-stu-id="f4978-146">Boolean</span></span>|<span data-ttu-id="f4978-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f4978-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4978-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f4978-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4978-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f4978-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4978-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f4978-150">This property is read-only.</span></span> <span data-ttu-id="f4978-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f4978-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f4978-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f4978-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f4978-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f4978-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f4978-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f4978-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f4978-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f4978-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f4978-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f4978-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f4978-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f4978-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f4978-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f4978-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f4978-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f4978-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f4978-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4978-164">createdDateTime</span></span>|<span data-ttu-id="f4978-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4978-165">DateTimeOffset</span></span>|<span data-ttu-id="f4978-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4978-166">DateTime the object was created.</span></span> <span data-ttu-id="f4978-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-168">说明</span><span class="sxs-lookup"><span data-stu-id="f4978-168">description</span></span>|<span data-ttu-id="f4978-169">String</span><span class="sxs-lookup"><span data-stu-id="f4978-169">String</span></span>|<span data-ttu-id="f4978-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f4978-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4978-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f4978-172">displayName</span></span>|<span data-ttu-id="f4978-173">String</span><span class="sxs-lookup"><span data-stu-id="f4978-173">String</span></span>|<span data-ttu-id="f4978-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f4978-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4978-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-176">version</span><span class="sxs-lookup"><span data-stu-id="f4978-176">version</span></span>|<span data-ttu-id="f4978-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-177">Int32</span></span>|<span data-ttu-id="f4978-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f4978-178">Version of the device configuration.</span></span> <span data-ttu-id="f4978-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4978-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4978-180">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="f4978-180">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="f4978-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-181">Boolean</span></span>|<span data-ttu-id="f4978-182">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="f4978-182">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="f4978-183">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f4978-183">This property is read-only.</span></span>|
|<span data-ttu-id="f4978-184">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="f4978-184">appsBlockCopyPaste</span></span>|<span data-ttu-id="f4978-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-185">Boolean</span></span>|<span data-ttu-id="f4978-186">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="f4978-186">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="f4978-187">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-187">bluetoothBlocked</span></span>|<span data-ttu-id="f4978-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-188">Boolean</span></span>|<span data-ttu-id="f4978-189">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="f4978-189">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="f4978-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-190">cameraBlocked</span></span>|<span data-ttu-id="f4978-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-191">Boolean</span></span>|<span data-ttu-id="f4978-192">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="f4978-192">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="f4978-193">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="f4978-193">cellularBlockWifiTethering</span></span>|<span data-ttu-id="f4978-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-194">Boolean</span></span>|<span data-ttu-id="f4978-195">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="f4978-195">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="f4978-196">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="f4978-196">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f4978-197">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f4978-197">compliantAppsList</span></span>|<span data-ttu-id="f4978-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4978-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f4978-199">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="f4978-199">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f4978-200">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f4978-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f4978-201">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f4978-201">compliantAppListType</span></span>|[<span data-ttu-id="f4978-202">appListType</span><span class="sxs-lookup"><span data-stu-id="f4978-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f4978-203">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="f4978-203">List that is in the AppComplianceList.</span></span> <span data-ttu-id="f4978-204">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="f4978-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f4978-205">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="f4978-205">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="f4978-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-206">Boolean</span></span>|<span data-ttu-id="f4978-207">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="f4978-207">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f4978-208">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="f4978-208">emailBlockAddingAccounts</span></span>|<span data-ttu-id="f4978-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-209">Boolean</span></span>|<span data-ttu-id="f4978-210">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="f4978-210">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="f4978-211">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-211">locationServicesBlocked</span></span>|<span data-ttu-id="f4978-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-212">Boolean</span></span>|<span data-ttu-id="f4978-213">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="f4978-213">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="f4978-214">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-214">microsoftAccountBlocked</span></span>|<span data-ttu-id="f4978-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-215">Boolean</span></span>|<span data-ttu-id="f4978-216">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="f4978-216">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="f4978-217">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-217">nfcBlocked</span></span>|<span data-ttu-id="f4978-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-218">Boolean</span></span>|<span data-ttu-id="f4978-219">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="f4978-219">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="f4978-220">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f4978-220">passwordBlockSimple</span></span>|<span data-ttu-id="f4978-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-221">Boolean</span></span>|<span data-ttu-id="f4978-222">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="f4978-222">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f4978-223">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f4978-223">passwordExpirationDays</span></span>|<span data-ttu-id="f4978-224">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-224">Int32</span></span>|<span data-ttu-id="f4978-225">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="f4978-225">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f4978-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f4978-226">passwordMinimumLength</span></span>|<span data-ttu-id="f4978-227">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-227">Int32</span></span>|<span data-ttu-id="f4978-228">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="f4978-228">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f4978-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f4978-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f4978-230">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-230">Int32</span></span>|<span data-ttu-id="f4978-231">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="f4978-231">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="f4978-232">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f4978-232">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f4978-233">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-233">Int32</span></span>|<span data-ttu-id="f4978-234">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f4978-234">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="f4978-235">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f4978-235">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f4978-236">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-236">Int32</span></span>|<span data-ttu-id="f4978-237">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f4978-237">Number of previous passwords to block.</span></span> <span data-ttu-id="f4978-238">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="f4978-238">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f4978-239">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f4978-239">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f4978-240">Int32</span><span class="sxs-lookup"><span data-stu-id="f4978-240">Int32</span></span>|<span data-ttu-id="f4978-241">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="f4978-241">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="f4978-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f4978-242">passwordRequiredType</span></span>|[<span data-ttu-id="f4978-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f4978-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f4978-244">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f4978-244">Password type that is required.</span></span> <span data-ttu-id="f4978-245">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f4978-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f4978-246">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f4978-246">passwordRequired</span></span>|<span data-ttu-id="f4978-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-247">Boolean</span></span>|<span data-ttu-id="f4978-248">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="f4978-248">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="f4978-249">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-249">screenCaptureBlocked</span></span>|<span data-ttu-id="f4978-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-250">Boolean</span></span>|<span data-ttu-id="f4978-251">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="f4978-251">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="f4978-252">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="f4978-252">storageBlockRemovableStorage</span></span>|<span data-ttu-id="f4978-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-253">Boolean</span></span>|<span data-ttu-id="f4978-254">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="f4978-254">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="f4978-255">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f4978-255">storageRequireEncryption</span></span>|<span data-ttu-id="f4978-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-256">Boolean</span></span>|<span data-ttu-id="f4978-257">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="f4978-257">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="f4978-258">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-258">webBrowserBlocked</span></span>|<span data-ttu-id="f4978-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-259">Boolean</span></span>|<span data-ttu-id="f4978-260">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="f4978-260">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="f4978-261">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-261">wifiBlocked</span></span>|<span data-ttu-id="f4978-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-262">Boolean</span></span>|<span data-ttu-id="f4978-263">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="f4978-263">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="f4978-264">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="f4978-264">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="f4978-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-265">Boolean</span></span>|<span data-ttu-id="f4978-266">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="f4978-266">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="f4978-267">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="f4978-267">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f4978-268">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="f4978-268">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="f4978-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-269">Boolean</span></span>|<span data-ttu-id="f4978-270">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="f4978-270">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="f4978-271">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="f4978-271">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f4978-272">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f4978-272">windowsStoreBlocked</span></span>|<span data-ttu-id="f4978-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4978-273">Boolean</span></span>|<span data-ttu-id="f4978-274">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="f4978-274">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="f4978-275">响应</span><span class="sxs-lookup"><span data-stu-id="f4978-275">Response</span></span>
<span data-ttu-id="f4978-276">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4978-276">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4978-277">示例</span><span class="sxs-lookup"><span data-stu-id="f4978-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4978-278">请求</span><span class="sxs-lookup"><span data-stu-id="f4978-278">Request</span></span>
<span data-ttu-id="f4978-279">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4978-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4978-280">响应</span><span class="sxs-lookup"><span data-stu-id="f4978-280">Response</span></span>
<span data-ttu-id="f4978-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4978-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





