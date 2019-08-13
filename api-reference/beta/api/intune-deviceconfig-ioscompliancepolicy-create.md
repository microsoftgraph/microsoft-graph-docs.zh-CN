---
title: 创建 iosCompliancePolicy
description: 创建新的 iosCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39190d143aaa3a2ae9185283518134c9136788cd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339692"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="09b12-103">创建 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="09b12-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="09b12-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09b12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09b12-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09b12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09b12-106">创建新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09b12-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09b12-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="09b12-107">Prerequisites</span></span>
<span data-ttu-id="09b12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09b12-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="09b12-110">Permission type</span></span>|<span data-ttu-id="09b12-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="09b12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09b12-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09b12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09b12-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09b12-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09b12-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09b12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09b12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="09b12-115">Not supported.</span></span>|
|<span data-ttu-id="09b12-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="09b12-116">Application</span></span>|<span data-ttu-id="09b12-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09b12-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09b12-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09b12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="09b12-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="09b12-119">Request headers</span></span>
|<span data-ttu-id="09b12-120">标头</span><span class="sxs-lookup"><span data-stu-id="09b12-120">Header</span></span>|<span data-ttu-id="09b12-121">值</span><span class="sxs-lookup"><span data-stu-id="09b12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09b12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09b12-122">Authorization</span></span>|<span data-ttu-id="09b12-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="09b12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09b12-124">接受</span><span class="sxs-lookup"><span data-stu-id="09b12-124">Accept</span></span>|<span data-ttu-id="09b12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09b12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09b12-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="09b12-126">Request body</span></span>
<span data-ttu-id="09b12-127">在请求正文中，提供 iosCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09b12-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="09b12-128">下表显示了创建 iosCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="09b12-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="09b12-129">属性</span><span class="sxs-lookup"><span data-stu-id="09b12-129">Property</span></span>|<span data-ttu-id="09b12-130">类型</span><span class="sxs-lookup"><span data-stu-id="09b12-130">Type</span></span>|<span data-ttu-id="09b12-131">说明</span><span class="sxs-lookup"><span data-stu-id="09b12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09b12-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09b12-132">roleScopeTagIds</span></span>|<span data-ttu-id="09b12-133">String collection</span><span class="sxs-lookup"><span data-stu-id="09b12-133">String collection</span></span>|<span data-ttu-id="09b12-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="09b12-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09b12-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-136">id</span><span class="sxs-lookup"><span data-stu-id="09b12-136">id</span></span>|<span data-ttu-id="09b12-137">字符串</span><span class="sxs-lookup"><span data-stu-id="09b12-137">String</span></span>|<span data-ttu-id="09b12-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="09b12-138">Key of the entity.</span></span> <span data-ttu-id="09b12-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09b12-140">createdDateTime</span></span>|<span data-ttu-id="09b12-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b12-141">DateTimeOffset</span></span>|<span data-ttu-id="09b12-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="09b12-142">DateTime the object was created.</span></span> <span data-ttu-id="09b12-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-144">说明</span><span class="sxs-lookup"><span data-stu-id="09b12-144">description</span></span>|<span data-ttu-id="09b12-145">String</span><span class="sxs-lookup"><span data-stu-id="09b12-145">String</span></span>|<span data-ttu-id="09b12-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="09b12-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09b12-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09b12-148">lastModifiedDateTime</span></span>|<span data-ttu-id="09b12-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b12-149">DateTimeOffset</span></span>|<span data-ttu-id="09b12-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="09b12-150">DateTime the object was last modified.</span></span> <span data-ttu-id="09b12-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-152">displayName</span><span class="sxs-lookup"><span data-stu-id="09b12-152">displayName</span></span>|<span data-ttu-id="09b12-153">字符串</span><span class="sxs-lookup"><span data-stu-id="09b12-153">String</span></span>|<span data-ttu-id="09b12-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="09b12-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09b12-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-156">version</span><span class="sxs-lookup"><span data-stu-id="09b12-156">version</span></span>|<span data-ttu-id="09b12-157">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-157">Int32</span></span>|<span data-ttu-id="09b12-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="09b12-158">Version of the device configuration.</span></span> <span data-ttu-id="09b12-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09b12-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09b12-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="09b12-160">passcodeBlockSimple</span></span>|<span data-ttu-id="09b12-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="09b12-161">Boolean</span></span>|<span data-ttu-id="09b12-162">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="09b12-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="09b12-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="09b12-163">passcodeExpirationDays</span></span>|<span data-ttu-id="09b12-164">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-164">Int32</span></span>|<span data-ttu-id="09b12-165">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="09b12-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="09b12-166">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="09b12-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="09b12-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="09b12-167">passcodeMinimumLength</span></span>|<span data-ttu-id="09b12-168">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-168">Int32</span></span>|<span data-ttu-id="09b12-169">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="09b12-169">Minimum length of passcode.</span></span> <span data-ttu-id="09b12-170">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="09b12-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="09b12-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="09b12-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="09b12-172">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-172">Int32</span></span>|<span data-ttu-id="09b12-173">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="09b12-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="09b12-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="09b12-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="09b12-175">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-175">Int32</span></span>|<span data-ttu-id="09b12-176">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="09b12-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="09b12-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="09b12-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="09b12-178">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-178">Int32</span></span>|<span data-ttu-id="09b12-179">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="09b12-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="09b12-180">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="09b12-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="09b12-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="09b12-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="09b12-182">Int32</span><span class="sxs-lookup"><span data-stu-id="09b12-182">Int32</span></span>|<span data-ttu-id="09b12-183">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="09b12-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="09b12-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="09b12-184">passcodeRequiredType</span></span>|[<span data-ttu-id="09b12-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="09b12-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="09b12-186">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="09b12-186">The required passcode type.</span></span> <span data-ttu-id="09b12-187">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="09b12-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="09b12-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="09b12-188">passcodeRequired</span></span>|<span data-ttu-id="09b12-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="09b12-189">Boolean</span></span>|<span data-ttu-id="09b12-190">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="09b12-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="09b12-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="09b12-191">osMinimumVersion</span></span>|<span data-ttu-id="09b12-192">String</span><span class="sxs-lookup"><span data-stu-id="09b12-192">String</span></span>|<span data-ttu-id="09b12-193">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="09b12-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="09b12-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="09b12-194">osMaximumVersion</span></span>|<span data-ttu-id="09b12-195">String</span><span class="sxs-lookup"><span data-stu-id="09b12-195">String</span></span>|<span data-ttu-id="09b12-196">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="09b12-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="09b12-197">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="09b12-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="09b12-198">String</span><span class="sxs-lookup"><span data-stu-id="09b12-198">String</span></span>|<span data-ttu-id="09b12-199">最低 IOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="09b12-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="09b12-200">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="09b12-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="09b12-201">String</span><span class="sxs-lookup"><span data-stu-id="09b12-201">String</span></span>|<span data-ttu-id="09b12-202">最大 IOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="09b12-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="09b12-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="09b12-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="09b12-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="09b12-204">Boolean</span></span>|<span data-ttu-id="09b12-205">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="09b12-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="09b12-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="09b12-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="09b12-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="09b12-207">Boolean</span></span>|<span data-ttu-id="09b12-208">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="09b12-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="09b12-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="09b12-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="09b12-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="09b12-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="09b12-211">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="09b12-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="09b12-212">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="09b12-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="09b12-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="09b12-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="09b12-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="09b12-214">Boolean</span></span>|<span data-ttu-id="09b12-215">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="09b12-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="09b12-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="09b12-216">restrictedApps</span></span>|<span data-ttu-id="09b12-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09b12-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="09b12-218">要求设备未安装指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="09b12-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="09b12-219">此集合最多可包含100个元素。</span><span class="sxs-lookup"><span data-stu-id="09b12-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="09b12-220">响应</span><span class="sxs-lookup"><span data-stu-id="09b12-220">Response</span></span>
<span data-ttu-id="09b12-221">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09b12-221">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09b12-222">示例</span><span class="sxs-lookup"><span data-stu-id="09b12-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="09b12-223">请求</span><span class="sxs-lookup"><span data-stu-id="09b12-223">Request</span></span>
<span data-ttu-id="09b12-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09b12-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09b12-225">响应</span><span class="sxs-lookup"><span data-stu-id="09b12-225">Response</span></span>
<span data-ttu-id="09b12-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09b12-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






