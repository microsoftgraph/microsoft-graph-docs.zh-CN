---
title: 更新 depIOSEnrollmentProfile
description: 更新 depIOSEnrollmentProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea708a5ffe661f8024c027d1ac9ef10877474cd6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986941"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="58541-103">更新 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="58541-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="58541-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58541-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58541-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58541-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58541-106">更新[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58541-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58541-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="58541-107">Prerequisites</span></span>
<span data-ttu-id="58541-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58541-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="58541-110">Permission type</span></span>|<span data-ttu-id="58541-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58541-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58541-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58541-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58541-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58541-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58541-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58541-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58541-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="58541-115">Not supported.</span></span>|
|<span data-ttu-id="58541-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="58541-116">Application</span></span>|<span data-ttu-id="58541-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="58541-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58541-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58541-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="58541-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="58541-119">Request headers</span></span>
|<span data-ttu-id="58541-120">标头</span><span class="sxs-lookup"><span data-stu-id="58541-120">Header</span></span>|<span data-ttu-id="58541-121">值</span><span class="sxs-lookup"><span data-stu-id="58541-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58541-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58541-122">Authorization</span></span>|<span data-ttu-id="58541-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58541-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58541-124">接受</span><span class="sxs-lookup"><span data-stu-id="58541-124">Accept</span></span>|<span data-ttu-id="58541-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58541-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58541-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="58541-126">Request body</span></span>
<span data-ttu-id="58541-127">在请求正文中, 提供[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58541-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="58541-128">下表显示创建[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58541-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="58541-129">属性</span><span class="sxs-lookup"><span data-stu-id="58541-129">Property</span></span>|<span data-ttu-id="58541-130">类型</span><span class="sxs-lookup"><span data-stu-id="58541-130">Type</span></span>|<span data-ttu-id="58541-131">说明</span><span class="sxs-lookup"><span data-stu-id="58541-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58541-132">id</span><span class="sxs-lookup"><span data-stu-id="58541-132">id</span></span>|<span data-ttu-id="58541-133">String</span><span class="sxs-lookup"><span data-stu-id="58541-133">String</span></span>|<span data-ttu-id="58541-134">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="58541-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-135">displayName</span><span class="sxs-lookup"><span data-stu-id="58541-135">displayName</span></span>|<span data-ttu-id="58541-136">String</span><span class="sxs-lookup"><span data-stu-id="58541-136">String</span></span>|<span data-ttu-id="58541-137">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="58541-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-138">description</span><span class="sxs-lookup"><span data-stu-id="58541-138">description</span></span>|<span data-ttu-id="58541-139">String</span><span class="sxs-lookup"><span data-stu-id="58541-139">String</span></span>|<span data-ttu-id="58541-140">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="58541-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="58541-141">requiresUserAuthentication</span></span>|<span data-ttu-id="58541-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-142">Boolean</span></span>|<span data-ttu-id="58541-143">指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="58541-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="58541-144">configurationEndpointUrl</span></span>|<span data-ttu-id="58541-145">String</span><span class="sxs-lookup"><span data-stu-id="58541-145">String</span></span>|<span data-ttu-id="58541-146">用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="58541-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="58541-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="58541-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-148">Boolean</span></span>|<span data-ttu-id="58541-149">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="58541-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="58541-150">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58541-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="58541-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="58541-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-152">Boolean</span></span>|<span data-ttu-id="58541-153">指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="58541-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58541-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="58541-154">isDefault</span></span>|<span data-ttu-id="58541-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-155">Boolean</span></span>|<span data-ttu-id="58541-156">指示这是否是从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="58541-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="58541-157">supervisedModeEnabled</span></span>|<span data-ttu-id="58541-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-158">Boolean</span></span>|<span data-ttu-id="58541-159">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="58541-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="58541-160">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="58541-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="58541-161">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58541-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="58541-162">supportDepartment</span></span>|<span data-ttu-id="58541-163">String</span><span class="sxs-lookup"><span data-stu-id="58541-163">String</span></span>|<span data-ttu-id="58541-164">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="58541-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-165">passCodeDisabled</span></span>|<span data-ttu-id="58541-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-166">Boolean</span></span>|<span data-ttu-id="58541-167">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="58541-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="58541-168">isMandatory</span></span>|<span data-ttu-id="58541-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-169">Boolean</span></span>|<span data-ttu-id="58541-170">指示是否必须从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="58541-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-171">locationDisabled</span></span>|<span data-ttu-id="58541-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-172">Boolean</span></span>|<span data-ttu-id="58541-173">指示是否禁用从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="58541-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="58541-174">supportPhoneNumber</span></span>|<span data-ttu-id="58541-175">String</span><span class="sxs-lookup"><span data-stu-id="58541-175">String</span></span>|<span data-ttu-id="58541-176">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="58541-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-177">profileRemovalDisabled</span></span>|<span data-ttu-id="58541-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-178">Boolean</span></span>|<span data-ttu-id="58541-179">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="58541-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="58541-180">restoreBlocked</span></span>|<span data-ttu-id="58541-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-181">Boolean</span></span>|<span data-ttu-id="58541-182">指示是否阻止从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="58541-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-183">appleIdDisabled</span></span>|<span data-ttu-id="58541-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-184">Boolean</span></span>|<span data-ttu-id="58541-185">指示是否禁用了 Apple id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="58541-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="58541-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-187">Boolean</span></span>|<span data-ttu-id="58541-188">指示是否已禁用 "条款和条件" 安装窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="58541-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-189">touchIdDisabled</span></span>|<span data-ttu-id="58541-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-190">Boolean</span></span>|<span data-ttu-id="58541-191">指示是否禁用了触控 id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="58541-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-192">applePayDisabled</span></span>|<span data-ttu-id="58541-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-193">Boolean</span></span>|<span data-ttu-id="58541-194">指示是否禁用了 Apple 付费设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="58541-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-195">zoomDisabled</span></span>|<span data-ttu-id="58541-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-196">Boolean</span></span>|<span data-ttu-id="58541-197">指示是否禁用了缩放设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="58541-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-198">siriDisabled</span></span>|<span data-ttu-id="58541-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-199">Boolean</span></span>|<span data-ttu-id="58541-200">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="58541-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-201">diagnosticsDisabled</span></span>|<span data-ttu-id="58541-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-202">Boolean</span></span>|<span data-ttu-id="58541-203">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="58541-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="58541-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-205">Boolean</span></span>|<span data-ttu-id="58541-206">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-207">privacyPaneDisabled</span></span>|<span data-ttu-id="58541-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-208">Boolean</span></span>|<span data-ttu-id="58541-209">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58541-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="58541-210">iTunesPairingMode</span></span>|[<span data-ttu-id="58541-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="58541-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="58541-212">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="58541-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="58541-213">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="58541-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="58541-214">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="58541-214">managementCertificates</span></span>|<span data-ttu-id="58541-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="58541-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="58541-216">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="58541-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="58541-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="58541-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-218">Boolean</span></span>|<span data-ttu-id="58541-219">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="58541-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="58541-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="58541-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="58541-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-221">Boolean</span></span>|<span data-ttu-id="58541-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="58541-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="58541-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="58541-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="58541-224">Int32</span><span class="sxs-lookup"><span data-stu-id="58541-224">Int32</span></span>|<span data-ttu-id="58541-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="58541-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="58541-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="58541-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="58541-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="58541-227">enableSharedIPad</span></span>|<span data-ttu-id="58541-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-228">Boolean</span></span>|<span data-ttu-id="58541-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="58541-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="58541-230">仅适用于共享 ipad。</span><span class="sxs-lookup"><span data-stu-id="58541-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="58541-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="58541-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="58541-232">String</span><span class="sxs-lookup"><span data-stu-id="58541-232">String</span></span>|<span data-ttu-id="58541-233">如果设置, 则指示应使用哪种 Vpp 令牌来部署带设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="58541-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="58541-234">若要设置此属性, 必须设置 "enableAuthenticationViaCompanyPortal"。</span><span class="sxs-lookup"><span data-stu-id="58541-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="58541-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="58541-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="58541-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-236">Boolean</span></span>|<span data-ttu-id="58541-237">通知设备启用单应用模式, 并在注册过程中应用应用锁定。</span><span class="sxs-lookup"><span data-stu-id="58541-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="58541-238">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="58541-238">Default is false.</span></span> <span data-ttu-id="58541-239">若要设置此属性, 必须设置 "enableAuthenticationViaCompanyPortal" 和 "companyPortalVppTokenId"。</span><span class="sxs-lookup"><span data-stu-id="58541-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="58541-240">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="58541-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-241">Boolean</span></span>|<span data-ttu-id="58541-242">指示是否禁用 "主页按钮灵敏度" 屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="58541-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="58541-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-244">Boolean</span></span>|<span data-ttu-id="58541-245">指示是否禁用 iMessage 和 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="58541-246">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="58541-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-247">Boolean</span></span>|<span data-ttu-id="58541-248">指示是否已禁用载入安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="58541-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="58541-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-250">Boolean</span></span>|<span data-ttu-id="58541-251">指示是否禁用屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="58541-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="58541-252">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="58541-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-253">Boolean</span></span>|<span data-ttu-id="58541-254">指示是否禁用了 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="58541-255">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="58541-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-256">Boolean</span></span>|<span data-ttu-id="58541-257">指示是否禁用强制 sofware 更新屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="58541-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="58541-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="58541-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="58541-259">Boolean</span></span>|<span data-ttu-id="58541-260">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="58541-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="58541-261">响应</span><span class="sxs-lookup"><span data-stu-id="58541-261">Response</span></span>
<span data-ttu-id="58541-262">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="58541-262">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58541-263">示例</span><span class="sxs-lookup"><span data-stu-id="58541-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="58541-264">请求</span><span class="sxs-lookup"><span data-stu-id="58541-264">Request</span></span>
<span data-ttu-id="58541-265">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58541-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1736

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="58541-266">响应</span><span class="sxs-lookup"><span data-stu-id="58541-266">Response</span></span>
<span data-ttu-id="58541-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58541-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1785

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




