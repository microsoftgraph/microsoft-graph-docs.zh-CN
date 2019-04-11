---
title: 更新 windowsPhone81GeneralConfiguration
description: 更新 windowsPhone81GeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e8f0aa1c3ba924769bec41231019f76739b23be
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789673"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="5c3d6-103">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c3d6-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="5c3d6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c3d6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c3d6-106">更新 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c3d6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c3d6-107">Prerequisites</span></span>
<span data-ttu-id="5c3d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c3d6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c3d6-110">Permission type</span></span>|<span data-ttu-id="5c3d6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c3d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c3d6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c3d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c3d6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c3d6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c3d6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c3d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c3d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-115">Not supported.</span></span>|
|<span data-ttu-id="5c3d6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c3d6-116">Application</span></span>|<span data-ttu-id="5c3d6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c3d6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c3d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c3d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c3d6-119">Request headers</span></span>
|<span data-ttu-id="5c3d6-120">标头</span><span class="sxs-lookup"><span data-stu-id="5c3d6-120">Header</span></span>|<span data-ttu-id="5c3d6-121">值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c3d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c3d6-122">Authorization</span></span>|<span data-ttu-id="5c3d6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c3d6-124">接受</span><span class="sxs-lookup"><span data-stu-id="5c3d6-124">Accept</span></span>|<span data-ttu-id="5c3d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c3d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c3d6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c3d6-126">Request body</span></span>
<span data-ttu-id="5c3d6-127">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="5c3d6-128">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="5c3d6-129">属性</span><span class="sxs-lookup"><span data-stu-id="5c3d6-129">Property</span></span>|<span data-ttu-id="5c3d6-130">类型</span><span class="sxs-lookup"><span data-stu-id="5c3d6-130">Type</span></span>|<span data-ttu-id="5c3d6-131">说明</span><span class="sxs-lookup"><span data-stu-id="5c3d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c3d6-132">id</span><span class="sxs-lookup"><span data-stu-id="5c3d6-132">id</span></span>|<span data-ttu-id="5c3d6-133">String</span><span class="sxs-lookup"><span data-stu-id="5c3d6-133">String</span></span>|<span data-ttu-id="5c3d6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-134">Key of the entity.</span></span> <span data-ttu-id="5c3d6-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c3d6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c3d6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c3d6-137">DateTimeOffset</span></span>|<span data-ttu-id="5c3d6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c3d6-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c3d6-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c3d6-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="5c3d6-141">String collection</span></span>|<span data-ttu-id="5c3d6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c3d6-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5c3d6-144">supportsScopeTags</span></span>|<span data-ttu-id="5c3d6-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-145">Boolean</span></span>|<span data-ttu-id="5c3d6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c3d6-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c3d6-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c3d6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-149">This property is read-only.</span></span> <span data-ttu-id="5c3d6-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c3d6-151">createdDateTime</span></span>|<span data-ttu-id="5c3d6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c3d6-152">DateTimeOffset</span></span>|<span data-ttu-id="5c3d6-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-153">DateTime the object was created.</span></span> <span data-ttu-id="5c3d6-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-155">description</span><span class="sxs-lookup"><span data-stu-id="5c3d6-155">description</span></span>|<span data-ttu-id="5c3d6-156">String</span><span class="sxs-lookup"><span data-stu-id="5c3d6-156">String</span></span>|<span data-ttu-id="5c3d6-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c3d6-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5c3d6-159">displayName</span></span>|<span data-ttu-id="5c3d6-160">String</span><span class="sxs-lookup"><span data-stu-id="5c3d6-160">String</span></span>|<span data-ttu-id="5c3d6-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c3d6-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-163">version</span><span class="sxs-lookup"><span data-stu-id="5c3d6-163">version</span></span>|<span data-ttu-id="5c3d6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-164">Int32</span></span>|<span data-ttu-id="5c3d6-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-165">Version of the device configuration.</span></span> <span data-ttu-id="5c3d6-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c3d6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c3d6-167">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="5c3d6-167">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="5c3d6-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-168">Boolean</span></span>|<span data-ttu-id="5c3d6-169">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-169">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="5c3d6-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-170">This property is read-only.</span></span>|
|<span data-ttu-id="5c3d6-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="5c3d6-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="5c3d6-172">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-172">Boolean</span></span>|<span data-ttu-id="5c3d6-173">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-173">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="5c3d6-174">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-174">bluetoothBlocked</span></span>|<span data-ttu-id="5c3d6-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-175">Boolean</span></span>|<span data-ttu-id="5c3d6-176">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-176">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="5c3d6-177">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-177">cameraBlocked</span></span>|<span data-ttu-id="5c3d6-178">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-178">Boolean</span></span>|<span data-ttu-id="5c3d6-179">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-179">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="5c3d6-180">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="5c3d6-180">cellularBlockWifiTethering</span></span>|<span data-ttu-id="5c3d6-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-181">Boolean</span></span>|<span data-ttu-id="5c3d6-182">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-182">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="5c3d6-183">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-183">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="5c3d6-184">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="5c3d6-184">compliantAppsList</span></span>|<span data-ttu-id="5c3d6-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c3d6-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5c3d6-186">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-186">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="5c3d6-187">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-187">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="5c3d6-188">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="5c3d6-188">compliantAppListType</span></span>|[<span data-ttu-id="5c3d6-189">appListType</span><span class="sxs-lookup"><span data-stu-id="5c3d6-189">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="5c3d6-190">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-190">List that is in the AppComplianceList.</span></span> <span data-ttu-id="5c3d6-191">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-191">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="5c3d6-192">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="5c3d6-192">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="5c3d6-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-193">Boolean</span></span>|<span data-ttu-id="5c3d6-194">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-194">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="5c3d6-195">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="5c3d6-195">emailBlockAddingAccounts</span></span>|<span data-ttu-id="5c3d6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c3d6-196">Boolean</span></span>|<span data-ttu-id="5c3d6-197">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-197">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="5c3d6-198">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-198">locationServicesBlocked</span></span>|<span data-ttu-id="5c3d6-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-199">Boolean</span></span>|<span data-ttu-id="5c3d6-200">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-200">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="5c3d6-201">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-201">microsoftAccountBlocked</span></span>|<span data-ttu-id="5c3d6-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-202">Boolean</span></span>|<span data-ttu-id="5c3d6-203">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-203">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="5c3d6-204">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-204">nfcBlocked</span></span>|<span data-ttu-id="5c3d6-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-205">Boolean</span></span>|<span data-ttu-id="5c3d6-206">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-206">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="5c3d6-207">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5c3d6-207">passwordBlockSimple</span></span>|<span data-ttu-id="5c3d6-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c3d6-208">Boolean</span></span>|<span data-ttu-id="5c3d6-209">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-209">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="5c3d6-210">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5c3d6-210">passwordExpirationDays</span></span>|<span data-ttu-id="5c3d6-211">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-211">Int32</span></span>|<span data-ttu-id="5c3d6-212">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-212">Number of days before the password expires.</span></span>|
|<span data-ttu-id="5c3d6-213">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5c3d6-213">passwordMinimumLength</span></span>|<span data-ttu-id="5c3d6-214">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-214">Int32</span></span>|<span data-ttu-id="5c3d6-215">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-215">Minimum length of passwords.</span></span>|
|<span data-ttu-id="5c3d6-216">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5c3d6-216">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5c3d6-217">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-217">Int32</span></span>|<span data-ttu-id="5c3d6-218">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-218">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="5c3d6-219">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5c3d6-219">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5c3d6-220">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-220">Int32</span></span>|<span data-ttu-id="5c3d6-221">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-221">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="5c3d6-222">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5c3d6-222">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5c3d6-223">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-223">Int32</span></span>|<span data-ttu-id="5c3d6-224">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-224">Number of previous passwords to block.</span></span> <span data-ttu-id="5c3d6-225">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="5c3d6-225">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5c3d6-226">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5c3d6-226">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5c3d6-227">Int32</span><span class="sxs-lookup"><span data-stu-id="5c3d6-227">Int32</span></span>|<span data-ttu-id="5c3d6-228">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-228">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="5c3d6-229">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5c3d6-229">passwordRequiredType</span></span>|[<span data-ttu-id="5c3d6-230">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5c3d6-230">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5c3d6-231">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-231">Password type that is required.</span></span> <span data-ttu-id="5c3d6-232">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-232">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5c3d6-233">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5c3d6-233">passwordRequired</span></span>|<span data-ttu-id="5c3d6-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-234">Boolean</span></span>|<span data-ttu-id="5c3d6-235">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-235">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="5c3d6-236">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-236">screenCaptureBlocked</span></span>|<span data-ttu-id="5c3d6-237">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-237">Boolean</span></span>|<span data-ttu-id="5c3d6-238">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-238">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="5c3d6-239">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="5c3d6-239">storageBlockRemovableStorage</span></span>|<span data-ttu-id="5c3d6-240">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-240">Boolean</span></span>|<span data-ttu-id="5c3d6-241">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-241">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="5c3d6-242">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5c3d6-242">storageRequireEncryption</span></span>|<span data-ttu-id="5c3d6-243">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-243">Boolean</span></span>|<span data-ttu-id="5c3d6-244">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-244">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="5c3d6-245">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-245">webBrowserBlocked</span></span>|<span data-ttu-id="5c3d6-246">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-246">Boolean</span></span>|<span data-ttu-id="5c3d6-247">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-247">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="5c3d6-248">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-248">wifiBlocked</span></span>|<span data-ttu-id="5c3d6-249">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-249">Boolean</span></span>|<span data-ttu-id="5c3d6-250">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-250">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="5c3d6-251">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="5c3d6-251">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="5c3d6-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c3d6-252">Boolean</span></span>|<span data-ttu-id="5c3d6-253">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-253">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="5c3d6-254">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-254">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="5c3d6-255">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="5c3d6-255">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="5c3d6-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c3d6-256">Boolean</span></span>|<span data-ttu-id="5c3d6-257">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-257">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="5c3d6-258">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-258">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="5c3d6-259">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="5c3d6-259">windowsStoreBlocked</span></span>|<span data-ttu-id="5c3d6-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c3d6-260">Boolean</span></span>|<span data-ttu-id="5c3d6-261">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-261">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="5c3d6-262">响应</span><span class="sxs-lookup"><span data-stu-id="5c3d6-262">Response</span></span>
<span data-ttu-id="5c3d6-263">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c3d6-264">示例</span><span class="sxs-lookup"><span data-stu-id="5c3d6-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c3d6-265">请求</span><span class="sxs-lookup"><span data-stu-id="5c3d6-265">Request</span></span>
<span data-ttu-id="5c3d6-266">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1553

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="5c3d6-267">响应</span><span class="sxs-lookup"><span data-stu-id="5c3d6-267">Response</span></span>
<span data-ttu-id="5c3d6-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c3d6-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





