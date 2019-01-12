---
title: 更新 windowsPhone81GeneralConfiguration
description: 更新 windowsPhone81GeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f0776dd36301bdb35d73e7e0564d445217e93be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984533"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="aeacd-103">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="aeacd-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="aeacd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aeacd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeacd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aeacd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aeacd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aeacd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aeacd-107">更新 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aeacd-107">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aeacd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aeacd-108">Prerequisites</span></span>
<span data-ttu-id="aeacd-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="aeacd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeacd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aeacd-111">Permission type</span></span>|<span data-ttu-id="aeacd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aeacd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeacd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aeacd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aeacd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeacd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aeacd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aeacd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeacd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aeacd-116">Not supported.</span></span>|
|<span data-ttu-id="aeacd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aeacd-117">Application</span></span>|<span data-ttu-id="aeacd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aeacd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeacd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aeacd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aeacd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aeacd-120">Request headers</span></span>
|<span data-ttu-id="aeacd-121">标头</span><span class="sxs-lookup"><span data-stu-id="aeacd-121">Header</span></span>|<span data-ttu-id="aeacd-122">值</span><span class="sxs-lookup"><span data-stu-id="aeacd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeacd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeacd-123">Authorization</span></span>|<span data-ttu-id="aeacd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aeacd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aeacd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aeacd-125">Accept</span></span>|<span data-ttu-id="aeacd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aeacd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeacd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aeacd-127">Request body</span></span>
<span data-ttu-id="aeacd-128">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeacd-128">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="aeacd-129">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aeacd-129">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="aeacd-130">属性</span><span class="sxs-lookup"><span data-stu-id="aeacd-130">Property</span></span>|<span data-ttu-id="aeacd-131">类型</span><span class="sxs-lookup"><span data-stu-id="aeacd-131">Type</span></span>|<span data-ttu-id="aeacd-132">说明</span><span class="sxs-lookup"><span data-stu-id="aeacd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeacd-133">id</span><span class="sxs-lookup"><span data-stu-id="aeacd-133">id</span></span>|<span data-ttu-id="aeacd-134">String</span><span class="sxs-lookup"><span data-stu-id="aeacd-134">String</span></span>|<span data-ttu-id="aeacd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aeacd-135">Key of the entity.</span></span> <span data-ttu-id="aeacd-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aeacd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aeacd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeacd-138">DateTimeOffset</span></span>|<span data-ttu-id="aeacd-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aeacd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aeacd-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aeacd-141">roleScopeTagIds</span></span>|<span data-ttu-id="aeacd-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="aeacd-142">String collection</span></span>|<span data-ttu-id="aeacd-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="aeacd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aeacd-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aeacd-145">supportsScopeTags</span></span>|<span data-ttu-id="aeacd-146">布尔</span><span class="sxs-lookup"><span data-stu-id="aeacd-146">Boolean</span></span>|<span data-ttu-id="aeacd-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="aeacd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aeacd-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="aeacd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aeacd-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="aeacd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aeacd-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aeacd-150">This property is read-only.</span></span> <span data-ttu-id="aeacd-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aeacd-152">createdDateTime</span></span>|<span data-ttu-id="aeacd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeacd-153">DateTimeOffset</span></span>|<span data-ttu-id="aeacd-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aeacd-154">DateTime the object was created.</span></span> <span data-ttu-id="aeacd-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-156">description</span><span class="sxs-lookup"><span data-stu-id="aeacd-156">description</span></span>|<span data-ttu-id="aeacd-157">String</span><span class="sxs-lookup"><span data-stu-id="aeacd-157">String</span></span>|<span data-ttu-id="aeacd-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="aeacd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aeacd-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="aeacd-160">displayName</span></span>|<span data-ttu-id="aeacd-161">String</span><span class="sxs-lookup"><span data-stu-id="aeacd-161">String</span></span>|<span data-ttu-id="aeacd-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="aeacd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aeacd-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-164">version</span><span class="sxs-lookup"><span data-stu-id="aeacd-164">version</span></span>|<span data-ttu-id="aeacd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-165">Int32</span></span>|<span data-ttu-id="aeacd-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="aeacd-166">Version of the device configuration.</span></span> <span data-ttu-id="aeacd-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aeacd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeacd-168">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="aeacd-168">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="aeacd-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-169">Boolean</span></span>|<span data-ttu-id="aeacd-170">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="aeacd-170">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="aeacd-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aeacd-171">This property is read-only.</span></span>|
|<span data-ttu-id="aeacd-172">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="aeacd-172">appsBlockCopyPaste</span></span>|<span data-ttu-id="aeacd-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-173">Boolean</span></span>|<span data-ttu-id="aeacd-174">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="aeacd-174">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="aeacd-175">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-175">bluetoothBlocked</span></span>|<span data-ttu-id="aeacd-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-176">Boolean</span></span>|<span data-ttu-id="aeacd-177">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="aeacd-177">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="aeacd-178">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-178">cameraBlocked</span></span>|<span data-ttu-id="aeacd-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-179">Boolean</span></span>|<span data-ttu-id="aeacd-180">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="aeacd-180">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="aeacd-181">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="aeacd-181">cellularBlockWifiTethering</span></span>|<span data-ttu-id="aeacd-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-182">Boolean</span></span>|<span data-ttu-id="aeacd-183">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="aeacd-183">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="aeacd-184">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="aeacd-184">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="aeacd-185">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="aeacd-185">compliantAppsList</span></span>|<span data-ttu-id="aeacd-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aeacd-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="aeacd-187">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="aeacd-187">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="aeacd-188">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="aeacd-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="aeacd-189">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="aeacd-189">compliantAppListType</span></span>|[<span data-ttu-id="aeacd-190">appListType</span><span class="sxs-lookup"><span data-stu-id="aeacd-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="aeacd-191">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="aeacd-191">List that is in the AppComplianceList.</span></span> <span data-ttu-id="aeacd-192">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="aeacd-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="aeacd-193">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="aeacd-193">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="aeacd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-194">Boolean</span></span>|<span data-ttu-id="aeacd-195">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="aeacd-195">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="aeacd-196">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="aeacd-196">emailBlockAddingAccounts</span></span>|<span data-ttu-id="aeacd-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-197">Boolean</span></span>|<span data-ttu-id="aeacd-198">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="aeacd-198">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="aeacd-199">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-199">locationServicesBlocked</span></span>|<span data-ttu-id="aeacd-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-200">Boolean</span></span>|<span data-ttu-id="aeacd-201">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="aeacd-201">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="aeacd-202">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-202">microsoftAccountBlocked</span></span>|<span data-ttu-id="aeacd-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-203">Boolean</span></span>|<span data-ttu-id="aeacd-204">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="aeacd-204">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="aeacd-205">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-205">nfcBlocked</span></span>|<span data-ttu-id="aeacd-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-206">Boolean</span></span>|<span data-ttu-id="aeacd-207">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="aeacd-207">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="aeacd-208">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="aeacd-208">passwordBlockSimple</span></span>|<span data-ttu-id="aeacd-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-209">Boolean</span></span>|<span data-ttu-id="aeacd-210">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="aeacd-210">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="aeacd-211">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aeacd-211">passwordExpirationDays</span></span>|<span data-ttu-id="aeacd-212">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-212">Int32</span></span>|<span data-ttu-id="aeacd-213">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="aeacd-213">Number of days before the password expires.</span></span>|
|<span data-ttu-id="aeacd-214">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aeacd-214">passwordMinimumLength</span></span>|<span data-ttu-id="aeacd-215">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-215">Int32</span></span>|<span data-ttu-id="aeacd-216">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="aeacd-216">Minimum length of passwords.</span></span>|
|<span data-ttu-id="aeacd-217">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="aeacd-217">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="aeacd-218">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-218">Int32</span></span>|<span data-ttu-id="aeacd-219">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="aeacd-219">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="aeacd-220">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="aeacd-220">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="aeacd-221">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-221">Int32</span></span>|<span data-ttu-id="aeacd-222">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="aeacd-222">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="aeacd-223">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aeacd-223">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aeacd-224">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-224">Int32</span></span>|<span data-ttu-id="aeacd-225">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="aeacd-225">Number of previous passwords to block.</span></span> <span data-ttu-id="aeacd-226">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="aeacd-226">Valid values 0 to 24</span></span>|
|<span data-ttu-id="aeacd-227">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="aeacd-227">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="aeacd-228">Int32</span><span class="sxs-lookup"><span data-stu-id="aeacd-228">Int32</span></span>|<span data-ttu-id="aeacd-229">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="aeacd-229">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="aeacd-230">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aeacd-230">passwordRequiredType</span></span>|[<span data-ttu-id="aeacd-231">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aeacd-231">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="aeacd-232">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="aeacd-232">Password type that is required.</span></span> <span data-ttu-id="aeacd-233">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="aeacd-233">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="aeacd-234">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aeacd-234">passwordRequired</span></span>|<span data-ttu-id="aeacd-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-235">Boolean</span></span>|<span data-ttu-id="aeacd-236">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="aeacd-236">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="aeacd-237">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-237">screenCaptureBlocked</span></span>|<span data-ttu-id="aeacd-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-238">Boolean</span></span>|<span data-ttu-id="aeacd-239">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="aeacd-239">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="aeacd-240">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="aeacd-240">storageBlockRemovableStorage</span></span>|<span data-ttu-id="aeacd-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-241">Boolean</span></span>|<span data-ttu-id="aeacd-242">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="aeacd-242">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="aeacd-243">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="aeacd-243">storageRequireEncryption</span></span>|<span data-ttu-id="aeacd-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-244">Boolean</span></span>|<span data-ttu-id="aeacd-245">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="aeacd-245">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="aeacd-246">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-246">webBrowserBlocked</span></span>|<span data-ttu-id="aeacd-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-247">Boolean</span></span>|<span data-ttu-id="aeacd-248">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="aeacd-248">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="aeacd-249">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-249">wifiBlocked</span></span>|<span data-ttu-id="aeacd-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-250">Boolean</span></span>|<span data-ttu-id="aeacd-251">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="aeacd-251">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="aeacd-252">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="aeacd-252">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="aeacd-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-253">Boolean</span></span>|<span data-ttu-id="aeacd-254">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="aeacd-254">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="aeacd-255">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="aeacd-255">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="aeacd-256">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="aeacd-256">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="aeacd-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-257">Boolean</span></span>|<span data-ttu-id="aeacd-258">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="aeacd-258">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="aeacd-259">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="aeacd-259">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="aeacd-260">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="aeacd-260">windowsStoreBlocked</span></span>|<span data-ttu-id="aeacd-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeacd-261">Boolean</span></span>|<span data-ttu-id="aeacd-262">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="aeacd-262">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="aeacd-263">响应</span><span class="sxs-lookup"><span data-stu-id="aeacd-263">Response</span></span>
<span data-ttu-id="aeacd-264">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aeacd-264">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeacd-265">示例</span><span class="sxs-lookup"><span data-stu-id="aeacd-265">Example</span></span>
### <a name="request"></a><span data-ttu-id="aeacd-266">请求</span><span class="sxs-lookup"><span data-stu-id="aeacd-266">Request</span></span>
<span data-ttu-id="aeacd-267">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aeacd-267">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1544

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="aeacd-268">响应</span><span class="sxs-lookup"><span data-stu-id="aeacd-268">Response</span></span>
<span data-ttu-id="aeacd-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aeacd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





