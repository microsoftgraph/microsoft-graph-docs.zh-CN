---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9ee2476d85ec1446fea4b45fac834eb62f82bc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967880"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="2a33e-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2a33e-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="2a33e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2a33e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a33e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2a33e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a33e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a33e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a33e-107">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a33e-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a33e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a33e-108">Prerequisites</span></span>
<span data-ttu-id="2a33e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2a33e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a33e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a33e-111">Permission type</span></span>|<span data-ttu-id="2a33e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a33e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a33e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a33e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a33e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a33e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a33e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a33e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a33e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a33e-116">Not supported.</span></span>|
|<span data-ttu-id="2a33e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a33e-117">Application</span></span>|<span data-ttu-id="2a33e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a33e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a33e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a33e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2a33e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a33e-120">Request headers</span></span>
|<span data-ttu-id="2a33e-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a33e-121">Header</span></span>|<span data-ttu-id="2a33e-122">值</span><span class="sxs-lookup"><span data-stu-id="2a33e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a33e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a33e-123">Authorization</span></span>|<span data-ttu-id="2a33e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a33e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a33e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a33e-125">Accept</span></span>|<span data-ttu-id="2a33e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a33e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a33e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a33e-127">Request body</span></span>
<span data-ttu-id="2a33e-128">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a33e-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="2a33e-129">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a33e-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="2a33e-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a33e-130">Property</span></span>|<span data-ttu-id="2a33e-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a33e-131">Type</span></span>|<span data-ttu-id="2a33e-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a33e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a33e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2a33e-133">roleScopeTagIds</span></span>|<span data-ttu-id="2a33e-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="2a33e-134">String collection</span></span>|<span data-ttu-id="2a33e-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="2a33e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2a33e-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-137">id</span><span class="sxs-lookup"><span data-stu-id="2a33e-137">id</span></span>|<span data-ttu-id="2a33e-138">String</span><span class="sxs-lookup"><span data-stu-id="2a33e-138">String</span></span>|<span data-ttu-id="2a33e-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a33e-139">Key of the entity.</span></span> <span data-ttu-id="2a33e-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a33e-141">createdDateTime</span></span>|<span data-ttu-id="2a33e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a33e-142">DateTimeOffset</span></span>|<span data-ttu-id="2a33e-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2a33e-143">DateTime the object was created.</span></span> <span data-ttu-id="2a33e-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-145">description</span><span class="sxs-lookup"><span data-stu-id="2a33e-145">description</span></span>|<span data-ttu-id="2a33e-146">String</span><span class="sxs-lookup"><span data-stu-id="2a33e-146">String</span></span>|<span data-ttu-id="2a33e-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2a33e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2a33e-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a33e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2a33e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a33e-150">DateTimeOffset</span></span>|<span data-ttu-id="2a33e-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2a33e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2a33e-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2a33e-153">displayName</span></span>|<span data-ttu-id="2a33e-154">String</span><span class="sxs-lookup"><span data-stu-id="2a33e-154">String</span></span>|<span data-ttu-id="2a33e-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2a33e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2a33e-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-157">version</span><span class="sxs-lookup"><span data-stu-id="2a33e-157">version</span></span>|<span data-ttu-id="2a33e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-158">Int32</span></span>|<span data-ttu-id="2a33e-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2a33e-159">Version of the device configuration.</span></span> <span data-ttu-id="2a33e-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a33e-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2a33e-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2a33e-161">passcodeBlockSimple</span></span>|<span data-ttu-id="2a33e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a33e-162">Boolean</span></span>|<span data-ttu-id="2a33e-163">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="2a33e-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="2a33e-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2a33e-164">passcodeExpirationDays</span></span>|<span data-ttu-id="2a33e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-165">Int32</span></span>|<span data-ttu-id="2a33e-166">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2a33e-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="2a33e-167">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="2a33e-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="2a33e-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2a33e-168">passcodeMinimumLength</span></span>|<span data-ttu-id="2a33e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-169">Int32</span></span>|<span data-ttu-id="2a33e-170">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="2a33e-170">Minimum length of passcode.</span></span> <span data-ttu-id="2a33e-171">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="2a33e-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="2a33e-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2a33e-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2a33e-173">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-173">Int32</span></span>|<span data-ttu-id="2a33e-174">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="2a33e-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="2a33e-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2a33e-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2a33e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-176">Int32</span></span>|<span data-ttu-id="2a33e-177">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="2a33e-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2a33e-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="2a33e-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="2a33e-179">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-179">Int32</span></span>|<span data-ttu-id="2a33e-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2a33e-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="2a33e-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="2a33e-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="2a33e-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2a33e-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="2a33e-183">Int32</span><span class="sxs-lookup"><span data-stu-id="2a33e-183">Int32</span></span>|<span data-ttu-id="2a33e-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2a33e-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2a33e-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="2a33e-185">passcodeRequiredType</span></span>|[<span data-ttu-id="2a33e-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2a33e-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2a33e-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2a33e-187">The required passcode type.</span></span> <span data-ttu-id="2a33e-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2a33e-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2a33e-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="2a33e-189">passcodeRequired</span></span>|<span data-ttu-id="2a33e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a33e-190">Boolean</span></span>|<span data-ttu-id="2a33e-191">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="2a33e-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="2a33e-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2a33e-192">osMinimumVersion</span></span>|<span data-ttu-id="2a33e-193">String</span><span class="sxs-lookup"><span data-stu-id="2a33e-193">String</span></span>|<span data-ttu-id="2a33e-194">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="2a33e-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="2a33e-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2a33e-195">osMaximumVersion</span></span>|<span data-ttu-id="2a33e-196">String</span><span class="sxs-lookup"><span data-stu-id="2a33e-196">String</span></span>|<span data-ttu-id="2a33e-197">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="2a33e-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="2a33e-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="2a33e-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="2a33e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a33e-199">Boolean</span></span>|<span data-ttu-id="2a33e-200">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="2a33e-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="2a33e-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2a33e-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2a33e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a33e-202">Boolean</span></span>|<span data-ttu-id="2a33e-203">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="2a33e-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="2a33e-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2a33e-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2a33e-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2a33e-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2a33e-206">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="2a33e-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2a33e-207">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="2a33e-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2a33e-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="2a33e-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="2a33e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a33e-209">Boolean</span></span>|<span data-ttu-id="2a33e-210">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="2a33e-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="2a33e-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="2a33e-211">restrictedApps</span></span>|<span data-ttu-id="2a33e-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a33e-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2a33e-213">要求设备，没有安装指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2a33e-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="2a33e-214">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="2a33e-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2a33e-215">响应</span><span class="sxs-lookup"><span data-stu-id="2a33e-215">Response</span></span>
<span data-ttu-id="2a33e-216">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a33e-216">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a33e-217">示例</span><span class="sxs-lookup"><span data-stu-id="2a33e-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a33e-218">请求</span><span class="sxs-lookup"><span data-stu-id="2a33e-218">Request</span></span>
<span data-ttu-id="2a33e-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a33e-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1123

{
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

### <a name="response"></a><span data-ttu-id="2a33e-220">响应</span><span class="sxs-lookup"><span data-stu-id="2a33e-220">Response</span></span>
<span data-ttu-id="2a33e-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a33e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





