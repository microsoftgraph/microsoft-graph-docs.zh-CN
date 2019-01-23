---
title: 创建 depEnrollmentProfile
description: 创建新的 depEnrollmentProfile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bc6b11a8367ff28b4e4b9957879e251cb939c7e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416312"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="6f79e-103">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6f79e-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="6f79e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6f79e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f79e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f79e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f79e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f79e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f79e-107">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6f79e-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f79e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f79e-108">Prerequisites</span></span>
<span data-ttu-id="6f79e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6f79e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f79e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f79e-111">Permission type</span></span>|<span data-ttu-id="6f79e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f79e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f79e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f79e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f79e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f79e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f79e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f79e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f79e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f79e-116">Not supported.</span></span>|
|<span data-ttu-id="6f79e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f79e-117">Application</span></span>|<span data-ttu-id="6f79e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f79e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f79e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f79e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6f79e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f79e-120">Request headers</span></span>
|<span data-ttu-id="6f79e-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f79e-121">Header</span></span>|<span data-ttu-id="6f79e-122">值</span><span class="sxs-lookup"><span data-stu-id="6f79e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f79e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f79e-123">Authorization</span></span>|<span data-ttu-id="6f79e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f79e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f79e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f79e-125">Accept</span></span>|<span data-ttu-id="6f79e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f79e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f79e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f79e-127">Request body</span></span>
<span data-ttu-id="6f79e-128">在请求正文中，提供 depEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f79e-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="6f79e-129">下表显示时创建 depEnrollmentProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6f79e-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="6f79e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f79e-130">Property</span></span>|<span data-ttu-id="6f79e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f79e-131">Type</span></span>|<span data-ttu-id="6f79e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f79e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f79e-133">id</span><span class="sxs-lookup"><span data-stu-id="6f79e-133">id</span></span>|<span data-ttu-id="6f79e-134">String</span><span class="sxs-lookup"><span data-stu-id="6f79e-134">String</span></span>|<span data-ttu-id="6f79e-135">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="6f79e-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6f79e-136">displayName</span></span>|<span data-ttu-id="6f79e-137">String</span><span class="sxs-lookup"><span data-stu-id="6f79e-137">String</span></span>|<span data-ttu-id="6f79e-138">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="6f79e-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-139">说明</span><span class="sxs-lookup"><span data-stu-id="6f79e-139">description</span></span>|<span data-ttu-id="6f79e-140">String</span><span class="sxs-lookup"><span data-stu-id="6f79e-140">String</span></span>|<span data-ttu-id="6f79e-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="6f79e-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6f79e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="6f79e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-143">Boolean</span></span>|<span data-ttu-id="6f79e-144">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="6f79e-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="6f79e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="6f79e-146">String</span><span class="sxs-lookup"><span data-stu-id="6f79e-146">String</span></span>|<span data-ttu-id="6f79e-147">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f79e-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6f79e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6f79e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-149">Boolean</span></span>|<span data-ttu-id="6f79e-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6f79e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="6f79e-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f79e-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="6f79e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6f79e-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-153">Boolean</span></span>|<span data-ttu-id="6f79e-154">指示安装程序注册的助手设备继承[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) ，需要的公司门户</span><span class="sxs-lookup"><span data-stu-id="6f79e-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6f79e-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="6f79e-155">isDefault</span></span>|<span data-ttu-id="6f79e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-156">Boolean</span></span>|<span data-ttu-id="6f79e-157">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="6f79e-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="6f79e-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-158">supervisedModeEnabled</span></span>|<span data-ttu-id="6f79e-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-159">Boolean</span></span>|<span data-ttu-id="6f79e-160">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="6f79e-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="6f79e-161">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="6f79e-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="6f79e-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="6f79e-162">supportDepartment</span></span>|<span data-ttu-id="6f79e-163">String</span><span class="sxs-lookup"><span data-stu-id="6f79e-163">String</span></span>|<span data-ttu-id="6f79e-164">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="6f79e-164">Support department information</span></span>|
|<span data-ttu-id="6f79e-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-165">passCodeDisabled</span></span>|<span data-ttu-id="6f79e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-166">Boolean</span></span>|<span data-ttu-id="6f79e-167">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="6f79e-168">isMandatory</span></span>|<span data-ttu-id="6f79e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-169">Boolean</span></span>|<span data-ttu-id="6f79e-170">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="6f79e-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="6f79e-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-171">locationDisabled</span></span>|<span data-ttu-id="6f79e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-172">Boolean</span></span>|<span data-ttu-id="6f79e-173">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="6f79e-174">supportPhoneNumber</span></span>|<span data-ttu-id="6f79e-175">String</span><span class="sxs-lookup"><span data-stu-id="6f79e-175">String</span></span>|<span data-ttu-id="6f79e-176">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="6f79e-176">Support phone number</span></span>|
|<span data-ttu-id="6f79e-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6f79e-177">iTunesPairingMode</span></span>|[<span data-ttu-id="6f79e-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6f79e-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="6f79e-179">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="6f79e-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="6f79e-180">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="6f79e-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="6f79e-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-181">profileRemovalDisabled</span></span>|<span data-ttu-id="6f79e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-182">Boolean</span></span>|<span data-ttu-id="6f79e-183">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="6f79e-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="6f79e-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="6f79e-184">managementCertificates</span></span>|<span data-ttu-id="6f79e-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="6f79e-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="6f79e-186">Apple 配置程序的管理证书</span><span class="sxs-lookup"><span data-stu-id="6f79e-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="6f79e-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6f79e-187">restoreBlocked</span></span>|<span data-ttu-id="6f79e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-188">Boolean</span></span>|<span data-ttu-id="6f79e-189">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="6f79e-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="6f79e-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="6f79e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-191">Boolean</span></span>|<span data-ttu-id="6f79e-192">指示是否从 Android 还原被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="6f79e-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-193">appleIdDisabled</span></span>|<span data-ttu-id="6f79e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-194">Boolean</span></span>|<span data-ttu-id="6f79e-195">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="6f79e-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-197">Boolean</span></span>|<span data-ttu-id="6f79e-198">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="6f79e-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-199">touchIdDisabled</span></span>|<span data-ttu-id="6f79e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-200">Boolean</span></span>|<span data-ttu-id="6f79e-201">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-202">applePayDisabled</span></span>|<span data-ttu-id="6f79e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-203">Boolean</span></span>|<span data-ttu-id="6f79e-204">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-205">zoomDisabled</span></span>|<span data-ttu-id="6f79e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-206">Boolean</span></span>|<span data-ttu-id="6f79e-207">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-208">siriDisabled</span></span>|<span data-ttu-id="6f79e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-209">Boolean</span></span>|<span data-ttu-id="6f79e-210">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-211">diagnosticsDisabled</span></span>|<span data-ttu-id="6f79e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-212">Boolean</span></span>|<span data-ttu-id="6f79e-213">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="6f79e-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="6f79e-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="6f79e-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-215">Boolean</span></span>|<span data-ttu-id="6f79e-216">指示已禁用 Mac OS 注册功能</span><span class="sxs-lookup"><span data-stu-id="6f79e-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="6f79e-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="6f79e-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="6f79e-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-218">Boolean</span></span>|<span data-ttu-id="6f79e-219">指示是否禁用 Mac OS 文件存储库</span><span class="sxs-lookup"><span data-stu-id="6f79e-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="6f79e-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="6f79e-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="6f79e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-221">Boolean</span></span>|<span data-ttu-id="6f79e-222">指示是否设备需要等待配置确认</span><span class="sxs-lookup"><span data-stu-id="6f79e-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="6f79e-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="6f79e-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="6f79e-224">Int32</span><span class="sxs-lookup"><span data-stu-id="6f79e-224">Int32</span></span>|<span data-ttu-id="6f79e-225">此选项指定的最大可以使用共享的 iPad 的用户数。</span><span class="sxs-lookup"><span data-stu-id="6f79e-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="6f79e-226">仅适用于共享的 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="6f79e-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="6f79e-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="6f79e-227">enableSharedIPad</span></span>|<span data-ttu-id="6f79e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f79e-228">Boolean</span></span>|<span data-ttu-id="6f79e-229">这指示是否要启用多用户方案模式注册设备。</span><span class="sxs-lookup"><span data-stu-id="6f79e-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="6f79e-230">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="6f79e-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="6f79e-231">响应</span><span class="sxs-lookup"><span data-stu-id="6f79e-231">Response</span></span>
<span data-ttu-id="6f79e-232">如果成功，此方法返回`201 Created`响应代码和响应正文中的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6f79e-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f79e-233">示例</span><span class="sxs-lookup"><span data-stu-id="6f79e-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f79e-234">请求</span><span class="sxs-lookup"><span data-stu-id="6f79e-234">Request</span></span>
<span data-ttu-id="6f79e-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f79e-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="6f79e-236">响应</span><span class="sxs-lookup"><span data-stu-id="6f79e-236">Response</span></span>
<span data-ttu-id="6f79e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f79e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




