---
title: 创建 depIOSEnrollmentProfile
description: 创建新的 depIOSEnrollmentProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8afb06dcb52305cd3c2434ed37c3c5e7f5c6617f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536067"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="c99fc-103">创建 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c99fc-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="c99fc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c99fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c99fc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c99fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c99fc-106">创建新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c99fc-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c99fc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c99fc-107">Prerequisites</span></span>
<span data-ttu-id="c99fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c99fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c99fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c99fc-110">Permission type</span></span>|<span data-ttu-id="c99fc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c99fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c99fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c99fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c99fc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99fc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c99fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c99fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c99fc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c99fc-115">Not supported.</span></span>|
|<span data-ttu-id="c99fc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c99fc-116">Application</span></span>|<span data-ttu-id="c99fc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99fc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c99fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c99fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c99fc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c99fc-119">Request headers</span></span>
|<span data-ttu-id="c99fc-120">标头</span><span class="sxs-lookup"><span data-stu-id="c99fc-120">Header</span></span>|<span data-ttu-id="c99fc-121">值</span><span class="sxs-lookup"><span data-stu-id="c99fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c99fc-122">授权</span><span class="sxs-lookup"><span data-stu-id="c99fc-122">Authorization</span></span>|<span data-ttu-id="c99fc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c99fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c99fc-124">接受</span><span class="sxs-lookup"><span data-stu-id="c99fc-124">Accept</span></span>|<span data-ttu-id="c99fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c99fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c99fc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c99fc-126">Request body</span></span>
<span data-ttu-id="c99fc-127">在请求正文中，提供 depIOSEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c99fc-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="c99fc-128">下表显示创建 depIOSEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c99fc-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="c99fc-129">属性</span><span class="sxs-lookup"><span data-stu-id="c99fc-129">Property</span></span>|<span data-ttu-id="c99fc-130">类型</span><span class="sxs-lookup"><span data-stu-id="c99fc-130">Type</span></span>|<span data-ttu-id="c99fc-131">说明</span><span class="sxs-lookup"><span data-stu-id="c99fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c99fc-132">id</span><span class="sxs-lookup"><span data-stu-id="c99fc-132">id</span></span>|<span data-ttu-id="c99fc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fc-133">String</span></span>|<span data-ttu-id="c99fc-134">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="c99fc-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c99fc-135">displayName</span></span>|<span data-ttu-id="c99fc-136">String</span><span class="sxs-lookup"><span data-stu-id="c99fc-136">String</span></span>|<span data-ttu-id="c99fc-137">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="c99fc-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-138">说明</span><span class="sxs-lookup"><span data-stu-id="c99fc-138">description</span></span>|<span data-ttu-id="c99fc-139">String</span><span class="sxs-lookup"><span data-stu-id="c99fc-139">String</span></span>|<span data-ttu-id="c99fc-140">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="c99fc-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="c99fc-141">requiresUserAuthentication</span></span>|<span data-ttu-id="c99fc-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-142">Boolean</span></span>|<span data-ttu-id="c99fc-143">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="c99fc-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="c99fc-144">configurationEndpointUrl</span></span>|<span data-ttu-id="c99fc-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fc-145">String</span></span>|<span data-ttu-id="c99fc-146">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="c99fc-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c99fc-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c99fc-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-148">Boolean</span></span>|<span data-ttu-id="c99fc-149">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="c99fc-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="c99fc-150">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c99fc-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="c99fc-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="c99fc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-152">Boolean</span></span>|<span data-ttu-id="c99fc-153">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="c99fc-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c99fc-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="c99fc-154">isDefault</span></span>|<span data-ttu-id="c99fc-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-155">Boolean</span></span>|<span data-ttu-id="c99fc-156">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="c99fc-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-157">supervisedModeEnabled</span></span>|<span data-ttu-id="c99fc-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-158">Boolean</span></span>|<span data-ttu-id="c99fc-159">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="c99fc-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="c99fc-160">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="c99fc-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="c99fc-161">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c99fc-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="c99fc-162">supportDepartment</span></span>|<span data-ttu-id="c99fc-163">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fc-163">String</span></span>|<span data-ttu-id="c99fc-164">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="c99fc-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-165">passCodeDisabled</span></span>|<span data-ttu-id="c99fc-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-166">Boolean</span></span>|<span data-ttu-id="c99fc-167">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="c99fc-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="c99fc-168">isMandatory</span></span>|<span data-ttu-id="c99fc-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-169">Boolean</span></span>|<span data-ttu-id="c99fc-170">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="c99fc-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-171">locationDisabled</span></span>|<span data-ttu-id="c99fc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-172">Boolean</span></span>|<span data-ttu-id="c99fc-173">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="c99fc-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c99fc-174">supportPhoneNumber</span></span>|<span data-ttu-id="c99fc-175">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fc-175">String</span></span>|<span data-ttu-id="c99fc-176">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="c99fc-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-177">profileRemovalDisabled</span></span>|<span data-ttu-id="c99fc-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-178">Boolean</span></span>|<span data-ttu-id="c99fc-179">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="c99fc-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c99fc-180">restoreBlocked</span></span>|<span data-ttu-id="c99fc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-181">Boolean</span></span>|<span data-ttu-id="c99fc-182">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="c99fc-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-183">appleIdDisabled</span></span>|<span data-ttu-id="c99fc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-184">Boolean</span></span>|<span data-ttu-id="c99fc-185">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="c99fc-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="c99fc-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-187">Boolean</span></span>|<span data-ttu-id="c99fc-188">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="c99fc-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-189">touchIdDisabled</span></span>|<span data-ttu-id="c99fc-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-190">Boolean</span></span>|<span data-ttu-id="c99fc-191">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="c99fc-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-192">applePayDisabled</span></span>|<span data-ttu-id="c99fc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-193">Boolean</span></span>|<span data-ttu-id="c99fc-194">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="c99fc-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-195">zoomDisabled</span></span>|<span data-ttu-id="c99fc-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-196">Boolean</span></span>|<span data-ttu-id="c99fc-197">指示是否禁用了缩放设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="c99fc-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-198">siriDisabled</span></span>|<span data-ttu-id="c99fc-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-199">Boolean</span></span>|<span data-ttu-id="c99fc-200">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="c99fc-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-201">diagnosticsDisabled</span></span>|<span data-ttu-id="c99fc-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-202">Boolean</span></span>|<span data-ttu-id="c99fc-203">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="c99fc-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="c99fc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-205">Boolean</span></span>|<span data-ttu-id="c99fc-206">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-207">privacyPaneDisabled</span></span>|<span data-ttu-id="c99fc-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-208">Boolean</span></span>|<span data-ttu-id="c99fc-209">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-210">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="c99fc-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-211">Boolean</span></span>|<span data-ttu-id="c99fc-212">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="c99fc-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-213">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="c99fc-213">deviceNameTemplate</span></span>|<span data-ttu-id="c99fc-214">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fc-214">String</span></span>|<span data-ttu-id="c99fc-215">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="c99fc-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="c99fc-216">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c99fc-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-217">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="c99fc-217">configurationWebUrl</span></span>|<span data-ttu-id="c99fc-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-218">Boolean</span></span>|<span data-ttu-id="c99fc-219">从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="c99fc-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="c99fc-220">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="c99fc-220">iTunesPairingMode</span></span>|[<span data-ttu-id="c99fc-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="c99fc-221">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="c99fc-222">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="c99fc-222">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="c99fc-223">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="c99fc-223">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="c99fc-224">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="c99fc-224">managementCertificates</span></span>|<span data-ttu-id="c99fc-225">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="c99fc-225">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="c99fc-226">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="c99fc-226">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="c99fc-227">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-227">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="c99fc-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-228">Boolean</span></span>|<span data-ttu-id="c99fc-229">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="c99fc-229">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="c99fc-230">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="c99fc-230">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="c99fc-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-231">Boolean</span></span>|<span data-ttu-id="c99fc-232">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="c99fc-232">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="c99fc-233">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="c99fc-233">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="c99fc-234">Int32</span><span class="sxs-lookup"><span data-stu-id="c99fc-234">Int32</span></span>|<span data-ttu-id="c99fc-235">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="c99fc-235">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="c99fc-236">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="c99fc-236">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="c99fc-237">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="c99fc-237">enableSharedIPad</span></span>|<span data-ttu-id="c99fc-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-238">Boolean</span></span>|<span data-ttu-id="c99fc-239">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="c99fc-239">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="c99fc-240">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="c99fc-240">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="c99fc-241">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="c99fc-241">companyPortalVppTokenId</span></span>|<span data-ttu-id="c99fc-242">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fc-242">String</span></span>|<span data-ttu-id="c99fc-243">如果设置，则指示应使用哪种 Vpp 令牌来部署带设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="c99fc-243">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="c99fc-244">若要设置此属性，必须设置 "enableAuthenticationViaCompanyPortal"。</span><span class="sxs-lookup"><span data-stu-id="c99fc-244">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="c99fc-245">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="c99fc-245">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="c99fc-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-246">Boolean</span></span>|<span data-ttu-id="c99fc-247">通知设备启用单应用模式，并在注册过程中应用应用锁定。</span><span class="sxs-lookup"><span data-stu-id="c99fc-247">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="c99fc-248">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="c99fc-248">Default is false.</span></span> <span data-ttu-id="c99fc-249">若要设置此属性，必须设置 "enableAuthenticationViaCompanyPortal" 和 "companyPortalVppTokenId"。</span><span class="sxs-lookup"><span data-stu-id="c99fc-249">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="c99fc-250">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-250">homeButtonScreenDisabled</span></span>|<span data-ttu-id="c99fc-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-251">Boolean</span></span>|<span data-ttu-id="c99fc-252">指示是否禁用 "主页按钮灵敏度" 屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-252">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="c99fc-253">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-253">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="c99fc-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-254">Boolean</span></span>|<span data-ttu-id="c99fc-255">指示是否禁用 iMessage 和 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-255">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="c99fc-256">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-256">onBoardingScreenDisabled</span></span>|<span data-ttu-id="c99fc-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-257">Boolean</span></span>|<span data-ttu-id="c99fc-258">指示是否已禁用载入安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-258">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="c99fc-259">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-259">simSetupScreenDisabled</span></span>|<span data-ttu-id="c99fc-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-260">Boolean</span></span>|<span data-ttu-id="c99fc-261">指示是否禁用了 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-261">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="c99fc-262">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-262">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="c99fc-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-263">Boolean</span></span>|<span data-ttu-id="c99fc-264">指示是否禁用强制 sofware 更新屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-264">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="c99fc-265">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-265">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="c99fc-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-266">Boolean</span></span>|<span data-ttu-id="c99fc-267">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-267">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="c99fc-268">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-268">appearanceScreenDisabled</span></span>|<span data-ttu-id="c99fc-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-269">Boolean</span></span>|<span data-ttu-id="c99fc-270">指示是否禁用 Apperance 屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-270">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="c99fc-271">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-271">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="c99fc-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-272">Boolean</span></span>|<span data-ttu-id="c99fc-273">指示是否已禁用 Express 语言屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-273">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="c99fc-274">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-274">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="c99fc-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-275">Boolean</span></span>|<span data-ttu-id="c99fc-276">指示是否禁用首选语言屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-276">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="c99fc-277">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-277">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="c99fc-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-278">Boolean</span></span>|<span data-ttu-id="c99fc-279">指示是否禁用设备到设备迁移</span><span class="sxs-lookup"><span data-stu-id="c99fc-279">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="c99fc-280">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="c99fc-280">welcomeScreenDisabled</span></span>|<span data-ttu-id="c99fc-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fc-281">Boolean</span></span>|<span data-ttu-id="c99fc-282">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="c99fc-282">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="c99fc-283">响应</span><span class="sxs-lookup"><span data-stu-id="c99fc-283">Response</span></span>
<span data-ttu-id="c99fc-284">如果成功，此方法在响应`201 Created`正文中返回响应代码和[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c99fc-284">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c99fc-285">示例</span><span class="sxs-lookup"><span data-stu-id="c99fc-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="c99fc-286">请求</span><span class="sxs-lookup"><span data-stu-id="c99fc-286">Request</span></span>
<span data-ttu-id="c99fc-287">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c99fc-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2024

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
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
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="c99fc-288">响应</span><span class="sxs-lookup"><span data-stu-id="c99fc-288">Response</span></span>
<span data-ttu-id="c99fc-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c99fc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2073

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
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
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true
}
```






