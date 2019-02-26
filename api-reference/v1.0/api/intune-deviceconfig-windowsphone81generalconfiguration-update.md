---
title: 更新 windowsPhone81GeneralConfiguration
description: 更新 windowsPhone81GeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49a200ef46b9f7f068d7100888daae576d7e8c9c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263929"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="c9cc0-103">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9cc0-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="c9cc0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9cc0-105">更新 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-105">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9cc0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9cc0-106">Prerequisites</span></span>
<span data-ttu-id="c9cc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9cc0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9cc0-109">Permission type</span></span>|<span data-ttu-id="c9cc0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9cc0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9cc0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9cc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9cc0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9cc0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9cc0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9cc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9cc0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-114">Not supported.</span></span>|
|<span data-ttu-id="c9cc0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9cc0-115">Application</span></span>|<span data-ttu-id="c9cc0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9cc0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9cc0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c9cc0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9cc0-118">Request headers</span></span>
|<span data-ttu-id="c9cc0-119">标头</span><span class="sxs-lookup"><span data-stu-id="c9cc0-119">Header</span></span>|<span data-ttu-id="c9cc0-120">值</span><span class="sxs-lookup"><span data-stu-id="c9cc0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9cc0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9cc0-121">Authorization</span></span>|<span data-ttu-id="c9cc0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9cc0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c9cc0-123">Accept</span></span>|<span data-ttu-id="c9cc0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c9cc0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9cc0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9cc0-125">Request body</span></span>
<span data-ttu-id="c9cc0-126">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-126">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="c9cc0-127">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-127">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="c9cc0-128">属性</span><span class="sxs-lookup"><span data-stu-id="c9cc0-128">Property</span></span>|<span data-ttu-id="c9cc0-129">类型</span><span class="sxs-lookup"><span data-stu-id="c9cc0-129">Type</span></span>|<span data-ttu-id="c9cc0-130">说明</span><span class="sxs-lookup"><span data-stu-id="c9cc0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9cc0-131">id</span><span class="sxs-lookup"><span data-stu-id="c9cc0-131">id</span></span>|<span data-ttu-id="c9cc0-132">String</span><span class="sxs-lookup"><span data-stu-id="c9cc0-132">String</span></span>|<span data-ttu-id="c9cc0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-133">Key of the entity.</span></span> <span data-ttu-id="c9cc0-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9cc0-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9cc0-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9cc0-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c9cc0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9cc0-136">DateTimeOffset</span></span>|<span data-ttu-id="c9cc0-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c9cc0-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9cc0-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9cc0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9cc0-139">createdDateTime</span></span>|<span data-ttu-id="c9cc0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9cc0-140">DateTimeOffset</span></span>|<span data-ttu-id="c9cc0-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-141">DateTime the object was created.</span></span> <span data-ttu-id="c9cc0-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9cc0-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9cc0-143">description</span><span class="sxs-lookup"><span data-stu-id="c9cc0-143">description</span></span>|<span data-ttu-id="c9cc0-144">String</span><span class="sxs-lookup"><span data-stu-id="c9cc0-144">String</span></span>|<span data-ttu-id="c9cc0-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9cc0-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9cc0-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9cc0-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c9cc0-147">displayName</span></span>|<span data-ttu-id="c9cc0-148">String</span><span class="sxs-lookup"><span data-stu-id="c9cc0-148">String</span></span>|<span data-ttu-id="c9cc0-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9cc0-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9cc0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9cc0-151">version</span><span class="sxs-lookup"><span data-stu-id="c9cc0-151">version</span></span>|<span data-ttu-id="c9cc0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-152">Int32</span></span>|<span data-ttu-id="c9cc0-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-153">Version of the device configuration.</span></span> <span data-ttu-id="c9cc0-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9cc0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9cc0-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="c9cc0-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="c9cc0-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-156">Boolean</span></span>|<span data-ttu-id="c9cc0-157">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="c9cc0-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-158">This property is read-only.</span></span>|
|<span data-ttu-id="c9cc0-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="c9cc0-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="c9cc0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-160">Boolean</span></span>|<span data-ttu-id="c9cc0-161">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="c9cc0-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-162">bluetoothBlocked</span></span>|<span data-ttu-id="c9cc0-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-163">Boolean</span></span>|<span data-ttu-id="c9cc0-164">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="c9cc0-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-165">cameraBlocked</span></span>|<span data-ttu-id="c9cc0-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-166">Boolean</span></span>|<span data-ttu-id="c9cc0-167">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="c9cc0-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="c9cc0-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="c9cc0-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-169">Boolean</span></span>|<span data-ttu-id="c9cc0-170">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="c9cc0-171">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="c9cc0-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c9cc0-172">compliantAppsList</span></span>|<span data-ttu-id="c9cc0-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9cc0-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c9cc0-174">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c9cc0-175">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c9cc0-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c9cc0-176">compliantAppListType</span></span>|[<span data-ttu-id="c9cc0-177">appListType</span><span class="sxs-lookup"><span data-stu-id="c9cc0-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c9cc0-178">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="c9cc0-179">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c9cc0-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c9cc0-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c9cc0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-181">Boolean</span></span>|<span data-ttu-id="c9cc0-182">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c9cc0-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="c9cc0-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="c9cc0-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-184">Boolean</span></span>|<span data-ttu-id="c9cc0-185">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="c9cc0-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-186">locationServicesBlocked</span></span>|<span data-ttu-id="c9cc0-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-187">Boolean</span></span>|<span data-ttu-id="c9cc0-188">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="c9cc0-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="c9cc0-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-190">Boolean</span></span>|<span data-ttu-id="c9cc0-191">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="c9cc0-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-192">nfcBlocked</span></span>|<span data-ttu-id="c9cc0-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-193">Boolean</span></span>|<span data-ttu-id="c9cc0-194">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="c9cc0-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c9cc0-195">passwordBlockSimple</span></span>|<span data-ttu-id="c9cc0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-196">Boolean</span></span>|<span data-ttu-id="c9cc0-197">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c9cc0-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c9cc0-198">passwordExpirationDays</span></span>|<span data-ttu-id="c9cc0-199">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-199">Int32</span></span>|<span data-ttu-id="c9cc0-200">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c9cc0-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c9cc0-201">passwordMinimumLength</span></span>|<span data-ttu-id="c9cc0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-202">Int32</span></span>|<span data-ttu-id="c9cc0-203">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c9cc0-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c9cc0-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c9cc0-205">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-205">Int32</span></span>|<span data-ttu-id="c9cc0-206">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="c9cc0-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c9cc0-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c9cc0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-208">Int32</span></span>|<span data-ttu-id="c9cc0-209">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="c9cc0-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c9cc0-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c9cc0-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-211">Int32</span></span>|<span data-ttu-id="c9cc0-212">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-212">Number of previous passwords to block.</span></span> <span data-ttu-id="c9cc0-213">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="c9cc0-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c9cc0-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c9cc0-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c9cc0-215">Int32</span><span class="sxs-lookup"><span data-stu-id="c9cc0-215">Int32</span></span>|<span data-ttu-id="c9cc0-216">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="c9cc0-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c9cc0-217">passwordRequiredType</span></span>|[<span data-ttu-id="c9cc0-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c9cc0-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c9cc0-219">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-219">Password type that is required.</span></span> <span data-ttu-id="c9cc0-220">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c9cc0-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c9cc0-221">passwordRequired</span></span>|<span data-ttu-id="c9cc0-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-222">Boolean</span></span>|<span data-ttu-id="c9cc0-223">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="c9cc0-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-224">screenCaptureBlocked</span></span>|<span data-ttu-id="c9cc0-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-225">Boolean</span></span>|<span data-ttu-id="c9cc0-226">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="c9cc0-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="c9cc0-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="c9cc0-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-228">Boolean</span></span>|<span data-ttu-id="c9cc0-229">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="c9cc0-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c9cc0-230">storageRequireEncryption</span></span>|<span data-ttu-id="c9cc0-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-231">Boolean</span></span>|<span data-ttu-id="c9cc0-232">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="c9cc0-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-233">webBrowserBlocked</span></span>|<span data-ttu-id="c9cc0-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-234">Boolean</span></span>|<span data-ttu-id="c9cc0-235">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="c9cc0-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-236">wifiBlocked</span></span>|<span data-ttu-id="c9cc0-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-237">Boolean</span></span>|<span data-ttu-id="c9cc0-238">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="c9cc0-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="c9cc0-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="c9cc0-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-240">Boolean</span></span>|<span data-ttu-id="c9cc0-241">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="c9cc0-242">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="c9cc0-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="c9cc0-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="c9cc0-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-244">Boolean</span></span>|<span data-ttu-id="c9cc0-245">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="c9cc0-246">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="c9cc0-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c9cc0-247">windowsStoreBlocked</span></span>|<span data-ttu-id="c9cc0-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9cc0-248">Boolean</span></span>|<span data-ttu-id="c9cc0-249">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="c9cc0-250">响应</span><span class="sxs-lookup"><span data-stu-id="c9cc0-250">Response</span></span>
<span data-ttu-id="c9cc0-251">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-251">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9cc0-252">示例</span><span class="sxs-lookup"><span data-stu-id="c9cc0-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9cc0-253">请求</span><span class="sxs-lookup"><span data-stu-id="c9cc0-253">Request</span></span>
<span data-ttu-id="c9cc0-254">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c9cc0-255">响应</span><span class="sxs-lookup"><span data-stu-id="c9cc0-255">Response</span></span>
<span data-ttu-id="c9cc0-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9cc0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



