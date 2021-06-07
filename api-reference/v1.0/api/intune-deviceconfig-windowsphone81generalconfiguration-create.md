---
title: 创建 windowsPhone81GeneralConfiguration
description: 创建新的 windowsPhone81GeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 267d3bbf4065e6e2f7c270efdab31cbe02f3d090
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760410"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="34a6b-103">创建 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="34a6b-103">Create windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="34a6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34a6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34a6b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34a6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a6b-106">创建新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34a6b-106">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34a6b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="34a6b-107">Prerequisites</span></span>
<span data-ttu-id="34a6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a6b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34a6b-110">Permission type</span></span>|<span data-ttu-id="34a6b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34a6b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34a6b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34a6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34a6b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a6b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34a6b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34a6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a6b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34a6b-115">Not supported.</span></span>|
|<span data-ttu-id="34a6b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="34a6b-116">Application</span></span>|<span data-ttu-id="34a6b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a6b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34a6b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34a6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34a6b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="34a6b-119">Request headers</span></span>
|<span data-ttu-id="34a6b-120">标头</span><span class="sxs-lookup"><span data-stu-id="34a6b-120">Header</span></span>|<span data-ttu-id="34a6b-121">值</span><span class="sxs-lookup"><span data-stu-id="34a6b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34a6b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a6b-122">Authorization</span></span>|<span data-ttu-id="34a6b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34a6b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34a6b-124">接受</span><span class="sxs-lookup"><span data-stu-id="34a6b-124">Accept</span></span>|<span data-ttu-id="34a6b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34a6b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a6b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="34a6b-126">Request body</span></span>
<span data-ttu-id="34a6b-127">在请求正文中，提供 windowsPhone81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34a6b-127">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="34a6b-128">下表显示了创建 windowsPhone81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="34a6b-128">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="34a6b-129">属性</span><span class="sxs-lookup"><span data-stu-id="34a6b-129">Property</span></span>|<span data-ttu-id="34a6b-130">类型</span><span class="sxs-lookup"><span data-stu-id="34a6b-130">Type</span></span>|<span data-ttu-id="34a6b-131">说明</span><span class="sxs-lookup"><span data-stu-id="34a6b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a6b-132">id</span><span class="sxs-lookup"><span data-stu-id="34a6b-132">id</span></span>|<span data-ttu-id="34a6b-133">String</span><span class="sxs-lookup"><span data-stu-id="34a6b-133">String</span></span>|<span data-ttu-id="34a6b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="34a6b-134">Key of the entity.</span></span> <span data-ttu-id="34a6b-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a6b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a6b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34a6b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="34a6b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a6b-137">DateTimeOffset</span></span>|<span data-ttu-id="34a6b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="34a6b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="34a6b-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a6b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a6b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34a6b-140">createdDateTime</span></span>|<span data-ttu-id="34a6b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a6b-141">DateTimeOffset</span></span>|<span data-ttu-id="34a6b-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="34a6b-142">DateTime the object was created.</span></span> <span data-ttu-id="34a6b-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a6b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a6b-144">description</span><span class="sxs-lookup"><span data-stu-id="34a6b-144">description</span></span>|<span data-ttu-id="34a6b-145">String</span><span class="sxs-lookup"><span data-stu-id="34a6b-145">String</span></span>|<span data-ttu-id="34a6b-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="34a6b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34a6b-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a6b-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a6b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="34a6b-148">displayName</span></span>|<span data-ttu-id="34a6b-149">String</span><span class="sxs-lookup"><span data-stu-id="34a6b-149">String</span></span>|<span data-ttu-id="34a6b-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="34a6b-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34a6b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a6b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a6b-152">version</span><span class="sxs-lookup"><span data-stu-id="34a6b-152">version</span></span>|<span data-ttu-id="34a6b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-153">Int32</span></span>|<span data-ttu-id="34a6b-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="34a6b-154">Version of the device configuration.</span></span> <span data-ttu-id="34a6b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a6b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a6b-156">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="34a6b-156">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="34a6b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-157">Boolean</span></span>|<span data-ttu-id="34a6b-158">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="34a6b-158">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="34a6b-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="34a6b-159">This property is read-only.</span></span>|
|<span data-ttu-id="34a6b-160">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="34a6b-160">appsBlockCopyPaste</span></span>|<span data-ttu-id="34a6b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-161">Boolean</span></span>|<span data-ttu-id="34a6b-162">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="34a6b-162">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="34a6b-163">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-163">bluetoothBlocked</span></span>|<span data-ttu-id="34a6b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-164">Boolean</span></span>|<span data-ttu-id="34a6b-165">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="34a6b-165">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="34a6b-166">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-166">cameraBlocked</span></span>|<span data-ttu-id="34a6b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-167">Boolean</span></span>|<span data-ttu-id="34a6b-168">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="34a6b-168">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="34a6b-169">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="34a6b-169">cellularBlockWifiTethering</span></span>|<span data-ttu-id="34a6b-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-170">Boolean</span></span>|<span data-ttu-id="34a6b-171">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="34a6b-171">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="34a6b-172">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="34a6b-172">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="34a6b-173">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="34a6b-173">compliantAppsList</span></span>|<span data-ttu-id="34a6b-174">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34a6b-174">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="34a6b-175">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="34a6b-175">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="34a6b-176">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="34a6b-176">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="34a6b-177">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="34a6b-177">compliantAppListType</span></span>|[<span data-ttu-id="34a6b-178">appListType</span><span class="sxs-lookup"><span data-stu-id="34a6b-178">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="34a6b-179">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="34a6b-179">List that is in the AppComplianceList.</span></span> <span data-ttu-id="34a6b-180">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="34a6b-180">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="34a6b-181">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="34a6b-181">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="34a6b-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-182">Boolean</span></span>|<span data-ttu-id="34a6b-183">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="34a6b-183">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="34a6b-184">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="34a6b-184">emailBlockAddingAccounts</span></span>|<span data-ttu-id="34a6b-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-185">Boolean</span></span>|<span data-ttu-id="34a6b-186">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="34a6b-186">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="34a6b-187">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-187">locationServicesBlocked</span></span>|<span data-ttu-id="34a6b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-188">Boolean</span></span>|<span data-ttu-id="34a6b-189">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="34a6b-189">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="34a6b-190">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-190">microsoftAccountBlocked</span></span>|<span data-ttu-id="34a6b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-191">Boolean</span></span>|<span data-ttu-id="34a6b-192">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="34a6b-192">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="34a6b-193">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-193">nfcBlocked</span></span>|<span data-ttu-id="34a6b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-194">Boolean</span></span>|<span data-ttu-id="34a6b-195">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="34a6b-195">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="34a6b-196">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="34a6b-196">passwordBlockSimple</span></span>|<span data-ttu-id="34a6b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-197">Boolean</span></span>|<span data-ttu-id="34a6b-198">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="34a6b-198">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="34a6b-199">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="34a6b-199">passwordExpirationDays</span></span>|<span data-ttu-id="34a6b-200">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-200">Int32</span></span>|<span data-ttu-id="34a6b-201">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="34a6b-201">Number of days before the password expires.</span></span>|
|<span data-ttu-id="34a6b-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="34a6b-202">passwordMinimumLength</span></span>|<span data-ttu-id="34a6b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-203">Int32</span></span>|<span data-ttu-id="34a6b-204">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="34a6b-204">Minimum length of passwords.</span></span>|
|<span data-ttu-id="34a6b-205">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="34a6b-205">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="34a6b-206">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-206">Int32</span></span>|<span data-ttu-id="34a6b-207">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="34a6b-207">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="34a6b-208">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="34a6b-208">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="34a6b-209">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-209">Int32</span></span>|<span data-ttu-id="34a6b-210">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="34a6b-210">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="34a6b-211">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="34a6b-211">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="34a6b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-212">Int32</span></span>|<span data-ttu-id="34a6b-213">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="34a6b-213">Number of previous passwords to block.</span></span> <span data-ttu-id="34a6b-214">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="34a6b-214">Valid values 0 to 24</span></span>|
|<span data-ttu-id="34a6b-215">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="34a6b-215">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="34a6b-216">Int32</span><span class="sxs-lookup"><span data-stu-id="34a6b-216">Int32</span></span>|<span data-ttu-id="34a6b-217">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="34a6b-217">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="34a6b-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="34a6b-218">passwordRequiredType</span></span>|[<span data-ttu-id="34a6b-219">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34a6b-219">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="34a6b-220">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="34a6b-220">Password type that is required.</span></span> <span data-ttu-id="34a6b-221">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="34a6b-221">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="34a6b-222">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="34a6b-222">passwordRequired</span></span>|<span data-ttu-id="34a6b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-223">Boolean</span></span>|<span data-ttu-id="34a6b-224">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="34a6b-224">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="34a6b-225">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-225">screenCaptureBlocked</span></span>|<span data-ttu-id="34a6b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-226">Boolean</span></span>|<span data-ttu-id="34a6b-227">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="34a6b-227">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="34a6b-228">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="34a6b-228">storageBlockRemovableStorage</span></span>|<span data-ttu-id="34a6b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-229">Boolean</span></span>|<span data-ttu-id="34a6b-230">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="34a6b-230">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="34a6b-231">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="34a6b-231">storageRequireEncryption</span></span>|<span data-ttu-id="34a6b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-232">Boolean</span></span>|<span data-ttu-id="34a6b-233">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="34a6b-233">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="34a6b-234">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-234">webBrowserBlocked</span></span>|<span data-ttu-id="34a6b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-235">Boolean</span></span>|<span data-ttu-id="34a6b-236">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="34a6b-236">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="34a6b-237">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-237">wifiBlocked</span></span>|<span data-ttu-id="34a6b-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-238">Boolean</span></span>|<span data-ttu-id="34a6b-239">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="34a6b-239">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="34a6b-240">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="34a6b-240">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="34a6b-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-241">Boolean</span></span>|<span data-ttu-id="34a6b-242">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="34a6b-242">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="34a6b-243">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="34a6b-243">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="34a6b-244">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="34a6b-244">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="34a6b-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-245">Boolean</span></span>|<span data-ttu-id="34a6b-246">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="34a6b-246">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="34a6b-247">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="34a6b-247">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="34a6b-248">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="34a6b-248">windowsStoreBlocked</span></span>|<span data-ttu-id="34a6b-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a6b-249">Boolean</span></span>|<span data-ttu-id="34a6b-250">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="34a6b-250">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="34a6b-251">响应</span><span class="sxs-lookup"><span data-stu-id="34a6b-251">Response</span></span>
<span data-ttu-id="34a6b-252">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34a6b-252">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a6b-253">示例</span><span class="sxs-lookup"><span data-stu-id="34a6b-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a6b-254">请求</span><span class="sxs-lookup"><span data-stu-id="34a6b-254">Request</span></span>
<span data-ttu-id="34a6b-255">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34a6b-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="34a6b-256">响应</span><span class="sxs-lookup"><span data-stu-id="34a6b-256">Response</span></span>
<span data-ttu-id="34a6b-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34a6b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




