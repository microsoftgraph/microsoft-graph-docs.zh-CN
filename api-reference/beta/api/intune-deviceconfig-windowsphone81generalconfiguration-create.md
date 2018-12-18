---
title: 创建 windowsPhone81GeneralConfiguration
description: 创建新的 windowsPhone81GeneralConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: bec529f093a1c732ab214e9324d224ab89497d06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349705"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="c9e30-103">创建 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9e30-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="c9e30-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9e30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9e30-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9e30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9e30-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9e30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9e30-107">创建新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9e30-107">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9e30-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9e30-108">Prerequisites</span></span>
<span data-ttu-id="c9e30-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c9e30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9e30-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9e30-111">Permission type</span></span>|<span data-ttu-id="c9e30-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9e30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9e30-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9e30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9e30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9e30-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9e30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9e30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9e30-116">Not supported.</span></span>|
|<span data-ttu-id="c9e30-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9e30-117">Application</span></span>|<span data-ttu-id="c9e30-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9e30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9e30-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9e30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c9e30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9e30-120">Request headers</span></span>
|<span data-ttu-id="c9e30-121">标头</span><span class="sxs-lookup"><span data-stu-id="c9e30-121">Header</span></span>|<span data-ttu-id="c9e30-122">值</span><span class="sxs-lookup"><span data-stu-id="c9e30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9e30-123">授权</span><span class="sxs-lookup"><span data-stu-id="c9e30-123">Authorization</span></span>|<span data-ttu-id="c9e30-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9e30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9e30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9e30-125">Accept</span></span>|<span data-ttu-id="c9e30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9e30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9e30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9e30-127">Request body</span></span>
<span data-ttu-id="c9e30-128">在请求正文中，提供 windowsPhone81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9e30-128">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="c9e30-129">下表显示了创建 windowsPhone81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9e30-129">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="c9e30-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9e30-130">Property</span></span>|<span data-ttu-id="c9e30-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9e30-131">Type</span></span>|<span data-ttu-id="c9e30-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9e30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9e30-133">id</span><span class="sxs-lookup"><span data-stu-id="c9e30-133">id</span></span>|<span data-ttu-id="c9e30-134">String</span><span class="sxs-lookup"><span data-stu-id="c9e30-134">String</span></span>|<span data-ttu-id="c9e30-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9e30-135">Key of the entity.</span></span> <span data-ttu-id="c9e30-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9e30-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c9e30-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9e30-138">DateTimeOffset</span></span>|<span data-ttu-id="c9e30-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9e30-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c9e30-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9e30-141">roleScopeTagIds</span></span>|<span data-ttu-id="c9e30-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="c9e30-142">String collection</span></span>|<span data-ttu-id="c9e30-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="c9e30-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9e30-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9e30-145">supportsScopeTags</span></span>|<span data-ttu-id="c9e30-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-146">Boolean</span></span>|<span data-ttu-id="c9e30-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="c9e30-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9e30-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c9e30-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9e30-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="c9e30-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9e30-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9e30-150">This property is read-only.</span></span> <span data-ttu-id="c9e30-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9e30-152">createdDateTime</span></span>|<span data-ttu-id="c9e30-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9e30-153">DateTimeOffset</span></span>|<span data-ttu-id="c9e30-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9e30-154">DateTime the object was created.</span></span> <span data-ttu-id="c9e30-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-156">description</span><span class="sxs-lookup"><span data-stu-id="c9e30-156">description</span></span>|<span data-ttu-id="c9e30-157">String</span><span class="sxs-lookup"><span data-stu-id="c9e30-157">String</span></span>|<span data-ttu-id="c9e30-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c9e30-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9e30-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c9e30-160">displayName</span></span>|<span data-ttu-id="c9e30-161">String</span><span class="sxs-lookup"><span data-stu-id="c9e30-161">String</span></span>|<span data-ttu-id="c9e30-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c9e30-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9e30-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-164">version</span><span class="sxs-lookup"><span data-stu-id="c9e30-164">version</span></span>|<span data-ttu-id="c9e30-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-165">Int32</span></span>|<span data-ttu-id="c9e30-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9e30-166">Version of the device configuration.</span></span> <span data-ttu-id="c9e30-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9e30-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9e30-168">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="c9e30-168">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="c9e30-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-169">Boolean</span></span>|<span data-ttu-id="c9e30-170">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="c9e30-170">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="c9e30-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9e30-171">This property is read-only.</span></span>|
|<span data-ttu-id="c9e30-172">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="c9e30-172">appsBlockCopyPaste</span></span>|<span data-ttu-id="c9e30-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-173">Boolean</span></span>|<span data-ttu-id="c9e30-174">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="c9e30-174">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="c9e30-175">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-175">bluetoothBlocked</span></span>|<span data-ttu-id="c9e30-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-176">Boolean</span></span>|<span data-ttu-id="c9e30-177">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="c9e30-177">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="c9e30-178">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-178">cameraBlocked</span></span>|<span data-ttu-id="c9e30-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-179">Boolean</span></span>|<span data-ttu-id="c9e30-180">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="c9e30-180">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="c9e30-181">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="c9e30-181">cellularBlockWifiTethering</span></span>|<span data-ttu-id="c9e30-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-182">Boolean</span></span>|<span data-ttu-id="c9e30-183">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="c9e30-183">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="c9e30-184">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="c9e30-184">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="c9e30-185">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c9e30-185">compliantAppsList</span></span>|<span data-ttu-id="c9e30-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9e30-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c9e30-187">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="c9e30-187">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c9e30-188">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c9e30-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c9e30-189">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c9e30-189">compliantAppListType</span></span>|[<span data-ttu-id="c9e30-190">appListType</span><span class="sxs-lookup"><span data-stu-id="c9e30-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c9e30-191">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="c9e30-191">List that is in the AppComplianceList.</span></span> <span data-ttu-id="c9e30-192">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="c9e30-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c9e30-193">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c9e30-193">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c9e30-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-194">Boolean</span></span>|<span data-ttu-id="c9e30-195">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="c9e30-195">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c9e30-196">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="c9e30-196">emailBlockAddingAccounts</span></span>|<span data-ttu-id="c9e30-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-197">Boolean</span></span>|<span data-ttu-id="c9e30-198">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="c9e30-198">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="c9e30-199">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-199">locationServicesBlocked</span></span>|<span data-ttu-id="c9e30-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-200">Boolean</span></span>|<span data-ttu-id="c9e30-201">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="c9e30-201">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="c9e30-202">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-202">microsoftAccountBlocked</span></span>|<span data-ttu-id="c9e30-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-203">Boolean</span></span>|<span data-ttu-id="c9e30-204">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="c9e30-204">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="c9e30-205">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-205">nfcBlocked</span></span>|<span data-ttu-id="c9e30-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-206">Boolean</span></span>|<span data-ttu-id="c9e30-207">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="c9e30-207">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="c9e30-208">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c9e30-208">passwordBlockSimple</span></span>|<span data-ttu-id="c9e30-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-209">Boolean</span></span>|<span data-ttu-id="c9e30-210">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="c9e30-210">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c9e30-211">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c9e30-211">passwordExpirationDays</span></span>|<span data-ttu-id="c9e30-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-212">Int32</span></span>|<span data-ttu-id="c9e30-213">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c9e30-213">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c9e30-214">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c9e30-214">passwordMinimumLength</span></span>|<span data-ttu-id="c9e30-215">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-215">Int32</span></span>|<span data-ttu-id="c9e30-216">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c9e30-216">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c9e30-217">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c9e30-217">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c9e30-218">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-218">Int32</span></span>|<span data-ttu-id="c9e30-219">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="c9e30-219">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="c9e30-220">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c9e30-220">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c9e30-221">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-221">Int32</span></span>|<span data-ttu-id="c9e30-222">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c9e30-222">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="c9e30-223">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c9e30-223">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c9e30-224">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-224">Int32</span></span>|<span data-ttu-id="c9e30-225">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c9e30-225">Number of previous passwords to block.</span></span> <span data-ttu-id="c9e30-226">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="c9e30-226">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c9e30-227">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c9e30-227">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c9e30-228">Int32</span><span class="sxs-lookup"><span data-stu-id="c9e30-228">Int32</span></span>|<span data-ttu-id="c9e30-229">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="c9e30-229">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="c9e30-230">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c9e30-230">passwordRequiredType</span></span>|[<span data-ttu-id="c9e30-231">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c9e30-231">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c9e30-232">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c9e30-232">Password type that is required.</span></span> <span data-ttu-id="c9e30-233">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c9e30-233">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c9e30-234">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c9e30-234">passwordRequired</span></span>|<span data-ttu-id="c9e30-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-235">Boolean</span></span>|<span data-ttu-id="c9e30-236">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c9e30-236">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="c9e30-237">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-237">screenCaptureBlocked</span></span>|<span data-ttu-id="c9e30-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-238">Boolean</span></span>|<span data-ttu-id="c9e30-239">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="c9e30-239">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="c9e30-240">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="c9e30-240">storageBlockRemovableStorage</span></span>|<span data-ttu-id="c9e30-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-241">Boolean</span></span>|<span data-ttu-id="c9e30-242">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="c9e30-242">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="c9e30-243">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c9e30-243">storageRequireEncryption</span></span>|<span data-ttu-id="c9e30-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-244">Boolean</span></span>|<span data-ttu-id="c9e30-245">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="c9e30-245">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="c9e30-246">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-246">webBrowserBlocked</span></span>|<span data-ttu-id="c9e30-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-247">Boolean</span></span>|<span data-ttu-id="c9e30-248">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="c9e30-248">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="c9e30-249">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-249">wifiBlocked</span></span>|<span data-ttu-id="c9e30-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-250">Boolean</span></span>|<span data-ttu-id="c9e30-251">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="c9e30-251">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="c9e30-252">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="c9e30-252">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="c9e30-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-253">Boolean</span></span>|<span data-ttu-id="c9e30-254">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="c9e30-254">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="c9e30-255">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="c9e30-255">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="c9e30-256">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="c9e30-256">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="c9e30-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-257">Boolean</span></span>|<span data-ttu-id="c9e30-258">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="c9e30-258">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="c9e30-259">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="c9e30-259">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="c9e30-260">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e30-260">windowsStoreBlocked</span></span>|<span data-ttu-id="c9e30-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9e30-261">Boolean</span></span>|<span data-ttu-id="c9e30-262">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="c9e30-262">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="c9e30-263">响应</span><span class="sxs-lookup"><span data-stu-id="c9e30-263">Response</span></span>
<span data-ttu-id="c9e30-264">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9e30-264">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9e30-265">示例</span><span class="sxs-lookup"><span data-stu-id="c9e30-265">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9e30-266">请求</span><span class="sxs-lookup"><span data-stu-id="c9e30-266">Request</span></span>
<span data-ttu-id="c9e30-267">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9e30-267">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1617

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="c9e30-268">响应</span><span class="sxs-lookup"><span data-stu-id="c9e30-268">Response</span></span>
<span data-ttu-id="c9e30-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9e30-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





