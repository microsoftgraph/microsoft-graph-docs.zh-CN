---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3477a8634e1382c4cebd2dcc3127f0fe5eee70d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348200"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="26b3c-103">更新 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26b3c-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="26b3c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26b3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26b3c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26b3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26b3c-106">更新[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26b3c-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26b3c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="26b3c-107">Prerequisites</span></span>
<span data-ttu-id="26b3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26b3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b3c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26b3c-110">Permission type</span></span>|<span data-ttu-id="26b3c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26b3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26b3c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26b3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26b3c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b3c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26b3c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26b3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26b3c-115">Not supported.</span></span>|
|<span data-ttu-id="26b3c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="26b3c-116">Application</span></span>|<span data-ttu-id="26b3c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b3c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26b3c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26b3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="26b3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26b3c-119">Request headers</span></span>
|<span data-ttu-id="26b3c-120">标头</span><span class="sxs-lookup"><span data-stu-id="26b3c-120">Header</span></span>|<span data-ttu-id="26b3c-121">值</span><span class="sxs-lookup"><span data-stu-id="26b3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26b3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b3c-122">Authorization</span></span>|<span data-ttu-id="26b3c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26b3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26b3c-124">接受</span><span class="sxs-lookup"><span data-stu-id="26b3c-124">Accept</span></span>|<span data-ttu-id="26b3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26b3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b3c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26b3c-126">Request body</span></span>
<span data-ttu-id="26b3c-127">在请求正文中, 提供[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26b3c-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="26b3c-128">下表显示创建[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="26b3c-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="26b3c-129">属性</span><span class="sxs-lookup"><span data-stu-id="26b3c-129">Property</span></span>|<span data-ttu-id="26b3c-130">类型</span><span class="sxs-lookup"><span data-stu-id="26b3c-130">Type</span></span>|<span data-ttu-id="26b3c-131">说明</span><span class="sxs-lookup"><span data-stu-id="26b3c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26b3c-132">id</span><span class="sxs-lookup"><span data-stu-id="26b3c-132">id</span></span>|<span data-ttu-id="26b3c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="26b3c-133">String</span></span>|<span data-ttu-id="26b3c-134">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="26b3c-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="26b3c-135">displayName</span></span>|<span data-ttu-id="26b3c-136">String</span><span class="sxs-lookup"><span data-stu-id="26b3c-136">String</span></span>|<span data-ttu-id="26b3c-137">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="26b3c-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-138">说明</span><span class="sxs-lookup"><span data-stu-id="26b3c-138">description</span></span>|<span data-ttu-id="26b3c-139">String</span><span class="sxs-lookup"><span data-stu-id="26b3c-139">String</span></span>|<span data-ttu-id="26b3c-140">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="26b3c-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="26b3c-141">requiresUserAuthentication</span></span>|<span data-ttu-id="26b3c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-142">Boolean</span></span>|<span data-ttu-id="26b3c-143">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="26b3c-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="26b3c-144">configurationEndpointUrl</span></span>|<span data-ttu-id="26b3c-145">String</span><span class="sxs-lookup"><span data-stu-id="26b3c-145">String</span></span>|<span data-ttu-id="26b3c-146">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="26b3c-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="26b3c-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="26b3c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-148">Boolean</span></span>|<span data-ttu-id="26b3c-149">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="26b3c-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="26b3c-150">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="26b3c-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="26b3c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="26b3c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-152">Boolean</span></span>|<span data-ttu-id="26b3c-153">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="26b3c-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="26b3c-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="26b3c-154">isDefault</span></span>|<span data-ttu-id="26b3c-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-155">Boolean</span></span>|<span data-ttu-id="26b3c-156">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="26b3c-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-157">supervisedModeEnabled</span></span>|<span data-ttu-id="26b3c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-158">Boolean</span></span>|<span data-ttu-id="26b3c-159">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="26b3c-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="26b3c-160">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="26b3c-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="26b3c-161">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="26b3c-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="26b3c-162">supportDepartment</span></span>|<span data-ttu-id="26b3c-163">String</span><span class="sxs-lookup"><span data-stu-id="26b3c-163">String</span></span>|<span data-ttu-id="26b3c-164">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="26b3c-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-165">passCodeDisabled</span></span>|<span data-ttu-id="26b3c-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-166">Boolean</span></span>|<span data-ttu-id="26b3c-167">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="26b3c-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="26b3c-168">isMandatory</span></span>|<span data-ttu-id="26b3c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-169">Boolean</span></span>|<span data-ttu-id="26b3c-170">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="26b3c-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-171">locationDisabled</span></span>|<span data-ttu-id="26b3c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-172">Boolean</span></span>|<span data-ttu-id="26b3c-173">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="26b3c-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="26b3c-174">supportPhoneNumber</span></span>|<span data-ttu-id="26b3c-175">String</span><span class="sxs-lookup"><span data-stu-id="26b3c-175">String</span></span>|<span data-ttu-id="26b3c-176">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="26b3c-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-177">profileRemovalDisabled</span></span>|<span data-ttu-id="26b3c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-178">Boolean</span></span>|<span data-ttu-id="26b3c-179">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="26b3c-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="26b3c-180">restoreBlocked</span></span>|<span data-ttu-id="26b3c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-181">Boolean</span></span>|<span data-ttu-id="26b3c-182">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="26b3c-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-183">appleIdDisabled</span></span>|<span data-ttu-id="26b3c-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-184">Boolean</span></span>|<span data-ttu-id="26b3c-185">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="26b3c-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="26b3c-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-187">Boolean</span></span>|<span data-ttu-id="26b3c-188">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="26b3c-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-189">touchIdDisabled</span></span>|<span data-ttu-id="26b3c-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-190">Boolean</span></span>|<span data-ttu-id="26b3c-191">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="26b3c-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-192">applePayDisabled</span></span>|<span data-ttu-id="26b3c-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-193">Boolean</span></span>|<span data-ttu-id="26b3c-194">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="26b3c-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-195">zoomDisabled</span></span>|<span data-ttu-id="26b3c-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-196">Boolean</span></span>|<span data-ttu-id="26b3c-197">指示是否禁用了缩放设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="26b3c-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-198">siriDisabled</span></span>|<span data-ttu-id="26b3c-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-199">Boolean</span></span>|<span data-ttu-id="26b3c-200">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="26b3c-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-201">diagnosticsDisabled</span></span>|<span data-ttu-id="26b3c-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-202">Boolean</span></span>|<span data-ttu-id="26b3c-203">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="26b3c-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="26b3c-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-205">Boolean</span></span>|<span data-ttu-id="26b3c-206">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="26b3c-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-207">privacyPaneDisabled</span></span>|<span data-ttu-id="26b3c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-208">Boolean</span></span>|<span data-ttu-id="26b3c-209">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="26b3c-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="26b3c-210">deviceNameTemplate</span></span>|<span data-ttu-id="26b3c-211">String</span><span class="sxs-lookup"><span data-stu-id="26b3c-211">String</span></span>|<span data-ttu-id="26b3c-212">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="26b3c-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="26b3c-213">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="26b3c-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="26b3c-214">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-214">registrationDisabled</span></span>|<span data-ttu-id="26b3c-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-215">Boolean</span></span>|<span data-ttu-id="26b3c-216">指示是否禁用注册</span><span class="sxs-lookup"><span data-stu-id="26b3c-216">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="26b3c-217">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-217">fileVaultDisabled</span></span>|<span data-ttu-id="26b3c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-218">Boolean</span></span>|<span data-ttu-id="26b3c-219">指示是否禁用了文件电子仓库</span><span class="sxs-lookup"><span data-stu-id="26b3c-219">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="26b3c-220">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-220">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="26b3c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-221">Boolean</span></span>|<span data-ttu-id="26b3c-222">指示是否禁用了 iCloud 分析屏幕</span><span class="sxs-lookup"><span data-stu-id="26b3c-222">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="26b3c-223">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-223">iCloudStorageDisabled</span></span>|<span data-ttu-id="26b3c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-224">Boolean</span></span>|<span data-ttu-id="26b3c-225">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="26b3c-225">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="26b3c-226">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="26b3c-226">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="26b3c-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b3c-227">Boolean</span></span>|<span data-ttu-id="26b3c-228">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="26b3c-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="26b3c-229">响应</span><span class="sxs-lookup"><span data-stu-id="26b3c-229">Response</span></span>
<span data-ttu-id="26b3c-230">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26b3c-230">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26b3c-231">示例</span><span class="sxs-lookup"><span data-stu-id="26b3c-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="26b3c-232">请求</span><span class="sxs-lookup"><span data-stu-id="26b3c-232">Request</span></span>
<span data-ttu-id="26b3c-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26b3c-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="26b3c-234">响应</span><span class="sxs-lookup"><span data-stu-id="26b3c-234">Response</span></span>
<span data-ttu-id="26b3c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26b3c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1240

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```






