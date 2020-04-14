---
title: 更新 depEnrollmentProfile
description: 更新 depEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca8d1387d2b96368a4891825d5ddaf3e03d012fd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413859"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="200ed-103">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="200ed-103">Update depEnrollmentProfile</span></span>

<span data-ttu-id="200ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="200ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="200ed-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="200ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="200ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="200ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="200ed-107">更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="200ed-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="200ed-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="200ed-108">Prerequisites</span></span>
<span data-ttu-id="200ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="200ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="200ed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="200ed-111">Permission type</span></span>|<span data-ttu-id="200ed-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="200ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="200ed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="200ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="200ed-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200ed-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="200ed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="200ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="200ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="200ed-116">Not supported.</span></span>|
|<span data-ttu-id="200ed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="200ed-117">Application</span></span>|<span data-ttu-id="200ed-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200ed-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="200ed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="200ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="200ed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="200ed-120">Request headers</span></span>
|<span data-ttu-id="200ed-121">标头</span><span class="sxs-lookup"><span data-stu-id="200ed-121">Header</span></span>|<span data-ttu-id="200ed-122">值</span><span class="sxs-lookup"><span data-stu-id="200ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="200ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="200ed-123">Authorization</span></span>|<span data-ttu-id="200ed-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="200ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="200ed-125">接受</span><span class="sxs-lookup"><span data-stu-id="200ed-125">Accept</span></span>|<span data-ttu-id="200ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="200ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="200ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="200ed-127">Request body</span></span>
<span data-ttu-id="200ed-128">在请求正文中，提供[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="200ed-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="200ed-129">下表显示创建[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="200ed-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="200ed-130">属性</span><span class="sxs-lookup"><span data-stu-id="200ed-130">Property</span></span>|<span data-ttu-id="200ed-131">类型</span><span class="sxs-lookup"><span data-stu-id="200ed-131">Type</span></span>|<span data-ttu-id="200ed-132">说明</span><span class="sxs-lookup"><span data-stu-id="200ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="200ed-133">id</span><span class="sxs-lookup"><span data-stu-id="200ed-133">id</span></span>|<span data-ttu-id="200ed-134">字符串</span><span class="sxs-lookup"><span data-stu-id="200ed-134">String</span></span>|<span data-ttu-id="200ed-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="200ed-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="200ed-136">displayName</span></span>|<span data-ttu-id="200ed-137">String</span><span class="sxs-lookup"><span data-stu-id="200ed-137">String</span></span>|<span data-ttu-id="200ed-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="200ed-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-139">description</span><span class="sxs-lookup"><span data-stu-id="200ed-139">description</span></span>|<span data-ttu-id="200ed-140">String</span><span class="sxs-lookup"><span data-stu-id="200ed-140">String</span></span>|<span data-ttu-id="200ed-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="200ed-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="200ed-142">requiresUserAuthentication</span></span>|<span data-ttu-id="200ed-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-143">Boolean</span></span>|<span data-ttu-id="200ed-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="200ed-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="200ed-145">configurationEndpointUrl</span></span>|<span data-ttu-id="200ed-146">String</span><span class="sxs-lookup"><span data-stu-id="200ed-146">String</span></span>|<span data-ttu-id="200ed-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="200ed-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="200ed-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="200ed-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-149">Boolean</span></span>|<span data-ttu-id="200ed-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="200ed-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="200ed-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200ed-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="200ed-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="200ed-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-153">Boolean</span></span>|<span data-ttu-id="200ed-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="200ed-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200ed-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="200ed-155">isDefault</span></span>|<span data-ttu-id="200ed-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-156">Boolean</span></span>|<span data-ttu-id="200ed-157">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="200ed-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="200ed-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="200ed-158">supervisedModeEnabled</span></span>|<span data-ttu-id="200ed-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-159">Boolean</span></span>|<span data-ttu-id="200ed-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="200ed-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="200ed-161">有关https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="200ed-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="200ed-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="200ed-162">supportDepartment</span></span>|<span data-ttu-id="200ed-163">String</span><span class="sxs-lookup"><span data-stu-id="200ed-163">String</span></span>|<span data-ttu-id="200ed-164">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="200ed-164">Support department information</span></span>|
|<span data-ttu-id="200ed-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-165">passCodeDisabled</span></span>|<span data-ttu-id="200ed-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-166">Boolean</span></span>|<span data-ttu-id="200ed-167">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="200ed-168">isMandatory</span></span>|<span data-ttu-id="200ed-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-169">Boolean</span></span>|<span data-ttu-id="200ed-170">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="200ed-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="200ed-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-171">locationDisabled</span></span>|<span data-ttu-id="200ed-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-172">Boolean</span></span>|<span data-ttu-id="200ed-173">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="200ed-174">supportPhoneNumber</span></span>|<span data-ttu-id="200ed-175">String</span><span class="sxs-lookup"><span data-stu-id="200ed-175">String</span></span>|<span data-ttu-id="200ed-176">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="200ed-176">Support phone number</span></span>|
|<span data-ttu-id="200ed-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="200ed-177">iTunesPairingMode</span></span>|[<span data-ttu-id="200ed-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="200ed-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="200ed-179">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="200ed-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="200ed-180">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="200ed-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="200ed-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-181">profileRemovalDisabled</span></span>|<span data-ttu-id="200ed-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-182">Boolean</span></span>|<span data-ttu-id="200ed-183">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="200ed-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="200ed-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="200ed-184">managementCertificates</span></span>|<span data-ttu-id="200ed-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="200ed-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="200ed-186">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="200ed-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="200ed-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="200ed-187">restoreBlocked</span></span>|<span data-ttu-id="200ed-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-188">Boolean</span></span>|<span data-ttu-id="200ed-189">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="200ed-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="200ed-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-191">Boolean</span></span>|<span data-ttu-id="200ed-192">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="200ed-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="200ed-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-193">appleIdDisabled</span></span>|<span data-ttu-id="200ed-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-194">Boolean</span></span>|<span data-ttu-id="200ed-195">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="200ed-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-197">Boolean</span></span>|<span data-ttu-id="200ed-198">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-199">touchIdDisabled</span></span>|<span data-ttu-id="200ed-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-200">Boolean</span></span>|<span data-ttu-id="200ed-201">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-202">applePayDisabled</span></span>|<span data-ttu-id="200ed-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-203">Boolean</span></span>|<span data-ttu-id="200ed-204">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-205">zoomDisabled</span></span>|<span data-ttu-id="200ed-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-206">Boolean</span></span>|<span data-ttu-id="200ed-207">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-208">siriDisabled</span></span>|<span data-ttu-id="200ed-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-209">Boolean</span></span>|<span data-ttu-id="200ed-210">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-211">diagnosticsDisabled</span></span>|<span data-ttu-id="200ed-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-212">Boolean</span></span>|<span data-ttu-id="200ed-213">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="200ed-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="200ed-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="200ed-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-215">Boolean</span></span>|<span data-ttu-id="200ed-216">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="200ed-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="200ed-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="200ed-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="200ed-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-218">Boolean</span></span>|<span data-ttu-id="200ed-219">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="200ed-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="200ed-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="200ed-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="200ed-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-221">Boolean</span></span>|<span data-ttu-id="200ed-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="200ed-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="200ed-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="200ed-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="200ed-224">Int32</span><span class="sxs-lookup"><span data-stu-id="200ed-224">Int32</span></span>|<span data-ttu-id="200ed-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="200ed-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="200ed-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="200ed-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="200ed-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="200ed-227">enableSharedIPad</span></span>|<span data-ttu-id="200ed-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="200ed-228">Boolean</span></span>|<span data-ttu-id="200ed-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="200ed-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="200ed-230">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="200ed-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="200ed-231">响应</span><span class="sxs-lookup"><span data-stu-id="200ed-231">Response</span></span>
<span data-ttu-id="200ed-232">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="200ed-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="200ed-233">示例</span><span class="sxs-lookup"><span data-stu-id="200ed-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="200ed-234">请求</span><span class="sxs-lookup"><span data-stu-id="200ed-234">Request</span></span>
<span data-ttu-id="200ed-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="200ed-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a><span data-ttu-id="200ed-236">响应</span><span class="sxs-lookup"><span data-stu-id="200ed-236">Response</span></span>
<span data-ttu-id="200ed-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="200ed-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```



