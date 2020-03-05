---
title: 创建 iosCompliancePolicy
description: 创建新的 iosCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ce2abd418d96598f617897c112c36ac70093d3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449052"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="0157f-103">创建 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0157f-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="0157f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0157f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0157f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0157f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0157f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0157f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0157f-107">创建新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0157f-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0157f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0157f-108">Prerequisites</span></span>
<span data-ttu-id="0157f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0157f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0157f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0157f-111">Permission type</span></span>|<span data-ttu-id="0157f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0157f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0157f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0157f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0157f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0157f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0157f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0157f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0157f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0157f-116">Not supported.</span></span>|
|<span data-ttu-id="0157f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0157f-117">Application</span></span>|<span data-ttu-id="0157f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0157f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0157f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0157f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0157f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0157f-120">Request headers</span></span>
|<span data-ttu-id="0157f-121">标头</span><span class="sxs-lookup"><span data-stu-id="0157f-121">Header</span></span>|<span data-ttu-id="0157f-122">值</span><span class="sxs-lookup"><span data-stu-id="0157f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0157f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0157f-123">Authorization</span></span>|<span data-ttu-id="0157f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0157f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0157f-125">接受</span><span class="sxs-lookup"><span data-stu-id="0157f-125">Accept</span></span>|<span data-ttu-id="0157f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0157f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0157f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0157f-127">Request body</span></span>
<span data-ttu-id="0157f-128">在请求正文中，提供 iosCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0157f-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="0157f-129">下表显示了创建 iosCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0157f-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="0157f-130">属性</span><span class="sxs-lookup"><span data-stu-id="0157f-130">Property</span></span>|<span data-ttu-id="0157f-131">类型</span><span class="sxs-lookup"><span data-stu-id="0157f-131">Type</span></span>|<span data-ttu-id="0157f-132">说明</span><span class="sxs-lookup"><span data-stu-id="0157f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0157f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0157f-133">roleScopeTagIds</span></span>|<span data-ttu-id="0157f-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="0157f-134">String collection</span></span>|<span data-ttu-id="0157f-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0157f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0157f-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-137">id</span><span class="sxs-lookup"><span data-stu-id="0157f-137">id</span></span>|<span data-ttu-id="0157f-138">字符串</span><span class="sxs-lookup"><span data-stu-id="0157f-138">String</span></span>|<span data-ttu-id="0157f-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0157f-139">Key of the entity.</span></span> <span data-ttu-id="0157f-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0157f-141">createdDateTime</span></span>|<span data-ttu-id="0157f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0157f-142">DateTimeOffset</span></span>|<span data-ttu-id="0157f-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0157f-143">DateTime the object was created.</span></span> <span data-ttu-id="0157f-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-145">说明</span><span class="sxs-lookup"><span data-stu-id="0157f-145">description</span></span>|<span data-ttu-id="0157f-146">String</span><span class="sxs-lookup"><span data-stu-id="0157f-146">String</span></span>|<span data-ttu-id="0157f-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0157f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0157f-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0157f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="0157f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0157f-150">DateTimeOffset</span></span>|<span data-ttu-id="0157f-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0157f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="0157f-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0157f-153">displayName</span></span>|<span data-ttu-id="0157f-154">字符串</span><span class="sxs-lookup"><span data-stu-id="0157f-154">String</span></span>|<span data-ttu-id="0157f-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0157f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0157f-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-157">version</span><span class="sxs-lookup"><span data-stu-id="0157f-157">version</span></span>|<span data-ttu-id="0157f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-158">Int32</span></span>|<span data-ttu-id="0157f-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0157f-159">Version of the device configuration.</span></span> <span data-ttu-id="0157f-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0157f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0157f-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0157f-161">passcodeBlockSimple</span></span>|<span data-ttu-id="0157f-162">布尔</span><span class="sxs-lookup"><span data-stu-id="0157f-162">Boolean</span></span>|<span data-ttu-id="0157f-163">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="0157f-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="0157f-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0157f-164">passcodeExpirationDays</span></span>|<span data-ttu-id="0157f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-165">Int32</span></span>|<span data-ttu-id="0157f-166">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="0157f-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="0157f-167">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="0157f-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0157f-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0157f-168">passcodeMinimumLength</span></span>|<span data-ttu-id="0157f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-169">Int32</span></span>|<span data-ttu-id="0157f-170">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="0157f-170">Minimum length of passcode.</span></span> <span data-ttu-id="0157f-171">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="0157f-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0157f-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0157f-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0157f-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-173">Int32</span></span>|<span data-ttu-id="0157f-174">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="0157f-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="0157f-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0157f-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0157f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-176">Int32</span></span>|<span data-ttu-id="0157f-177">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="0157f-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="0157f-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="0157f-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="0157f-179">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-179">Int32</span></span>|<span data-ttu-id="0157f-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="0157f-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="0157f-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="0157f-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0157f-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0157f-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="0157f-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0157f-183">Int32</span></span>|<span data-ttu-id="0157f-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="0157f-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0157f-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="0157f-185">passcodeRequiredType</span></span>|[<span data-ttu-id="0157f-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0157f-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0157f-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="0157f-187">The required passcode type.</span></span> <span data-ttu-id="0157f-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="0157f-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0157f-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="0157f-189">passcodeRequired</span></span>|<span data-ttu-id="0157f-190">布尔</span><span class="sxs-lookup"><span data-stu-id="0157f-190">Boolean</span></span>|<span data-ttu-id="0157f-191">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="0157f-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="0157f-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0157f-192">osMinimumVersion</span></span>|<span data-ttu-id="0157f-193">String</span><span class="sxs-lookup"><span data-stu-id="0157f-193">String</span></span>|<span data-ttu-id="0157f-194">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="0157f-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="0157f-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0157f-195">osMaximumVersion</span></span>|<span data-ttu-id="0157f-196">String</span><span class="sxs-lookup"><span data-stu-id="0157f-196">String</span></span>|<span data-ttu-id="0157f-197">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="0157f-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="0157f-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0157f-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="0157f-199">String</span><span class="sxs-lookup"><span data-stu-id="0157f-199">String</span></span>|<span data-ttu-id="0157f-200">最低 IOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="0157f-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="0157f-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0157f-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="0157f-202">String</span><span class="sxs-lookup"><span data-stu-id="0157f-202">String</span></span>|<span data-ttu-id="0157f-203">最大 IOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="0157f-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="0157f-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="0157f-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="0157f-205">布尔</span><span class="sxs-lookup"><span data-stu-id="0157f-205">Boolean</span></span>|<span data-ttu-id="0157f-206">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="0157f-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="0157f-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0157f-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0157f-208">布尔</span><span class="sxs-lookup"><span data-stu-id="0157f-208">Boolean</span></span>|<span data-ttu-id="0157f-209">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="0157f-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="0157f-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0157f-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0157f-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0157f-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0157f-212">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="0157f-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0157f-213">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="0157f-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0157f-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="0157f-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="0157f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="0157f-215">Boolean</span></span>|<span data-ttu-id="0157f-216">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="0157f-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="0157f-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="0157f-217">restrictedApps</span></span>|<span data-ttu-id="0157f-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0157f-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0157f-219">要求设备未安装指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0157f-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="0157f-220">此集合最多可包含100个元素。</span><span class="sxs-lookup"><span data-stu-id="0157f-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0157f-221">响应</span><span class="sxs-lookup"><span data-stu-id="0157f-221">Response</span></span>
<span data-ttu-id="0157f-222">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0157f-222">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0157f-223">示例</span><span class="sxs-lookup"><span data-stu-id="0157f-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="0157f-224">请求</span><span class="sxs-lookup"><span data-stu-id="0157f-224">Request</span></span>
<span data-ttu-id="0157f-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0157f-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0157f-226">响应</span><span class="sxs-lookup"><span data-stu-id="0157f-226">Response</span></span>
<span data-ttu-id="0157f-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0157f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```





