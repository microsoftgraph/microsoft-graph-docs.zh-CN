---
title: 更新 depEnrollmentProfile
description: 更新 depEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6183fed00b52144e5d24ed9ecfba064bdbbca3d2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201994"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="f4a11-103">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f4a11-103">Update depEnrollmentProfile</span></span>

<span data-ttu-id="f4a11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4a11-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4a11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4a11-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4a11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a11-107">更新 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4a11-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4a11-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4a11-108">Prerequisites</span></span>
<span data-ttu-id="f4a11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4a11-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4a11-111">Permission type</span></span>|<span data-ttu-id="f4a11-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4a11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4a11-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4a11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4a11-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a11-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4a11-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4a11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4a11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4a11-116">Not supported.</span></span>|
|<span data-ttu-id="f4a11-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4a11-117">Application</span></span>|<span data-ttu-id="f4a11-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a11-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4a11-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4a11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="f4a11-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4a11-120">Request headers</span></span>
|<span data-ttu-id="f4a11-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4a11-121">Header</span></span>|<span data-ttu-id="f4a11-122">值</span><span class="sxs-lookup"><span data-stu-id="f4a11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4a11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4a11-123">Authorization</span></span>|<span data-ttu-id="f4a11-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4a11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4a11-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4a11-125">Accept</span></span>|<span data-ttu-id="f4a11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4a11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4a11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4a11-127">Request body</span></span>
<span data-ttu-id="f4a11-128">在请求正文中，提供 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4a11-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="f4a11-129">下表显示创建 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4a11-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="f4a11-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4a11-130">Property</span></span>|<span data-ttu-id="f4a11-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4a11-131">Type</span></span>|<span data-ttu-id="f4a11-132">说明</span><span class="sxs-lookup"><span data-stu-id="f4a11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a11-133">id</span><span class="sxs-lookup"><span data-stu-id="f4a11-133">id</span></span>|<span data-ttu-id="f4a11-134">String</span><span class="sxs-lookup"><span data-stu-id="f4a11-134">String</span></span>|<span data-ttu-id="f4a11-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="f4a11-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f4a11-136">displayName</span></span>|<span data-ttu-id="f4a11-137">String</span><span class="sxs-lookup"><span data-stu-id="f4a11-137">String</span></span>|<span data-ttu-id="f4a11-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="f4a11-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-139">description</span><span class="sxs-lookup"><span data-stu-id="f4a11-139">description</span></span>|<span data-ttu-id="f4a11-140">String</span><span class="sxs-lookup"><span data-stu-id="f4a11-140">String</span></span>|<span data-ttu-id="f4a11-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="f4a11-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f4a11-142">requiresUserAuthentication</span></span>|<span data-ttu-id="f4a11-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-143">Boolean</span></span>|<span data-ttu-id="f4a11-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="f4a11-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f4a11-145">configurationEndpointUrl</span></span>|<span data-ttu-id="f4a11-146">String</span><span class="sxs-lookup"><span data-stu-id="f4a11-146">String</span></span>|<span data-ttu-id="f4a11-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="f4a11-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f4a11-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f4a11-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-149">Boolean</span></span>|<span data-ttu-id="f4a11-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="f4a11-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f4a11-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4a11-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f4a11-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f4a11-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-153">Boolean</span></span>|<span data-ttu-id="f4a11-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="f4a11-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4a11-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="f4a11-155">isDefault</span></span>|<span data-ttu-id="f4a11-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-156">Boolean</span></span>|<span data-ttu-id="f4a11-157">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="f4a11-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="f4a11-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-158">supervisedModeEnabled</span></span>|<span data-ttu-id="f4a11-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-159">Boolean</span></span>|<span data-ttu-id="f4a11-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="f4a11-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f4a11-161"> https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="f4a11-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="f4a11-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f4a11-162">supportDepartment</span></span>|<span data-ttu-id="f4a11-163">String</span><span class="sxs-lookup"><span data-stu-id="f4a11-163">String</span></span>|<span data-ttu-id="f4a11-164">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="f4a11-164">Support department information</span></span>|
|<span data-ttu-id="f4a11-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-165">passCodeDisabled</span></span>|<span data-ttu-id="f4a11-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-166">Boolean</span></span>|<span data-ttu-id="f4a11-167">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="f4a11-168">isMandatory</span></span>|<span data-ttu-id="f4a11-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-169">Boolean</span></span>|<span data-ttu-id="f4a11-170">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="f4a11-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="f4a11-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-171">locationDisabled</span></span>|<span data-ttu-id="f4a11-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-172">Boolean</span></span>|<span data-ttu-id="f4a11-173">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f4a11-174">supportPhoneNumber</span></span>|<span data-ttu-id="f4a11-175">String</span><span class="sxs-lookup"><span data-stu-id="f4a11-175">String</span></span>|<span data-ttu-id="f4a11-176">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="f4a11-176">Support phone number</span></span>|
|<span data-ttu-id="f4a11-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="f4a11-177">iTunesPairingMode</span></span>|[<span data-ttu-id="f4a11-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="f4a11-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="f4a11-179">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="f4a11-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="f4a11-180">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="f4a11-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="f4a11-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-181">profileRemovalDisabled</span></span>|<span data-ttu-id="f4a11-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-182">Boolean</span></span>|<span data-ttu-id="f4a11-183">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="f4a11-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="f4a11-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="f4a11-184">managementCertificates</span></span>|<span data-ttu-id="f4a11-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4a11-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="f4a11-186">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="f4a11-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="f4a11-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f4a11-187">restoreBlocked</span></span>|<span data-ttu-id="f4a11-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-188">Boolean</span></span>|<span data-ttu-id="f4a11-189">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="f4a11-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="f4a11-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-191">Boolean</span></span>|<span data-ttu-id="f4a11-192">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="f4a11-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="f4a11-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-193">appleIdDisabled</span></span>|<span data-ttu-id="f4a11-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-194">Boolean</span></span>|<span data-ttu-id="f4a11-195">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f4a11-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-197">Boolean</span></span>|<span data-ttu-id="f4a11-198">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-199">touchIdDisabled</span></span>|<span data-ttu-id="f4a11-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-200">Boolean</span></span>|<span data-ttu-id="f4a11-201">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-202">applePayDisabled</span></span>|<span data-ttu-id="f4a11-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-203">Boolean</span></span>|<span data-ttu-id="f4a11-204">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-205">zoomDisabled</span></span>|<span data-ttu-id="f4a11-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-206">Boolean</span></span>|<span data-ttu-id="f4a11-207">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-208">siriDisabled</span></span>|<span data-ttu-id="f4a11-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-209">Boolean</span></span>|<span data-ttu-id="f4a11-210">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-211">diagnosticsDisabled</span></span>|<span data-ttu-id="f4a11-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-212">Boolean</span></span>|<span data-ttu-id="f4a11-213">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="f4a11-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="f4a11-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="f4a11-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-215">Boolean</span></span>|<span data-ttu-id="f4a11-216">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="f4a11-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="f4a11-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="f4a11-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="f4a11-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-218">Boolean</span></span>|<span data-ttu-id="f4a11-219">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="f4a11-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="f4a11-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="f4a11-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="f4a11-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-221">Boolean</span></span>|<span data-ttu-id="f4a11-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="f4a11-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="f4a11-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="f4a11-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="f4a11-224">Int32</span><span class="sxs-lookup"><span data-stu-id="f4a11-224">Int32</span></span>|<span data-ttu-id="f4a11-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="f4a11-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="f4a11-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="f4a11-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="f4a11-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="f4a11-227">enableSharedIPad</span></span>|<span data-ttu-id="f4a11-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4a11-228">Boolean</span></span>|<span data-ttu-id="f4a11-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="f4a11-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="f4a11-230">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="f4a11-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="f4a11-231">响应</span><span class="sxs-lookup"><span data-stu-id="f4a11-231">Response</span></span>
<span data-ttu-id="f4a11-232">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4a11-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4a11-233">示例</span><span class="sxs-lookup"><span data-stu-id="f4a11-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4a11-234">请求</span><span class="sxs-lookup"><span data-stu-id="f4a11-234">Request</span></span>
<span data-ttu-id="f4a11-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4a11-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4a11-236">响应</span><span class="sxs-lookup"><span data-stu-id="f4a11-236">Response</span></span>
<span data-ttu-id="f4a11-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4a11-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




