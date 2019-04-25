---
title: 创建 depEnrollmentProfile
description: 创建新的 depEnrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ce46c8ff178b62f7b99f7bf454ccd29689fac1e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533987"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="cba3c-103">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cba3c-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="cba3c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cba3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cba3c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cba3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cba3c-106">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cba3c-106">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cba3c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cba3c-107">Prerequisites</span></span>
<span data-ttu-id="cba3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cba3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cba3c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cba3c-110">Permission type</span></span>|<span data-ttu-id="cba3c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cba3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cba3c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cba3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cba3c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cba3c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cba3c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cba3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cba3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba3c-115">Not supported.</span></span>|
|<span data-ttu-id="cba3c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cba3c-116">Application</span></span>|<span data-ttu-id="cba3c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba3c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cba3c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cba3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cba3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cba3c-119">Request headers</span></span>
|<span data-ttu-id="cba3c-120">标头</span><span class="sxs-lookup"><span data-stu-id="cba3c-120">Header</span></span>|<span data-ttu-id="cba3c-121">值</span><span class="sxs-lookup"><span data-stu-id="cba3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cba3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba3c-122">Authorization</span></span>|<span data-ttu-id="cba3c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cba3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cba3c-124">接受</span><span class="sxs-lookup"><span data-stu-id="cba3c-124">Accept</span></span>|<span data-ttu-id="cba3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cba3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cba3c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cba3c-126">Request body</span></span>
<span data-ttu-id="cba3c-127">在请求正文中, 提供 depEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cba3c-127">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="cba3c-128">下表显示创建 depEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cba3c-128">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="cba3c-129">属性</span><span class="sxs-lookup"><span data-stu-id="cba3c-129">Property</span></span>|<span data-ttu-id="cba3c-130">类型</span><span class="sxs-lookup"><span data-stu-id="cba3c-130">Type</span></span>|<span data-ttu-id="cba3c-131">说明</span><span class="sxs-lookup"><span data-stu-id="cba3c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba3c-132">id</span><span class="sxs-lookup"><span data-stu-id="cba3c-132">id</span></span>|<span data-ttu-id="cba3c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cba3c-133">String</span></span>|<span data-ttu-id="cba3c-134">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="cba3c-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cba3c-135">displayName</span></span>|<span data-ttu-id="cba3c-136">String</span><span class="sxs-lookup"><span data-stu-id="cba3c-136">String</span></span>|<span data-ttu-id="cba3c-137">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cba3c-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-138">description</span><span class="sxs-lookup"><span data-stu-id="cba3c-138">description</span></span>|<span data-ttu-id="cba3c-139">String</span><span class="sxs-lookup"><span data-stu-id="cba3c-139">String</span></span>|<span data-ttu-id="cba3c-140">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cba3c-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="cba3c-141">requiresUserAuthentication</span></span>|<span data-ttu-id="cba3c-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-142">Boolean</span></span>|<span data-ttu-id="cba3c-143">指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="cba3c-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="cba3c-144">configurationEndpointUrl</span></span>|<span data-ttu-id="cba3c-145">String</span><span class="sxs-lookup"><span data-stu-id="cba3c-145">String</span></span>|<span data-ttu-id="cba3c-146">用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="cba3c-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cba3c-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cba3c-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-148">Boolean</span></span>|<span data-ttu-id="cba3c-149">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="cba3c-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="cba3c-150">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cba3c-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="cba3c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="cba3c-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-152">Boolean</span></span>|<span data-ttu-id="cba3c-153">指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="cba3c-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cba3c-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="cba3c-154">isDefault</span></span>|<span data-ttu-id="cba3c-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="cba3c-155">Boolean</span></span>|<span data-ttu-id="cba3c-156">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="cba3c-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="cba3c-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-157">supervisedModeEnabled</span></span>|<span data-ttu-id="cba3c-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-158">Boolean</span></span>|<span data-ttu-id="cba3c-159">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="cba3c-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="cba3c-160">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="cba3c-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="cba3c-161">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="cba3c-161">supportDepartment</span></span>|<span data-ttu-id="cba3c-162">String</span><span class="sxs-lookup"><span data-stu-id="cba3c-162">String</span></span>|<span data-ttu-id="cba3c-163">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="cba3c-163">Support department information</span></span>|
|<span data-ttu-id="cba3c-164">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-164">passCodeDisabled</span></span>|<span data-ttu-id="cba3c-165">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-165">Boolean</span></span>|<span data-ttu-id="cba3c-166">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-167">isMandatory</span><span class="sxs-lookup"><span data-stu-id="cba3c-167">isMandatory</span></span>|<span data-ttu-id="cba3c-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-168">Boolean</span></span>|<span data-ttu-id="cba3c-169">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="cba3c-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="cba3c-170">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-170">locationDisabled</span></span>|<span data-ttu-id="cba3c-171">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-171">Boolean</span></span>|<span data-ttu-id="cba3c-172">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="cba3c-173">supportPhoneNumber</span></span>|<span data-ttu-id="cba3c-174">String</span><span class="sxs-lookup"><span data-stu-id="cba3c-174">String</span></span>|<span data-ttu-id="cba3c-175">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="cba3c-175">Support phone number</span></span>|
|<span data-ttu-id="cba3c-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="cba3c-176">iTunesPairingMode</span></span>|[<span data-ttu-id="cba3c-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="cba3c-177">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="cba3c-178">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="cba3c-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="cba3c-179">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="cba3c-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="cba3c-180">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-180">profileRemovalDisabled</span></span>|<span data-ttu-id="cba3c-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-181">Boolean</span></span>|<span data-ttu-id="cba3c-182">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="cba3c-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="cba3c-183">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="cba3c-183">managementCertificates</span></span>|<span data-ttu-id="cba3c-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="cba3c-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="cba3c-185">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="cba3c-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="cba3c-186">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="cba3c-186">restoreBlocked</span></span>|<span data-ttu-id="cba3c-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-187">Boolean</span></span>|<span data-ttu-id="cba3c-188">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="cba3c-189">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="cba3c-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-190">Boolean</span></span>|<span data-ttu-id="cba3c-191">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="cba3c-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="cba3c-192">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-192">appleIdDisabled</span></span>|<span data-ttu-id="cba3c-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-193">Boolean</span></span>|<span data-ttu-id="cba3c-194">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-195">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="cba3c-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-196">Boolean</span></span>|<span data-ttu-id="cba3c-197">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-198">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-198">touchIdDisabled</span></span>|<span data-ttu-id="cba3c-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-199">Boolean</span></span>|<span data-ttu-id="cba3c-200">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-201">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-201">applePayDisabled</span></span>|<span data-ttu-id="cba3c-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-202">Boolean</span></span>|<span data-ttu-id="cba3c-203">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-204">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-204">zoomDisabled</span></span>|<span data-ttu-id="cba3c-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-205">Boolean</span></span>|<span data-ttu-id="cba3c-206">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-207">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-207">siriDisabled</span></span>|<span data-ttu-id="cba3c-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-208">Boolean</span></span>|<span data-ttu-id="cba3c-209">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-210">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-210">diagnosticsDisabled</span></span>|<span data-ttu-id="cba3c-211">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-211">Boolean</span></span>|<span data-ttu-id="cba3c-212">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="cba3c-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="cba3c-213">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="cba3c-214">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-214">Boolean</span></span>|<span data-ttu-id="cba3c-215">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="cba3c-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="cba3c-216">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="cba3c-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="cba3c-217">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-217">Boolean</span></span>|<span data-ttu-id="cba3c-218">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="cba3c-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="cba3c-219">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="cba3c-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="cba3c-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-220">Boolean</span></span>|<span data-ttu-id="cba3c-221">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="cba3c-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="cba3c-222">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="cba3c-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="cba3c-223">Int32</span><span class="sxs-lookup"><span data-stu-id="cba3c-223">Int32</span></span>|<span data-ttu-id="cba3c-224">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="cba3c-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="cba3c-225">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="cba3c-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="cba3c-226">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="cba3c-226">enableSharedIPad</span></span>|<span data-ttu-id="cba3c-227">布尔值</span><span class="sxs-lookup"><span data-stu-id="cba3c-227">Boolean</span></span>|<span data-ttu-id="cba3c-228">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="cba3c-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="cba3c-229">仅适用于共享 ipad。</span><span class="sxs-lookup"><span data-stu-id="cba3c-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="cba3c-230">响应</span><span class="sxs-lookup"><span data-stu-id="cba3c-230">Response</span></span>
<span data-ttu-id="cba3c-231">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cba3c-231">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba3c-232">示例</span><span class="sxs-lookup"><span data-stu-id="cba3c-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="cba3c-233">请求</span><span class="sxs-lookup"><span data-stu-id="cba3c-233">Request</span></span>
<span data-ttu-id="cba3c-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cba3c-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cba3c-235">响应</span><span class="sxs-lookup"><span data-stu-id="cba3c-235">Response</span></span>
<span data-ttu-id="cba3c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cba3c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





