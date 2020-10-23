---
title: 创建 depEnrollmentProfile
description: 创建新的 depEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8157e164113de27bd0761bbf8a48bae380c2e42
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706665"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="6b370-103">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b370-103">Create depEnrollmentProfile</span></span>

<span data-ttu-id="6b370-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b370-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b370-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b370-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b370-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b370-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b370-107">创建新的 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b370-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b370-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b370-108">Prerequisites</span></span>
<span data-ttu-id="6b370-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b370-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b370-111">Permission type</span></span>|<span data-ttu-id="6b370-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b370-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b370-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b370-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b370-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b370-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6b370-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b370-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b370-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b370-116">Not supported.</span></span>|
|<span data-ttu-id="6b370-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b370-117">Application</span></span>|<span data-ttu-id="6b370-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b370-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b370-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b370-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6b370-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b370-120">Request headers</span></span>
|<span data-ttu-id="6b370-121">标头</span><span class="sxs-lookup"><span data-stu-id="6b370-121">Header</span></span>|<span data-ttu-id="6b370-122">值</span><span class="sxs-lookup"><span data-stu-id="6b370-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b370-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b370-123">Authorization</span></span>|<span data-ttu-id="6b370-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b370-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b370-125">接受</span><span class="sxs-lookup"><span data-stu-id="6b370-125">Accept</span></span>|<span data-ttu-id="6b370-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b370-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b370-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b370-127">Request body</span></span>
<span data-ttu-id="6b370-128">在请求正文中，提供 depEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b370-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="6b370-129">下表显示创建 depEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b370-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="6b370-130">属性</span><span class="sxs-lookup"><span data-stu-id="6b370-130">Property</span></span>|<span data-ttu-id="6b370-131">类型</span><span class="sxs-lookup"><span data-stu-id="6b370-131">Type</span></span>|<span data-ttu-id="6b370-132">说明</span><span class="sxs-lookup"><span data-stu-id="6b370-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b370-133">id</span><span class="sxs-lookup"><span data-stu-id="6b370-133">id</span></span>|<span data-ttu-id="6b370-134">String</span><span class="sxs-lookup"><span data-stu-id="6b370-134">String</span></span>|<span data-ttu-id="6b370-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="6b370-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6b370-136">displayName</span></span>|<span data-ttu-id="6b370-137">String</span><span class="sxs-lookup"><span data-stu-id="6b370-137">String</span></span>|<span data-ttu-id="6b370-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="6b370-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-139">说明</span><span class="sxs-lookup"><span data-stu-id="6b370-139">description</span></span>|<span data-ttu-id="6b370-140">String</span><span class="sxs-lookup"><span data-stu-id="6b370-140">String</span></span>|<span data-ttu-id="6b370-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="6b370-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6b370-142">requiresUserAuthentication</span></span>|<span data-ttu-id="6b370-143">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-143">Boolean</span></span>|<span data-ttu-id="6b370-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="6b370-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="6b370-145">configurationEndpointUrl</span></span>|<span data-ttu-id="6b370-146">String</span><span class="sxs-lookup"><span data-stu-id="6b370-146">String</span></span>|<span data-ttu-id="6b370-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="6b370-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6b370-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6b370-149">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-149">Boolean</span></span>|<span data-ttu-id="6b370-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6b370-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="6b370-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6b370-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="6b370-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6b370-153">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-153">Boolean</span></span>|<span data-ttu-id="6b370-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="6b370-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6b370-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="6b370-155">isDefault</span></span>|<span data-ttu-id="6b370-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b370-156">Boolean</span></span>|<span data-ttu-id="6b370-157">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="6b370-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="6b370-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="6b370-158">supervisedModeEnabled</span></span>|<span data-ttu-id="6b370-159">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-159">Boolean</span></span>|<span data-ttu-id="6b370-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="6b370-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="6b370-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="6b370-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="6b370-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="6b370-162">supportDepartment</span></span>|<span data-ttu-id="6b370-163">String</span><span class="sxs-lookup"><span data-stu-id="6b370-163">String</span></span>|<span data-ttu-id="6b370-164">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="6b370-164">Support department information</span></span>|
|<span data-ttu-id="6b370-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-165">passCodeDisabled</span></span>|<span data-ttu-id="6b370-166">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-166">Boolean</span></span>|<span data-ttu-id="6b370-167">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="6b370-168">isMandatory</span></span>|<span data-ttu-id="6b370-169">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-169">Boolean</span></span>|<span data-ttu-id="6b370-170">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="6b370-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="6b370-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-171">locationDisabled</span></span>|<span data-ttu-id="6b370-172">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-172">Boolean</span></span>|<span data-ttu-id="6b370-173">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="6b370-174">supportPhoneNumber</span></span>|<span data-ttu-id="6b370-175">String</span><span class="sxs-lookup"><span data-stu-id="6b370-175">String</span></span>|<span data-ttu-id="6b370-176">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="6b370-176">Support phone number</span></span>|
|<span data-ttu-id="6b370-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6b370-177">iTunesPairingMode</span></span>|[<span data-ttu-id="6b370-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6b370-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="6b370-179">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="6b370-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="6b370-180">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="6b370-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="6b370-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-181">profileRemovalDisabled</span></span>|<span data-ttu-id="6b370-182">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-182">Boolean</span></span>|<span data-ttu-id="6b370-183">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="6b370-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="6b370-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="6b370-184">managementCertificates</span></span>|<span data-ttu-id="6b370-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b370-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="6b370-186">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="6b370-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="6b370-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6b370-187">restoreBlocked</span></span>|<span data-ttu-id="6b370-188">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-188">Boolean</span></span>|<span data-ttu-id="6b370-189">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="6b370-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="6b370-191">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-191">Boolean</span></span>|<span data-ttu-id="6b370-192">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="6b370-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="6b370-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-193">appleIdDisabled</span></span>|<span data-ttu-id="6b370-194">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-194">Boolean</span></span>|<span data-ttu-id="6b370-195">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="6b370-197">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-197">Boolean</span></span>|<span data-ttu-id="6b370-198">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-199">touchIdDisabled</span></span>|<span data-ttu-id="6b370-200">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-200">Boolean</span></span>|<span data-ttu-id="6b370-201">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-202">applePayDisabled</span></span>|<span data-ttu-id="6b370-203">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-203">Boolean</span></span>|<span data-ttu-id="6b370-204">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-205">zoomDisabled</span></span>|<span data-ttu-id="6b370-206">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-206">Boolean</span></span>|<span data-ttu-id="6b370-207">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-208">siriDisabled</span></span>|<span data-ttu-id="6b370-209">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-209">Boolean</span></span>|<span data-ttu-id="6b370-210">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-211">diagnosticsDisabled</span></span>|<span data-ttu-id="6b370-212">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-212">Boolean</span></span>|<span data-ttu-id="6b370-213">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="6b370-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="6b370-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="6b370-215">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-215">Boolean</span></span>|<span data-ttu-id="6b370-216">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="6b370-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="6b370-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="6b370-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="6b370-218">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-218">Boolean</span></span>|<span data-ttu-id="6b370-219">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="6b370-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="6b370-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="6b370-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="6b370-221">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-221">Boolean</span></span>|<span data-ttu-id="6b370-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="6b370-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="6b370-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="6b370-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="6b370-224">Int32</span><span class="sxs-lookup"><span data-stu-id="6b370-224">Int32</span></span>|<span data-ttu-id="6b370-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="6b370-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="6b370-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="6b370-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="6b370-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="6b370-227">enableSharedIPad</span></span>|<span data-ttu-id="6b370-228">布尔</span><span class="sxs-lookup"><span data-stu-id="6b370-228">Boolean</span></span>|<span data-ttu-id="6b370-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="6b370-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="6b370-230">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="6b370-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="6b370-231">响应</span><span class="sxs-lookup"><span data-stu-id="6b370-231">Response</span></span>
<span data-ttu-id="6b370-232">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b370-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b370-233">示例</span><span class="sxs-lookup"><span data-stu-id="6b370-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b370-234">请求</span><span class="sxs-lookup"><span data-stu-id="6b370-234">Request</span></span>
<span data-ttu-id="6b370-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b370-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b370-236">响应</span><span class="sxs-lookup"><span data-stu-id="6b370-236">Response</span></span>
<span data-ttu-id="6b370-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b370-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





