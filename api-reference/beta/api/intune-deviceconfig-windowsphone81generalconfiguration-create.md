---
title: 创建 windowsPhone81GeneralConfiguration
description: 创建新的 windowsPhone81GeneralConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: add0d2495f9b702baa6c8e9fff90844a184e0e22
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917777"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="df87c-103">创建 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="df87c-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="df87c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df87c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df87c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df87c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df87c-106">创建新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df87c-106">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df87c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="df87c-107">Prerequisites</span></span>
<span data-ttu-id="df87c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df87c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="df87c-110">Permission type</span></span>|<span data-ttu-id="df87c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df87c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df87c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df87c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df87c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df87c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df87c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df87c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df87c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="df87c-115">Not supported.</span></span>|
|<span data-ttu-id="df87c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="df87c-116">Application</span></span>|<span data-ttu-id="df87c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="df87c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df87c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df87c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="df87c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="df87c-119">Request headers</span></span>
|<span data-ttu-id="df87c-120">标头</span><span class="sxs-lookup"><span data-stu-id="df87c-120">Header</span></span>|<span data-ttu-id="df87c-121">值</span><span class="sxs-lookup"><span data-stu-id="df87c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df87c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df87c-122">Authorization</span></span>|<span data-ttu-id="df87c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df87c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df87c-124">接受</span><span class="sxs-lookup"><span data-stu-id="df87c-124">Accept</span></span>|<span data-ttu-id="df87c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df87c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df87c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="df87c-126">Request body</span></span>
<span data-ttu-id="df87c-127">在请求正文中，提供 windowsPhone81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df87c-127">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="df87c-128">下表显示了创建 windowsPhone81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df87c-128">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="df87c-129">属性</span><span class="sxs-lookup"><span data-stu-id="df87c-129">Property</span></span>|<span data-ttu-id="df87c-130">类型</span><span class="sxs-lookup"><span data-stu-id="df87c-130">Type</span></span>|<span data-ttu-id="df87c-131">说明</span><span class="sxs-lookup"><span data-stu-id="df87c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df87c-132">id</span><span class="sxs-lookup"><span data-stu-id="df87c-132">id</span></span>|<span data-ttu-id="df87c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="df87c-133">String</span></span>|<span data-ttu-id="df87c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df87c-134">Key of the entity.</span></span> <span data-ttu-id="df87c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df87c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="df87c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df87c-137">DateTimeOffset</span></span>|<span data-ttu-id="df87c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df87c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="df87c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df87c-140">roleScopeTagIds</span></span>|<span data-ttu-id="df87c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="df87c-141">String collection</span></span>|<span data-ttu-id="df87c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="df87c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df87c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="df87c-144">supportsScopeTags</span></span>|<span data-ttu-id="df87c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-145">Boolean</span></span>|<span data-ttu-id="df87c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="df87c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="df87c-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="df87c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="df87c-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="df87c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="df87c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="df87c-149">This property is read-only.</span></span> <span data-ttu-id="df87c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df87c-151">createdDateTime</span></span>|<span data-ttu-id="df87c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df87c-152">DateTimeOffset</span></span>|<span data-ttu-id="df87c-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df87c-153">DateTime the object was created.</span></span> <span data-ttu-id="df87c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-155">说明</span><span class="sxs-lookup"><span data-stu-id="df87c-155">description</span></span>|<span data-ttu-id="df87c-156">String</span><span class="sxs-lookup"><span data-stu-id="df87c-156">String</span></span>|<span data-ttu-id="df87c-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="df87c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df87c-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="df87c-159">displayName</span></span>|<span data-ttu-id="df87c-160">String</span><span class="sxs-lookup"><span data-stu-id="df87c-160">String</span></span>|<span data-ttu-id="df87c-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="df87c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df87c-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-163">version</span><span class="sxs-lookup"><span data-stu-id="df87c-163">version</span></span>|<span data-ttu-id="df87c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-164">Int32</span></span>|<span data-ttu-id="df87c-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="df87c-165">Version of the device configuration.</span></span> <span data-ttu-id="df87c-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df87c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df87c-167">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="df87c-167">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="df87c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-168">Boolean</span></span>|<span data-ttu-id="df87c-169">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="df87c-169">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="df87c-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="df87c-170">This property is read-only.</span></span>|
|<span data-ttu-id="df87c-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="df87c-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="df87c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-172">Boolean</span></span>|<span data-ttu-id="df87c-173">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="df87c-173">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="df87c-174">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-174">bluetoothBlocked</span></span>|<span data-ttu-id="df87c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-175">Boolean</span></span>|<span data-ttu-id="df87c-176">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="df87c-176">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="df87c-177">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-177">cameraBlocked</span></span>|<span data-ttu-id="df87c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-178">Boolean</span></span>|<span data-ttu-id="df87c-179">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="df87c-179">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="df87c-180">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="df87c-180">cellularBlockWifiTethering</span></span>|<span data-ttu-id="df87c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-181">Boolean</span></span>|<span data-ttu-id="df87c-182">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="df87c-182">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="df87c-183">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="df87c-183">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="df87c-184">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="df87c-184">compliantAppsList</span></span>|<span data-ttu-id="df87c-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df87c-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="df87c-186">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="df87c-186">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="df87c-187">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="df87c-187">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="df87c-188">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="df87c-188">compliantAppListType</span></span>|[<span data-ttu-id="df87c-189">appListType</span><span class="sxs-lookup"><span data-stu-id="df87c-189">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="df87c-190">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="df87c-190">List that is in the AppComplianceList.</span></span> <span data-ttu-id="df87c-191">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="df87c-191">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="df87c-192">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="df87c-192">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="df87c-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-193">Boolean</span></span>|<span data-ttu-id="df87c-194">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="df87c-194">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="df87c-195">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="df87c-195">emailBlockAddingAccounts</span></span>|<span data-ttu-id="df87c-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-196">Boolean</span></span>|<span data-ttu-id="df87c-197">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="df87c-197">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="df87c-198">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-198">locationServicesBlocked</span></span>|<span data-ttu-id="df87c-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-199">Boolean</span></span>|<span data-ttu-id="df87c-200">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="df87c-200">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="df87c-201">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-201">microsoftAccountBlocked</span></span>|<span data-ttu-id="df87c-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-202">Boolean</span></span>|<span data-ttu-id="df87c-203">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="df87c-203">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="df87c-204">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-204">nfcBlocked</span></span>|<span data-ttu-id="df87c-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-205">Boolean</span></span>|<span data-ttu-id="df87c-206">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="df87c-206">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="df87c-207">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="df87c-207">passwordBlockSimple</span></span>|<span data-ttu-id="df87c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-208">Boolean</span></span>|<span data-ttu-id="df87c-209">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="df87c-209">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="df87c-210">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="df87c-210">passwordExpirationDays</span></span>|<span data-ttu-id="df87c-211">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-211">Int32</span></span>|<span data-ttu-id="df87c-212">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="df87c-212">Number of days before the password expires.</span></span>|
|<span data-ttu-id="df87c-213">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="df87c-213">passwordMinimumLength</span></span>|<span data-ttu-id="df87c-214">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-214">Int32</span></span>|<span data-ttu-id="df87c-215">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="df87c-215">Minimum length of passwords.</span></span>|
|<span data-ttu-id="df87c-216">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="df87c-216">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="df87c-217">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-217">Int32</span></span>|<span data-ttu-id="df87c-218">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="df87c-218">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="df87c-219">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="df87c-219">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="df87c-220">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-220">Int32</span></span>|<span data-ttu-id="df87c-221">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="df87c-221">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="df87c-222">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="df87c-222">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="df87c-223">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-223">Int32</span></span>|<span data-ttu-id="df87c-224">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="df87c-224">Number of previous passwords to block.</span></span> <span data-ttu-id="df87c-225">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="df87c-225">Valid values 0 to 24</span></span>|
|<span data-ttu-id="df87c-226">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="df87c-226">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="df87c-227">Int32</span><span class="sxs-lookup"><span data-stu-id="df87c-227">Int32</span></span>|<span data-ttu-id="df87c-228">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="df87c-228">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="df87c-229">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="df87c-229">passwordRequiredType</span></span>|[<span data-ttu-id="df87c-230">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="df87c-230">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="df87c-231">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="df87c-231">Password type that is required.</span></span> <span data-ttu-id="df87c-232">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="df87c-232">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="df87c-233">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="df87c-233">passwordRequired</span></span>|<span data-ttu-id="df87c-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-234">Boolean</span></span>|<span data-ttu-id="df87c-235">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="df87c-235">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="df87c-236">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-236">screenCaptureBlocked</span></span>|<span data-ttu-id="df87c-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-237">Boolean</span></span>|<span data-ttu-id="df87c-238">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="df87c-238">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="df87c-239">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="df87c-239">storageBlockRemovableStorage</span></span>|<span data-ttu-id="df87c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-240">Boolean</span></span>|<span data-ttu-id="df87c-241">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="df87c-241">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="df87c-242">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="df87c-242">storageRequireEncryption</span></span>|<span data-ttu-id="df87c-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-243">Boolean</span></span>|<span data-ttu-id="df87c-244">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="df87c-244">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="df87c-245">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-245">webBrowserBlocked</span></span>|<span data-ttu-id="df87c-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-246">Boolean</span></span>|<span data-ttu-id="df87c-247">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="df87c-247">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="df87c-248">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-248">wifiBlocked</span></span>|<span data-ttu-id="df87c-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-249">Boolean</span></span>|<span data-ttu-id="df87c-250">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="df87c-250">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="df87c-251">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="df87c-251">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="df87c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-252">Boolean</span></span>|<span data-ttu-id="df87c-253">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="df87c-253">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="df87c-254">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="df87c-254">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="df87c-255">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="df87c-255">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="df87c-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-256">Boolean</span></span>|<span data-ttu-id="df87c-257">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="df87c-257">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="df87c-258">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="df87c-258">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="df87c-259">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="df87c-259">windowsStoreBlocked</span></span>|<span data-ttu-id="df87c-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="df87c-260">Boolean</span></span>|<span data-ttu-id="df87c-261">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="df87c-261">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="df87c-262">响应</span><span class="sxs-lookup"><span data-stu-id="df87c-262">Response</span></span>
<span data-ttu-id="df87c-263">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df87c-263">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df87c-264">示例</span><span class="sxs-lookup"><span data-stu-id="df87c-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="df87c-265">请求</span><span class="sxs-lookup"><span data-stu-id="df87c-265">Request</span></span>
<span data-ttu-id="df87c-266">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df87c-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="df87c-267">响应</span><span class="sxs-lookup"><span data-stu-id="df87c-267">Response</span></span>
<span data-ttu-id="df87c-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df87c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




