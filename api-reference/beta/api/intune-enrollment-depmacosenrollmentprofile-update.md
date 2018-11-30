---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
ms.openlocfilehash: 7d0e7a8634d852395fd606e3053e5a2b5609e2a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048433"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="9a3ac-103">更新 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="9a3ac-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="9a3ac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a3ac-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a3ac-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a3ac-107">更新[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a3ac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a3ac-108">Prerequisites</span></span>
<span data-ttu-id="9a3ac-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9a3ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a3ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a3ac-111">Permission type</span></span>|<span data-ttu-id="9a3ac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a3ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a3ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a3ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a3ac-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a3ac-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a3ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a3ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a3ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-116">Not supported.</span></span>|
|<span data-ttu-id="9a3ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a3ac-117">Application</span></span>|<span data-ttu-id="9a3ac-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a3ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a3ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="9a3ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a3ac-120">Request headers</span></span>
|<span data-ttu-id="9a3ac-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a3ac-121">Header</span></span>|<span data-ttu-id="9a3ac-122">值</span><span class="sxs-lookup"><span data-stu-id="9a3ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a3ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a3ac-123">Authorization</span></span>|<span data-ttu-id="9a3ac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a3ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a3ac-125">Accept</span></span>|<span data-ttu-id="9a3ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a3ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a3ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a3ac-127">Request body</span></span>
<span data-ttu-id="9a3ac-128">在请求正文中，提供[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="9a3ac-129">下表显示时创建[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="9a3ac-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a3ac-130">Property</span></span>|<span data-ttu-id="9a3ac-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a3ac-131">Type</span></span>|<span data-ttu-id="9a3ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a3ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a3ac-133">id</span><span class="sxs-lookup"><span data-stu-id="9a3ac-133">id</span></span>|<span data-ttu-id="9a3ac-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9a3ac-134">String</span></span>|<span data-ttu-id="9a3ac-135">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="9a3ac-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9a3ac-136">displayName</span></span>|<span data-ttu-id="9a3ac-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9a3ac-137">String</span></span>|<span data-ttu-id="9a3ac-138">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="9a3ac-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-139">说明</span><span class="sxs-lookup"><span data-stu-id="9a3ac-139">description</span></span>|<span data-ttu-id="9a3ac-140">字符串</span><span class="sxs-lookup"><span data-stu-id="9a3ac-140">String</span></span>|<span data-ttu-id="9a3ac-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="9a3ac-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="9a3ac-142">requiresUserAuthentication</span></span>|<span data-ttu-id="9a3ac-143">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-143">Boolean</span></span>|<span data-ttu-id="9a3ac-144">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="9a3ac-145">configurationEndpointUrl</span></span>|<span data-ttu-id="9a3ac-146">字符串</span><span class="sxs-lookup"><span data-stu-id="9a3ac-146">String</span></span>|<span data-ttu-id="9a3ac-147">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="9a3ac-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="9a3ac-149">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-149">Boolean</span></span>|<span data-ttu-id="9a3ac-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="9a3ac-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="9a3ac-152">isDefault</span></span>|<span data-ttu-id="9a3ac-153">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-153">Boolean</span></span>|<span data-ttu-id="9a3ac-154">指示是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的默认配置文件继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-155">supervisedModeEnabled</span></span>|<span data-ttu-id="9a3ac-156">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-156">Boolean</span></span>|<span data-ttu-id="9a3ac-157">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="9a3ac-158">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="9a3ac-159">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="9a3ac-160">supportDepartment</span></span>|<span data-ttu-id="9a3ac-161">字符串</span><span class="sxs-lookup"><span data-stu-id="9a3ac-161">String</span></span>|<span data-ttu-id="9a3ac-162">从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)支持部门信息继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-163">passCodeDisabled</span></span>|<span data-ttu-id="9a3ac-164">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-164">Boolean</span></span>|<span data-ttu-id="9a3ac-165">指示是否密码设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="9a3ac-166">isMandatory</span></span>|<span data-ttu-id="9a3ac-167">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-167">Boolean</span></span>|<span data-ttu-id="9a3ac-168">指示是否强制继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)配置文件</span><span class="sxs-lookup"><span data-stu-id="9a3ac-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-169">locationDisabled</span></span>|<span data-ttu-id="9a3ac-170">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-170">Boolean</span></span>|<span data-ttu-id="9a3ac-171">指示是否服务设置窗格中的位置禁用[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9a3ac-172">supportPhoneNumber</span></span>|<span data-ttu-id="9a3ac-173">字符串</span><span class="sxs-lookup"><span data-stu-id="9a3ac-173">String</span></span>|<span data-ttu-id="9a3ac-174">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的电话号码继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-175">profileRemovalDisabled</span></span>|<span data-ttu-id="9a3ac-176">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-176">Boolean</span></span>|<span data-ttu-id="9a3ac-177">指示是否已禁用配置文件删除选项继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9a3ac-178">restoreBlocked</span></span>|<span data-ttu-id="9a3ac-179">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-179">Boolean</span></span>|<span data-ttu-id="9a3ac-180">指示是否还原设置窗格被阻止继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-181">appleIdDisabled</span></span>|<span data-ttu-id="9a3ac-182">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-182">Boolean</span></span>|<span data-ttu-id="9a3ac-183">指示是否 Apple id 设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="9a3ac-185">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-185">Boolean</span></span>|<span data-ttu-id="9a3ac-186">指示是否已禁用条款和条件设置窗格继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-187">touchIdDisabled</span></span>|<span data-ttu-id="9a3ac-188">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-188">Boolean</span></span>|<span data-ttu-id="9a3ac-189">指示是否触摸 id 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-190">applePayDisabled</span></span>|<span data-ttu-id="9a3ac-191">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-191">Boolean</span></span>|<span data-ttu-id="9a3ac-192">指示是否 Apple 付薪设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-193">zoomDisabled</span></span>|<span data-ttu-id="9a3ac-194">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-194">Boolean</span></span>|<span data-ttu-id="9a3ac-195">指示是否缩放设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-196">siriDisabled</span></span>|<span data-ttu-id="9a3ac-197">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-197">Boolean</span></span>|<span data-ttu-id="9a3ac-198">指示是否 siri 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ac-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-199">diagnosticsDisabled</span></span>|<span data-ttu-id="9a3ac-200">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-200">Boolean</span></span>|<span data-ttu-id="9a3ac-201">指示安装程序窗格是的诊断是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="9a3ac-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9a3ac-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-202">registrationDisabled</span></span>|<span data-ttu-id="9a3ac-203">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-203">Boolean</span></span>|<span data-ttu-id="9a3ac-204">指示已禁用注册功能</span><span class="sxs-lookup"><span data-stu-id="9a3ac-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="9a3ac-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-205">fileVaultDisabled</span></span>|<span data-ttu-id="9a3ac-206">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-206">Boolean</span></span>|<span data-ttu-id="9a3ac-207">指示是否禁用文件存储库</span><span class="sxs-lookup"><span data-stu-id="9a3ac-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="9a3ac-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="9a3ac-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="9a3ac-209">布尔</span><span class="sxs-lookup"><span data-stu-id="9a3ac-209">Boolean</span></span>|<span data-ttu-id="9a3ac-210">指示是否禁用 iCloud 分析屏幕</span><span class="sxs-lookup"><span data-stu-id="9a3ac-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="9a3ac-211">响应</span><span class="sxs-lookup"><span data-stu-id="9a3ac-211">Response</span></span>
<span data-ttu-id="9a3ac-212">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-212">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a3ac-213">示例</span><span class="sxs-lookup"><span data-stu-id="9a3ac-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a3ac-214">请求</span><span class="sxs-lookup"><span data-stu-id="9a3ac-214">Request</span></span>
<span data-ttu-id="9a3ac-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 864

{
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="9a3ac-216">响应</span><span class="sxs-lookup"><span data-stu-id="9a3ac-216">Response</span></span>
<span data-ttu-id="9a3ac-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a3ac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```





