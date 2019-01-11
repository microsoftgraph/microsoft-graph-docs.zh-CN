---
title: 创建 iosCompliancePolicy
description: 创建新的 iosCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd5eca6a10492356f65449f2a1b98e6c79744b72
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873701"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="c6a9d-103">创建 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c6a9d-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="c6a9d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6a9d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6a9d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6a9d-107">创建新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6a9d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6a9d-108">Prerequisites</span></span>
<span data-ttu-id="c6a9d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c6a9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6a9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6a9d-111">Permission type</span></span>|<span data-ttu-id="c6a9d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6a9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6a9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6a9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6a9d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6a9d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6a9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6a9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6a9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-116">Not supported.</span></span>|
|<span data-ttu-id="c6a9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6a9d-117">Application</span></span>|<span data-ttu-id="c6a9d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6a9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6a9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c6a9d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6a9d-120">Request headers</span></span>
|<span data-ttu-id="c6a9d-121">标头</span><span class="sxs-lookup"><span data-stu-id="c6a9d-121">Header</span></span>|<span data-ttu-id="c6a9d-122">值</span><span class="sxs-lookup"><span data-stu-id="c6a9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6a9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6a9d-123">Authorization</span></span>|<span data-ttu-id="c6a9d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6a9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6a9d-125">Accept</span></span>|<span data-ttu-id="c6a9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6a9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6a9d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6a9d-127">Request body</span></span>
<span data-ttu-id="c6a9d-128">在请求正文中，提供 iosCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="c6a9d-129">下表显示了创建 iosCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="c6a9d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c6a9d-130">Property</span></span>|<span data-ttu-id="c6a9d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c6a9d-131">Type</span></span>|<span data-ttu-id="c6a9d-132">Description</span><span class="sxs-lookup"><span data-stu-id="c6a9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6a9d-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c6a9d-133">roleScopeTagIds</span></span>|<span data-ttu-id="c6a9d-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="c6a9d-134">String collection</span></span>|<span data-ttu-id="c6a9d-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c6a9d-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-137">id</span><span class="sxs-lookup"><span data-stu-id="c6a9d-137">id</span></span>|<span data-ttu-id="c6a9d-138">String</span><span class="sxs-lookup"><span data-stu-id="c6a9d-138">String</span></span>|<span data-ttu-id="c6a9d-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-139">Key of the entity.</span></span> <span data-ttu-id="c6a9d-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6a9d-141">createdDateTime</span></span>|<span data-ttu-id="c6a9d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6a9d-142">DateTimeOffset</span></span>|<span data-ttu-id="c6a9d-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-143">DateTime the object was created.</span></span> <span data-ttu-id="c6a9d-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-145">description</span><span class="sxs-lookup"><span data-stu-id="c6a9d-145">description</span></span>|<span data-ttu-id="c6a9d-146">String</span><span class="sxs-lookup"><span data-stu-id="c6a9d-146">String</span></span>|<span data-ttu-id="c6a9d-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c6a9d-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6a9d-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c6a9d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6a9d-150">DateTimeOffset</span></span>|<span data-ttu-id="c6a9d-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c6a9d-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c6a9d-153">displayName</span></span>|<span data-ttu-id="c6a9d-154">String</span><span class="sxs-lookup"><span data-stu-id="c6a9d-154">String</span></span>|<span data-ttu-id="c6a9d-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c6a9d-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-157">version</span><span class="sxs-lookup"><span data-stu-id="c6a9d-157">version</span></span>|<span data-ttu-id="c6a9d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-158">Int32</span></span>|<span data-ttu-id="c6a9d-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-159">Version of the device configuration.</span></span> <span data-ttu-id="c6a9d-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6a9d-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6a9d-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c6a9d-161">passcodeBlockSimple</span></span>|<span data-ttu-id="c6a9d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6a9d-162">Boolean</span></span>|<span data-ttu-id="c6a9d-163">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="c6a9d-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c6a9d-164">passcodeExpirationDays</span></span>|<span data-ttu-id="c6a9d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-165">Int32</span></span>|<span data-ttu-id="c6a9d-166">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="c6a9d-167">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="c6a9d-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c6a9d-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c6a9d-168">passcodeMinimumLength</span></span>|<span data-ttu-id="c6a9d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-169">Int32</span></span>|<span data-ttu-id="c6a9d-170">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-170">Minimum length of passcode.</span></span> <span data-ttu-id="c6a9d-171">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="c6a9d-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c6a9d-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c6a9d-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c6a9d-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-173">Int32</span></span>|<span data-ttu-id="c6a9d-174">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="c6a9d-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c6a9d-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c6a9d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-176">Int32</span></span>|<span data-ttu-id="c6a9d-177">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c6a9d-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="c6a9d-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="c6a9d-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-179">Int32</span></span>|<span data-ttu-id="c6a9d-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="c6a9d-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="c6a9d-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c6a9d-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c6a9d-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="c6a9d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a9d-183">Int32</span></span>|<span data-ttu-id="c6a9d-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c6a9d-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="c6a9d-185">passcodeRequiredType</span></span>|[<span data-ttu-id="c6a9d-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c6a9d-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c6a9d-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-187">The required passcode type.</span></span> <span data-ttu-id="c6a9d-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c6a9d-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="c6a9d-189">passcodeRequired</span></span>|<span data-ttu-id="c6a9d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6a9d-190">Boolean</span></span>|<span data-ttu-id="c6a9d-191">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="c6a9d-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c6a9d-192">osMinimumVersion</span></span>|<span data-ttu-id="c6a9d-193">String</span><span class="sxs-lookup"><span data-stu-id="c6a9d-193">String</span></span>|<span data-ttu-id="c6a9d-194">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="c6a9d-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c6a9d-195">osMaximumVersion</span></span>|<span data-ttu-id="c6a9d-196">String</span><span class="sxs-lookup"><span data-stu-id="c6a9d-196">String</span></span>|<span data-ttu-id="c6a9d-197">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="c6a9d-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c6a9d-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c6a9d-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6a9d-199">Boolean</span></span>|<span data-ttu-id="c6a9d-200">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c6a9d-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c6a9d-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c6a9d-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6a9d-202">Boolean</span></span>|<span data-ttu-id="c6a9d-203">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="c6a9d-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c6a9d-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c6a9d-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c6a9d-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c6a9d-206">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c6a9d-207">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c6a9d-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="c6a9d-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="c6a9d-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6a9d-209">Boolean</span></span>|<span data-ttu-id="c6a9d-210">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="c6a9d-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="c6a9d-211">restrictedApps</span></span>|<span data-ttu-id="c6a9d-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6a9d-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c6a9d-213">要求设备，没有安装指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="c6a9d-214">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c6a9d-215">响应</span><span class="sxs-lookup"><span data-stu-id="c6a9d-215">Response</span></span>
<span data-ttu-id="c6a9d-216">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-216">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6a9d-217">示例</span><span class="sxs-lookup"><span data-stu-id="c6a9d-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6a9d-218">请求</span><span class="sxs-lookup"><span data-stu-id="c6a9d-218">Request</span></span>
<span data-ttu-id="c6a9d-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1181

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="c6a9d-220">响应</span><span class="sxs-lookup"><span data-stu-id="c6a9d-220">Response</span></span>
<span data-ttu-id="c6a9d-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6a9d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1289

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





