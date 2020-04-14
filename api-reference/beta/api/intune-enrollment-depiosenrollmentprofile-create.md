---
title: 创建 depIOSEnrollmentProfile
description: 创建新的 depIOSEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e88af42bfb50a3d2f21b35b6a1e723956e0e3881
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441472"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="6122f-103">创建 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6122f-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="6122f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6122f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6122f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6122f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6122f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6122f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6122f-107">创建新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6122f-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6122f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6122f-108">Prerequisites</span></span>
<span data-ttu-id="6122f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6122f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6122f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6122f-111">Permission type</span></span>|<span data-ttu-id="6122f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6122f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6122f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6122f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6122f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6122f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6122f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6122f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6122f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6122f-116">Not supported.</span></span>|
|<span data-ttu-id="6122f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6122f-117">Application</span></span>|<span data-ttu-id="6122f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6122f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6122f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6122f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6122f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6122f-120">Request headers</span></span>
|<span data-ttu-id="6122f-121">标头</span><span class="sxs-lookup"><span data-stu-id="6122f-121">Header</span></span>|<span data-ttu-id="6122f-122">值</span><span class="sxs-lookup"><span data-stu-id="6122f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6122f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6122f-123">Authorization</span></span>|<span data-ttu-id="6122f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6122f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6122f-125">接受</span><span class="sxs-lookup"><span data-stu-id="6122f-125">Accept</span></span>|<span data-ttu-id="6122f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6122f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6122f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6122f-127">Request body</span></span>
<span data-ttu-id="6122f-128">在请求正文中，提供 depIOSEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6122f-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="6122f-129">下表显示创建 depIOSEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6122f-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="6122f-130">属性</span><span class="sxs-lookup"><span data-stu-id="6122f-130">Property</span></span>|<span data-ttu-id="6122f-131">类型</span><span class="sxs-lookup"><span data-stu-id="6122f-131">Type</span></span>|<span data-ttu-id="6122f-132">说明</span><span class="sxs-lookup"><span data-stu-id="6122f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6122f-133">id</span><span class="sxs-lookup"><span data-stu-id="6122f-133">id</span></span>|<span data-ttu-id="6122f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6122f-134">String</span></span>|<span data-ttu-id="6122f-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="6122f-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6122f-136">displayName</span></span>|<span data-ttu-id="6122f-137">String</span><span class="sxs-lookup"><span data-stu-id="6122f-137">String</span></span>|<span data-ttu-id="6122f-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="6122f-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-139">description</span><span class="sxs-lookup"><span data-stu-id="6122f-139">description</span></span>|<span data-ttu-id="6122f-140">String</span><span class="sxs-lookup"><span data-stu-id="6122f-140">String</span></span>|<span data-ttu-id="6122f-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="6122f-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6122f-142">requiresUserAuthentication</span></span>|<span data-ttu-id="6122f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-143">Boolean</span></span>|<span data-ttu-id="6122f-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="6122f-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="6122f-145">configurationEndpointUrl</span></span>|<span data-ttu-id="6122f-146">String</span><span class="sxs-lookup"><span data-stu-id="6122f-146">String</span></span>|<span data-ttu-id="6122f-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="6122f-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6122f-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6122f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-149">Boolean</span></span>|<span data-ttu-id="6122f-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6122f-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="6122f-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6122f-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="6122f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6122f-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-153">Boolean</span></span>|<span data-ttu-id="6122f-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="6122f-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6122f-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="6122f-155">isDefault</span></span>|<span data-ttu-id="6122f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-156">Boolean</span></span>|<span data-ttu-id="6122f-157">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="6122f-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="6122f-158">supervisedModeEnabled</span></span>|<span data-ttu-id="6122f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-159">Boolean</span></span>|<span data-ttu-id="6122f-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="6122f-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="6122f-161">有关https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="6122f-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="6122f-162">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6122f-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="6122f-163">supportDepartment</span></span>|<span data-ttu-id="6122f-164">String</span><span class="sxs-lookup"><span data-stu-id="6122f-164">String</span></span>|<span data-ttu-id="6122f-165">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="6122f-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-166">passCodeDisabled</span></span>|<span data-ttu-id="6122f-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-167">Boolean</span></span>|<span data-ttu-id="6122f-168">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="6122f-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="6122f-169">isMandatory</span></span>|<span data-ttu-id="6122f-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-170">Boolean</span></span>|<span data-ttu-id="6122f-171">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="6122f-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-172">locationDisabled</span></span>|<span data-ttu-id="6122f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-173">Boolean</span></span>|<span data-ttu-id="6122f-174">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="6122f-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="6122f-175">supportPhoneNumber</span></span>|<span data-ttu-id="6122f-176">String</span><span class="sxs-lookup"><span data-stu-id="6122f-176">String</span></span>|<span data-ttu-id="6122f-177">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="6122f-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-178">profileRemovalDisabled</span></span>|<span data-ttu-id="6122f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-179">Boolean</span></span>|<span data-ttu-id="6122f-180">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="6122f-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6122f-181">restoreBlocked</span></span>|<span data-ttu-id="6122f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-182">Boolean</span></span>|<span data-ttu-id="6122f-183">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="6122f-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-184">appleIdDisabled</span></span>|<span data-ttu-id="6122f-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-185">Boolean</span></span>|<span data-ttu-id="6122f-186">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="6122f-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="6122f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-188">Boolean</span></span>|<span data-ttu-id="6122f-189">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="6122f-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-190">touchIdDisabled</span></span>|<span data-ttu-id="6122f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-191">Boolean</span></span>|<span data-ttu-id="6122f-192">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="6122f-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-193">applePayDisabled</span></span>|<span data-ttu-id="6122f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-194">Boolean</span></span>|<span data-ttu-id="6122f-195">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="6122f-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-196">zoomDisabled</span></span>|<span data-ttu-id="6122f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-197">Boolean</span></span>|<span data-ttu-id="6122f-198">指示是否禁用了缩放设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="6122f-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-199">siriDisabled</span></span>|<span data-ttu-id="6122f-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-200">Boolean</span></span>|<span data-ttu-id="6122f-201">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="6122f-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-202">diagnosticsDisabled</span></span>|<span data-ttu-id="6122f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-203">Boolean</span></span>|<span data-ttu-id="6122f-204">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="6122f-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="6122f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-206">Boolean</span></span>|<span data-ttu-id="6122f-207">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-208">privacyPaneDisabled</span></span>|<span data-ttu-id="6122f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-209">Boolean</span></span>|<span data-ttu-id="6122f-210">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-211">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="6122f-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-212">Boolean</span></span>|<span data-ttu-id="6122f-213">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="6122f-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-214">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="6122f-214">deviceNameTemplate</span></span>|<span data-ttu-id="6122f-215">String</span><span class="sxs-lookup"><span data-stu-id="6122f-215">String</span></span>|<span data-ttu-id="6122f-216">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="6122f-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="6122f-217">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6122f-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-218">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="6122f-218">configurationWebUrl</span></span>|<span data-ttu-id="6122f-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-219">Boolean</span></span>|<span data-ttu-id="6122f-220">从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="6122f-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6122f-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6122f-221">iTunesPairingMode</span></span>|[<span data-ttu-id="6122f-222">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6122f-222">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="6122f-223">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="6122f-223">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="6122f-224">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="6122f-224">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="6122f-225">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="6122f-225">managementCertificates</span></span>|<span data-ttu-id="6122f-226">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="6122f-226">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="6122f-227">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="6122f-227">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="6122f-228">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-228">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="6122f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-229">Boolean</span></span>|<span data-ttu-id="6122f-230">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="6122f-230">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="6122f-231">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="6122f-231">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="6122f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-232">Boolean</span></span>|<span data-ttu-id="6122f-233">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="6122f-233">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="6122f-234">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="6122f-234">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="6122f-235">Int32</span><span class="sxs-lookup"><span data-stu-id="6122f-235">Int32</span></span>|<span data-ttu-id="6122f-236">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="6122f-236">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="6122f-237">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="6122f-237">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="6122f-238">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="6122f-238">enableSharedIPad</span></span>|<span data-ttu-id="6122f-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-239">Boolean</span></span>|<span data-ttu-id="6122f-240">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="6122f-240">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="6122f-241">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="6122f-241">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="6122f-242">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="6122f-242">companyPortalVppTokenId</span></span>|<span data-ttu-id="6122f-243">String</span><span class="sxs-lookup"><span data-stu-id="6122f-243">String</span></span>|<span data-ttu-id="6122f-244">如果设置，则指示应使用哪种 Vpp 令牌来部署带设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="6122f-244">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="6122f-245">若要设置此属性，必须设置 "enableAuthenticationViaCompanyPortal"。</span><span class="sxs-lookup"><span data-stu-id="6122f-245">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="6122f-246">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="6122f-246">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="6122f-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-247">Boolean</span></span>|<span data-ttu-id="6122f-248">通知设备启用单应用模式，并在注册过程中应用应用锁定。</span><span class="sxs-lookup"><span data-stu-id="6122f-248">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="6122f-249">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="6122f-249">Default is false.</span></span> <span data-ttu-id="6122f-250">若要设置此属性，必须设置 "enableAuthenticationViaCompanyPortal" 和 "companyPortalVppTokenId"。</span><span class="sxs-lookup"><span data-stu-id="6122f-250">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="6122f-251">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-251">homeButtonScreenDisabled</span></span>|<span data-ttu-id="6122f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-252">Boolean</span></span>|<span data-ttu-id="6122f-253">指示是否禁用 "主页按钮灵敏度" 屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-253">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="6122f-254">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-254">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="6122f-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-255">Boolean</span></span>|<span data-ttu-id="6122f-256">指示是否禁用 iMessage 和 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-256">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="6122f-257">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-257">onBoardingScreenDisabled</span></span>|<span data-ttu-id="6122f-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-258">Boolean</span></span>|<span data-ttu-id="6122f-259">指示是否已禁用载入安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-259">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="6122f-260">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-260">simSetupScreenDisabled</span></span>|<span data-ttu-id="6122f-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-261">Boolean</span></span>|<span data-ttu-id="6122f-262">指示是否禁用了 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-262">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="6122f-263">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-263">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="6122f-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-264">Boolean</span></span>|<span data-ttu-id="6122f-265">指示是否禁用强制 sofware 更新屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-265">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="6122f-266">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-266">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="6122f-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-267">Boolean</span></span>|<span data-ttu-id="6122f-268">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-268">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="6122f-269">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-269">appearanceScreenDisabled</span></span>|<span data-ttu-id="6122f-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-270">Boolean</span></span>|<span data-ttu-id="6122f-271">指示是否禁用 Apperance 屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-271">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="6122f-272">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-272">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="6122f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-273">Boolean</span></span>|<span data-ttu-id="6122f-274">指示是否已禁用 Express 语言屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-274">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="6122f-275">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-275">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="6122f-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-276">Boolean</span></span>|<span data-ttu-id="6122f-277">指示是否禁用首选语言屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-277">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="6122f-278">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-278">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="6122f-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-279">Boolean</span></span>|<span data-ttu-id="6122f-280">指示是否禁用设备到设备迁移</span><span class="sxs-lookup"><span data-stu-id="6122f-280">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="6122f-281">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="6122f-281">welcomeScreenDisabled</span></span>|<span data-ttu-id="6122f-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="6122f-282">Boolean</span></span>|<span data-ttu-id="6122f-283">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="6122f-283">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="6122f-284">响应</span><span class="sxs-lookup"><span data-stu-id="6122f-284">Response</span></span>
<span data-ttu-id="6122f-285">如果成功，此方法在响应`201 Created`正文中返回响应代码和[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6122f-285">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6122f-286">示例</span><span class="sxs-lookup"><span data-stu-id="6122f-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="6122f-287">请求</span><span class="sxs-lookup"><span data-stu-id="6122f-287">Request</span></span>
<span data-ttu-id="6122f-288">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6122f-288">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6122f-289">响应</span><span class="sxs-lookup"><span data-stu-id="6122f-289">Response</span></span>
<span data-ttu-id="6122f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6122f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



