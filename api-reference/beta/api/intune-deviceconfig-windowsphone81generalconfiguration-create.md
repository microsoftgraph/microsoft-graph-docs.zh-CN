---
title: 创建 windowsPhone81GeneralConfiguration
description: 创建新的 windowsPhone81GeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0722942abe17ff2789e7c4997c21ffaa71d8204c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43333636"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="4b3e0-103">创建 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b3e0-103">Create windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="4b3e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b3e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b3e0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b3e0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b3e0-107">创建新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-107">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b3e0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b3e0-108">Prerequisites</span></span>
<span data-ttu-id="4b3e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b3e0-111">Permission type</span></span>|<span data-ttu-id="4b3e0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b3e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b3e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b3e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b3e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b3e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b3e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b3e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b3e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-116">Not supported.</span></span>|
|<span data-ttu-id="4b3e0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b3e0-117">Application</span></span>|<span data-ttu-id="4b3e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b3e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b3e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b3e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b3e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b3e0-120">Request headers</span></span>
|<span data-ttu-id="4b3e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="4b3e0-121">Header</span></span>|<span data-ttu-id="4b3e0-122">值</span><span class="sxs-lookup"><span data-stu-id="4b3e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b3e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b3e0-123">Authorization</span></span>|<span data-ttu-id="4b3e0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b3e0-125">接受</span><span class="sxs-lookup"><span data-stu-id="4b3e0-125">Accept</span></span>|<span data-ttu-id="4b3e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b3e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b3e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b3e0-127">Request body</span></span>
<span data-ttu-id="4b3e0-128">在请求正文中，提供 windowsPhone81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-128">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="4b3e0-129">下表显示了创建 windowsPhone81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-129">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="4b3e0-130">属性</span><span class="sxs-lookup"><span data-stu-id="4b3e0-130">Property</span></span>|<span data-ttu-id="4b3e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="4b3e0-131">Type</span></span>|<span data-ttu-id="4b3e0-132">说明</span><span class="sxs-lookup"><span data-stu-id="4b3e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b3e0-133">id</span><span class="sxs-lookup"><span data-stu-id="4b3e0-133">id</span></span>|<span data-ttu-id="4b3e0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4b3e0-134">String</span></span>|<span data-ttu-id="4b3e0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-135">Key of the entity.</span></span> <span data-ttu-id="4b3e0-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b3e0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4b3e0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b3e0-138">DateTimeOffset</span></span>|<span data-ttu-id="4b3e0-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4b3e0-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b3e0-141">roleScopeTagIds</span></span>|<span data-ttu-id="4b3e0-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="4b3e0-142">String collection</span></span>|<span data-ttu-id="4b3e0-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b3e0-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4b3e0-145">supportsScopeTags</span></span>|<span data-ttu-id="4b3e0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-146">Boolean</span></span>|<span data-ttu-id="4b3e0-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b3e0-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b3e0-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b3e0-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-150">This property is read-only.</span></span> <span data-ttu-id="4b3e0-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b3e0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4b3e0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b3e0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4b3e0-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4b3e0-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b3e0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4b3e0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b3e0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4b3e0-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4b3e0-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b3e0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4b3e0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b3e0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4b3e0-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4b3e0-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b3e0-164">createdDateTime</span></span>|<span data-ttu-id="4b3e0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b3e0-165">DateTimeOffset</span></span>|<span data-ttu-id="4b3e0-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-166">DateTime the object was created.</span></span> <span data-ttu-id="4b3e0-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-168">description</span><span class="sxs-lookup"><span data-stu-id="4b3e0-168">description</span></span>|<span data-ttu-id="4b3e0-169">String</span><span class="sxs-lookup"><span data-stu-id="4b3e0-169">String</span></span>|<span data-ttu-id="4b3e0-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b3e0-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4b3e0-172">displayName</span></span>|<span data-ttu-id="4b3e0-173">String</span><span class="sxs-lookup"><span data-stu-id="4b3e0-173">String</span></span>|<span data-ttu-id="4b3e0-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b3e0-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-176">version</span><span class="sxs-lookup"><span data-stu-id="4b3e0-176">version</span></span>|<span data-ttu-id="4b3e0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-177">Int32</span></span>|<span data-ttu-id="4b3e0-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-178">Version of the device configuration.</span></span> <span data-ttu-id="4b3e0-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b3e0-180">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4b3e0-180">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4b3e0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-181">Boolean</span></span>|<span data-ttu-id="4b3e0-182">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-182">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4b3e0-183">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-183">This property is read-only.</span></span>|
|<span data-ttu-id="4b3e0-184">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4b3e0-184">appsBlockCopyPaste</span></span>|<span data-ttu-id="4b3e0-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-185">Boolean</span></span>|<span data-ttu-id="4b3e0-186">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-186">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4b3e0-187">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-187">bluetoothBlocked</span></span>|<span data-ttu-id="4b3e0-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-188">Boolean</span></span>|<span data-ttu-id="4b3e0-189">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-189">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4b3e0-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-190">cameraBlocked</span></span>|<span data-ttu-id="4b3e0-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-191">Boolean</span></span>|<span data-ttu-id="4b3e0-192">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-192">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4b3e0-193">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4b3e0-193">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4b3e0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-194">Boolean</span></span>|<span data-ttu-id="4b3e0-195">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-195">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4b3e0-196">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-196">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4b3e0-197">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4b3e0-197">compliantAppsList</span></span>|<span data-ttu-id="4b3e0-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b3e0-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4b3e0-199">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-199">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4b3e0-200">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4b3e0-201">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4b3e0-201">compliantAppListType</span></span>|[<span data-ttu-id="4b3e0-202">appListType</span><span class="sxs-lookup"><span data-stu-id="4b3e0-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4b3e0-203">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-203">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4b3e0-204">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4b3e0-205">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4b3e0-205">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4b3e0-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-206">Boolean</span></span>|<span data-ttu-id="4b3e0-207">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-207">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4b3e0-208">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4b3e0-208">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4b3e0-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-209">Boolean</span></span>|<span data-ttu-id="4b3e0-210">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-210">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4b3e0-211">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-211">locationServicesBlocked</span></span>|<span data-ttu-id="4b3e0-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-212">Boolean</span></span>|<span data-ttu-id="4b3e0-213">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-213">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4b3e0-214">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-214">microsoftAccountBlocked</span></span>|<span data-ttu-id="4b3e0-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-215">Boolean</span></span>|<span data-ttu-id="4b3e0-216">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-216">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4b3e0-217">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-217">nfcBlocked</span></span>|<span data-ttu-id="4b3e0-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-218">Boolean</span></span>|<span data-ttu-id="4b3e0-219">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-219">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4b3e0-220">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4b3e0-220">passwordBlockSimple</span></span>|<span data-ttu-id="4b3e0-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-221">Boolean</span></span>|<span data-ttu-id="4b3e0-222">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-222">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4b3e0-223">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4b3e0-223">passwordExpirationDays</span></span>|<span data-ttu-id="4b3e0-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-224">Int32</span></span>|<span data-ttu-id="4b3e0-225">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-225">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4b3e0-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4b3e0-226">passwordMinimumLength</span></span>|<span data-ttu-id="4b3e0-227">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-227">Int32</span></span>|<span data-ttu-id="4b3e0-228">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-228">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4b3e0-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4b3e0-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4b3e0-230">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-230">Int32</span></span>|<span data-ttu-id="4b3e0-231">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-231">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4b3e0-232">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4b3e0-232">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4b3e0-233">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-233">Int32</span></span>|<span data-ttu-id="4b3e0-234">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-234">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4b3e0-235">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4b3e0-235">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4b3e0-236">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-236">Int32</span></span>|<span data-ttu-id="4b3e0-237">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-237">Number of previous passwords to block.</span></span> <span data-ttu-id="4b3e0-238">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="4b3e0-238">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4b3e0-239">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4b3e0-239">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4b3e0-240">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3e0-240">Int32</span></span>|<span data-ttu-id="4b3e0-241">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-241">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4b3e0-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4b3e0-242">passwordRequiredType</span></span>|[<span data-ttu-id="4b3e0-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4b3e0-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4b3e0-244">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-244">Password type that is required.</span></span> <span data-ttu-id="4b3e0-245">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4b3e0-246">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4b3e0-246">passwordRequired</span></span>|<span data-ttu-id="4b3e0-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-247">Boolean</span></span>|<span data-ttu-id="4b3e0-248">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-248">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4b3e0-249">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-249">screenCaptureBlocked</span></span>|<span data-ttu-id="4b3e0-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-250">Boolean</span></span>|<span data-ttu-id="4b3e0-251">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-251">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4b3e0-252">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4b3e0-252">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4b3e0-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-253">Boolean</span></span>|<span data-ttu-id="4b3e0-254">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-254">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4b3e0-255">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4b3e0-255">storageRequireEncryption</span></span>|<span data-ttu-id="4b3e0-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-256">Boolean</span></span>|<span data-ttu-id="4b3e0-257">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-257">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4b3e0-258">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-258">webBrowserBlocked</span></span>|<span data-ttu-id="4b3e0-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-259">Boolean</span></span>|<span data-ttu-id="4b3e0-260">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-260">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4b3e0-261">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-261">wifiBlocked</span></span>|<span data-ttu-id="4b3e0-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-262">Boolean</span></span>|<span data-ttu-id="4b3e0-263">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-263">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4b3e0-264">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4b3e0-264">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4b3e0-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-265">Boolean</span></span>|<span data-ttu-id="4b3e0-266">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-266">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4b3e0-267">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-267">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4b3e0-268">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4b3e0-268">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4b3e0-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-269">Boolean</span></span>|<span data-ttu-id="4b3e0-270">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-270">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4b3e0-271">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-271">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4b3e0-272">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4b3e0-272">windowsStoreBlocked</span></span>|<span data-ttu-id="4b3e0-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b3e0-273">Boolean</span></span>|<span data-ttu-id="4b3e0-274">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-274">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4b3e0-275">响应</span><span class="sxs-lookup"><span data-stu-id="4b3e0-275">Response</span></span>
<span data-ttu-id="4b3e0-276">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-276">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b3e0-277">示例</span><span class="sxs-lookup"><span data-stu-id="4b3e0-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b3e0-278">请求</span><span class="sxs-lookup"><span data-stu-id="4b3e0-278">Request</span></span>
<span data-ttu-id="4b3e0-279">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-279">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4b3e0-280">响应</span><span class="sxs-lookup"><span data-stu-id="4b3e0-280">Response</span></span>
<span data-ttu-id="4b3e0-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b3e0-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



