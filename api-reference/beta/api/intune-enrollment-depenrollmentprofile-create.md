---
title: 创建 depEnrollmentProfile
description: 创建新的 depEnrollmentProfile 对象。
author: tfitzmac
ms.openlocfilehash: 5038013701692611272ffc922c81b37b16a55122
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350734"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="cbd26-103">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cbd26-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="cbd26-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cbd26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd26-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbd26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbd26-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cbd26-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbd26-107">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cbd26-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbd26-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbd26-108">Prerequisites</span></span>
<span data-ttu-id="cbd26-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cbd26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd26-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbd26-111">Permission type</span></span>|<span data-ttu-id="cbd26-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbd26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbd26-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbd26-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbd26-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cbd26-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbd26-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd26-116">Not supported.</span></span>|
|<span data-ttu-id="cbd26-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbd26-117">Application</span></span>|<span data-ttu-id="cbd26-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd26-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbd26-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbd26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cbd26-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbd26-120">Request headers</span></span>
|<span data-ttu-id="cbd26-121">标头</span><span class="sxs-lookup"><span data-stu-id="cbd26-121">Header</span></span>|<span data-ttu-id="cbd26-122">值</span><span class="sxs-lookup"><span data-stu-id="cbd26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbd26-123">授权</span><span class="sxs-lookup"><span data-stu-id="cbd26-123">Authorization</span></span>|<span data-ttu-id="cbd26-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbd26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbd26-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cbd26-125">Accept</span></span>|<span data-ttu-id="cbd26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbd26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbd26-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbd26-127">Request body</span></span>
<span data-ttu-id="cbd26-128">在请求正文中，提供 depEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbd26-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="cbd26-129">下表显示时创建 depEnrollmentProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cbd26-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="cbd26-130">属性</span><span class="sxs-lookup"><span data-stu-id="cbd26-130">Property</span></span>|<span data-ttu-id="cbd26-131">类型</span><span class="sxs-lookup"><span data-stu-id="cbd26-131">Type</span></span>|<span data-ttu-id="cbd26-132">说明</span><span class="sxs-lookup"><span data-stu-id="cbd26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd26-133">id</span><span class="sxs-lookup"><span data-stu-id="cbd26-133">id</span></span>|<span data-ttu-id="cbd26-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd26-134">String</span></span>|<span data-ttu-id="cbd26-135">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="cbd26-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbd26-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cbd26-136">displayName</span></span>|<span data-ttu-id="cbd26-137">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd26-137">String</span></span>|<span data-ttu-id="cbd26-138">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cbd26-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbd26-139">说明</span><span class="sxs-lookup"><span data-stu-id="cbd26-139">description</span></span>|<span data-ttu-id="cbd26-140">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd26-140">String</span></span>|<span data-ttu-id="cbd26-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cbd26-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbd26-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="cbd26-142">requiresUserAuthentication</span></span>|<span data-ttu-id="cbd26-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-143">Boolean</span></span>|<span data-ttu-id="cbd26-144">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="cbd26-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbd26-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="cbd26-145">configurationEndpointUrl</span></span>|<span data-ttu-id="cbd26-146">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd26-146">String</span></span>|<span data-ttu-id="cbd26-147">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cbd26-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbd26-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cbd26-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cbd26-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-149">Boolean</span></span>|<span data-ttu-id="cbd26-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="cbd26-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="cbd26-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cbd26-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbd26-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="cbd26-152">isDefault</span></span>|<span data-ttu-id="cbd26-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-153">Boolean</span></span>|<span data-ttu-id="cbd26-154">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="cbd26-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="cbd26-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-155">supervisedModeEnabled</span></span>|<span data-ttu-id="cbd26-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-156">Boolean</span></span>|<span data-ttu-id="cbd26-157">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="cbd26-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="cbd26-158">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="cbd26-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="cbd26-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="cbd26-159">supportDepartment</span></span>|<span data-ttu-id="cbd26-160">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd26-160">String</span></span>|<span data-ttu-id="cbd26-161">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="cbd26-161">Support department information</span></span>|
|<span data-ttu-id="cbd26-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-162">passCodeDisabled</span></span>|<span data-ttu-id="cbd26-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-163">Boolean</span></span>|<span data-ttu-id="cbd26-164">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="cbd26-165">isMandatory</span></span>|<span data-ttu-id="cbd26-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-166">Boolean</span></span>|<span data-ttu-id="cbd26-167">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="cbd26-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="cbd26-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-168">locationDisabled</span></span>|<span data-ttu-id="cbd26-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-169">Boolean</span></span>|<span data-ttu-id="cbd26-170">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="cbd26-171">supportPhoneNumber</span></span>|<span data-ttu-id="cbd26-172">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd26-172">String</span></span>|<span data-ttu-id="cbd26-173">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="cbd26-173">Support phone number</span></span>|
|<span data-ttu-id="cbd26-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="cbd26-174">iTunesPairingMode</span></span>|[<span data-ttu-id="cbd26-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="cbd26-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="cbd26-176">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="cbd26-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="cbd26-177">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="cbd26-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="cbd26-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-178">profileRemovalDisabled</span></span>|<span data-ttu-id="cbd26-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-179">Boolean</span></span>|<span data-ttu-id="cbd26-180">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="cbd26-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="cbd26-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="cbd26-181">managementCertificates</span></span>|<span data-ttu-id="cbd26-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="cbd26-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="cbd26-183">Apple 配置程序的管理证书</span><span class="sxs-lookup"><span data-stu-id="cbd26-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="cbd26-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="cbd26-184">restoreBlocked</span></span>|<span data-ttu-id="cbd26-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-185">Boolean</span></span>|<span data-ttu-id="cbd26-186">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="cbd26-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="cbd26-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="cbd26-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-188">Boolean</span></span>|<span data-ttu-id="cbd26-189">指示是否从 Android 还原被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="cbd26-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-190">appleIdDisabled</span></span>|<span data-ttu-id="cbd26-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-191">Boolean</span></span>|<span data-ttu-id="cbd26-192">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="cbd26-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-194">Boolean</span></span>|<span data-ttu-id="cbd26-195">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="cbd26-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-196">touchIdDisabled</span></span>|<span data-ttu-id="cbd26-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-197">Boolean</span></span>|<span data-ttu-id="cbd26-198">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-199">applePayDisabled</span></span>|<span data-ttu-id="cbd26-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-200">Boolean</span></span>|<span data-ttu-id="cbd26-201">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-202">zoomDisabled</span></span>|<span data-ttu-id="cbd26-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-203">Boolean</span></span>|<span data-ttu-id="cbd26-204">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-205">siriDisabled</span></span>|<span data-ttu-id="cbd26-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-206">Boolean</span></span>|<span data-ttu-id="cbd26-207">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-208">diagnosticsDisabled</span></span>|<span data-ttu-id="cbd26-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-209">Boolean</span></span>|<span data-ttu-id="cbd26-210">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="cbd26-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="cbd26-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="cbd26-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-212">Boolean</span></span>|<span data-ttu-id="cbd26-213">指示已禁用 Mac OS 注册功能</span><span class="sxs-lookup"><span data-stu-id="cbd26-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="cbd26-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="cbd26-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="cbd26-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-215">Boolean</span></span>|<span data-ttu-id="cbd26-216">指示是否禁用 Mac OS 文件存储库</span><span class="sxs-lookup"><span data-stu-id="cbd26-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="cbd26-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="cbd26-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="cbd26-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-218">Boolean</span></span>|<span data-ttu-id="cbd26-219">指示是否设备需要等待配置确认</span><span class="sxs-lookup"><span data-stu-id="cbd26-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="cbd26-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="cbd26-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="cbd26-221">Int32</span><span class="sxs-lookup"><span data-stu-id="cbd26-221">Int32</span></span>|<span data-ttu-id="cbd26-222">此选项指定的最大可以使用共享的 iPad 的用户数。</span><span class="sxs-lookup"><span data-stu-id="cbd26-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="cbd26-223">仅适用于共享的 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="cbd26-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="cbd26-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="cbd26-224">enableSharedIPad</span></span>|<span data-ttu-id="cbd26-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd26-225">Boolean</span></span>|<span data-ttu-id="cbd26-226">这指示是否要启用多用户方案模式注册设备。</span><span class="sxs-lookup"><span data-stu-id="cbd26-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="cbd26-227">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="cbd26-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="cbd26-228">响应</span><span class="sxs-lookup"><span data-stu-id="cbd26-228">Response</span></span>
<span data-ttu-id="cbd26-229">如果成功，此方法返回`201 Created`响应代码和响应正文中的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cbd26-229">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbd26-230">示例</span><span class="sxs-lookup"><span data-stu-id="cbd26-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbd26-231">请求</span><span class="sxs-lookup"><span data-stu-id="cbd26-231">Request</span></span>
<span data-ttu-id="cbd26-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbd26-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1290

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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

### <a name="response"></a><span data-ttu-id="cbd26-233">响应</span><span class="sxs-lookup"><span data-stu-id="cbd26-233">Response</span></span>
<span data-ttu-id="cbd26-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbd26-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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





