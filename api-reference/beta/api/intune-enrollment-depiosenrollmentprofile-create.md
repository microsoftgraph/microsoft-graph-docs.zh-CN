---
title: 创建 depIOSEnrollmentProfile
description: 创建新的 depIOSEnrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e251217a568ffe0c3e25940ab8300565929861b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174219"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="3d31e-103">创建 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3d31e-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="3d31e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d31e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d31e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d31e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d31e-106">创建新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d31e-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d31e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d31e-107">Prerequisites</span></span>
<span data-ttu-id="3d31e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3d31e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d31e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d31e-110">Permission type</span></span>|<span data-ttu-id="3d31e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d31e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d31e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d31e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d31e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d31e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d31e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d31e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d31e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d31e-115">Not supported.</span></span>|
|<span data-ttu-id="3d31e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d31e-116">Application</span></span>|<span data-ttu-id="3d31e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d31e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d31e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d31e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3d31e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d31e-119">Request headers</span></span>
|<span data-ttu-id="3d31e-120">标头</span><span class="sxs-lookup"><span data-stu-id="3d31e-120">Header</span></span>|<span data-ttu-id="3d31e-121">值</span><span class="sxs-lookup"><span data-stu-id="3d31e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d31e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d31e-122">Authorization</span></span>|<span data-ttu-id="3d31e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d31e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d31e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3d31e-124">Accept</span></span>|<span data-ttu-id="3d31e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d31e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d31e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d31e-126">Request body</span></span>
<span data-ttu-id="3d31e-127">在请求正文中, 提供 depIOSEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d31e-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="3d31e-128">下表显示创建 depIOSEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d31e-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="3d31e-129">属性</span><span class="sxs-lookup"><span data-stu-id="3d31e-129">Property</span></span>|<span data-ttu-id="3d31e-130">类型</span><span class="sxs-lookup"><span data-stu-id="3d31e-130">Type</span></span>|<span data-ttu-id="3d31e-131">说明</span><span class="sxs-lookup"><span data-stu-id="3d31e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d31e-132">id</span><span class="sxs-lookup"><span data-stu-id="3d31e-132">id</span></span>|<span data-ttu-id="3d31e-133">String</span><span class="sxs-lookup"><span data-stu-id="3d31e-133">String</span></span>|<span data-ttu-id="3d31e-134">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="3d31e-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3d31e-135">displayName</span></span>|<span data-ttu-id="3d31e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3d31e-136">String</span></span>|<span data-ttu-id="3d31e-137">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="3d31e-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-138">说明</span><span class="sxs-lookup"><span data-stu-id="3d31e-138">description</span></span>|<span data-ttu-id="3d31e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="3d31e-139">String</span></span>|<span data-ttu-id="3d31e-140">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="3d31e-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="3d31e-141">requiresUserAuthentication</span></span>|<span data-ttu-id="3d31e-142">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-142">Boolean</span></span>|<span data-ttu-id="3d31e-143">指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="3d31e-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="3d31e-144">configurationEndpointUrl</span></span>|<span data-ttu-id="3d31e-145">字符串</span><span class="sxs-lookup"><span data-stu-id="3d31e-145">String</span></span>|<span data-ttu-id="3d31e-146">用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="3d31e-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="3d31e-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="3d31e-148">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-148">Boolean</span></span>|<span data-ttu-id="3d31e-149">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="3d31e-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="3d31e-150">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3d31e-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="3d31e-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="3d31e-152">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-152">Boolean</span></span>|<span data-ttu-id="3d31e-153">指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="3d31e-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3d31e-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="3d31e-154">isDefault</span></span>|<span data-ttu-id="3d31e-155">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-155">Boolean</span></span>|<span data-ttu-id="3d31e-156">指示这是否是从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="3d31e-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-157">supervisedModeEnabled</span></span>|<span data-ttu-id="3d31e-158">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-158">Boolean</span></span>|<span data-ttu-id="3d31e-159">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="3d31e-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="3d31e-160">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="3d31e-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="3d31e-161">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3d31e-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="3d31e-162">supportDepartment</span></span>|<span data-ttu-id="3d31e-163">字符串</span><span class="sxs-lookup"><span data-stu-id="3d31e-163">String</span></span>|<span data-ttu-id="3d31e-164">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="3d31e-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-165">passCodeDisabled</span></span>|<span data-ttu-id="3d31e-166">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-166">Boolean</span></span>|<span data-ttu-id="3d31e-167">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="3d31e-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="3d31e-168">isMandatory</span></span>|<span data-ttu-id="3d31e-169">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-169">Boolean</span></span>|<span data-ttu-id="3d31e-170">指示是否必须从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="3d31e-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-171">locationDisabled</span></span>|<span data-ttu-id="3d31e-172">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-172">Boolean</span></span>|<span data-ttu-id="3d31e-173">指示是否禁用从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="3d31e-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3d31e-174">supportPhoneNumber</span></span>|<span data-ttu-id="3d31e-175">字符串</span><span class="sxs-lookup"><span data-stu-id="3d31e-175">String</span></span>|<span data-ttu-id="3d31e-176">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="3d31e-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-177">profileRemovalDisabled</span></span>|<span data-ttu-id="3d31e-178">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-178">Boolean</span></span>|<span data-ttu-id="3d31e-179">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="3d31e-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3d31e-180">restoreBlocked</span></span>|<span data-ttu-id="3d31e-181">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-181">Boolean</span></span>|<span data-ttu-id="3d31e-182">指示是否阻止从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="3d31e-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-183">appleIdDisabled</span></span>|<span data-ttu-id="3d31e-184">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-184">Boolean</span></span>|<span data-ttu-id="3d31e-185">指示是否禁用了 Apple id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="3d31e-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="3d31e-187">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-187">Boolean</span></span>|<span data-ttu-id="3d31e-188">指示是否已禁用 "条款和条件" 安装窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="3d31e-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-189">touchIdDisabled</span></span>|<span data-ttu-id="3d31e-190">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-190">Boolean</span></span>|<span data-ttu-id="3d31e-191">指示是否禁用了触控 id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="3d31e-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-192">applePayDisabled</span></span>|<span data-ttu-id="3d31e-193">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-193">Boolean</span></span>|<span data-ttu-id="3d31e-194">指示是否禁用了 Apple 付费设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="3d31e-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-195">zoomDisabled</span></span>|<span data-ttu-id="3d31e-196">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-196">Boolean</span></span>|<span data-ttu-id="3d31e-197">指示是否禁用了缩放设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="3d31e-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-198">siriDisabled</span></span>|<span data-ttu-id="3d31e-199">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-199">Boolean</span></span>|<span data-ttu-id="3d31e-200">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="3d31e-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-201">diagnosticsDisabled</span></span>|<span data-ttu-id="3d31e-202">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-202">Boolean</span></span>|<span data-ttu-id="3d31e-203">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="3d31e-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="3d31e-205">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-205">Boolean</span></span>|<span data-ttu-id="3d31e-206">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-207">privacyPaneDisabled</span></span>|<span data-ttu-id="3d31e-208">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-208">Boolean</span></span>|<span data-ttu-id="3d31e-209">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="3d31e-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="3d31e-210">iTunesPairingMode</span></span>|[<span data-ttu-id="3d31e-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="3d31e-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="3d31e-212">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="3d31e-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="3d31e-213">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="3d31e-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="3d31e-214">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="3d31e-214">managementCertificates</span></span>|<span data-ttu-id="3d31e-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="3d31e-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="3d31e-216">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="3d31e-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="3d31e-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="3d31e-218">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-218">Boolean</span></span>|<span data-ttu-id="3d31e-219">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="3d31e-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="3d31e-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="3d31e-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="3d31e-221">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-221">Boolean</span></span>|<span data-ttu-id="3d31e-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="3d31e-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="3d31e-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="3d31e-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="3d31e-224">Int32</span><span class="sxs-lookup"><span data-stu-id="3d31e-224">Int32</span></span>|<span data-ttu-id="3d31e-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="3d31e-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="3d31e-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="3d31e-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="3d31e-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="3d31e-227">enableSharedIPad</span></span>|<span data-ttu-id="3d31e-228">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-228">Boolean</span></span>|<span data-ttu-id="3d31e-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="3d31e-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="3d31e-230">仅适用于共享 ipad。</span><span class="sxs-lookup"><span data-stu-id="3d31e-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="3d31e-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="3d31e-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="3d31e-232">字符串</span><span class="sxs-lookup"><span data-stu-id="3d31e-232">String</span></span>|<span data-ttu-id="3d31e-233">如果设置, 则指示应使用哪种 Vpp 令牌来部署带设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="3d31e-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="3d31e-234">若要设置此属性, 必须设置 "enableAuthenticationViaCompanyPortal"。</span><span class="sxs-lookup"><span data-stu-id="3d31e-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="3d31e-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="3d31e-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="3d31e-236">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-236">Boolean</span></span>|<span data-ttu-id="3d31e-237">通知设备启用单应用模式, 并在注册过程中应用应用锁定。</span><span class="sxs-lookup"><span data-stu-id="3d31e-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="3d31e-238">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="3d31e-238">Default is false.</span></span> <span data-ttu-id="3d31e-239">若要设置此属性, 必须设置 "enableAuthenticationViaCompanyPortal" 和 "companyPortalVppTokenId"。</span><span class="sxs-lookup"><span data-stu-id="3d31e-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="3d31e-240">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="3d31e-241">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-241">Boolean</span></span>|<span data-ttu-id="3d31e-242">指示是否禁用 "主页按钮灵敏度" 屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="3d31e-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="3d31e-244">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-244">Boolean</span></span>|<span data-ttu-id="3d31e-245">指示是否禁用 iMessage 和 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="3d31e-246">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="3d31e-247">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-247">Boolean</span></span>|<span data-ttu-id="3d31e-248">指示是否已禁用载入安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="3d31e-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="3d31e-250">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-250">Boolean</span></span>|<span data-ttu-id="3d31e-251">指示是否禁用屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="3d31e-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="3d31e-252">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="3d31e-253">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-253">Boolean</span></span>|<span data-ttu-id="3d31e-254">指示是否禁用了 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="3d31e-255">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="3d31e-256">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-256">Boolean</span></span>|<span data-ttu-id="3d31e-257">指示是否禁用强制 sofware 更新屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="3d31e-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="3d31e-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="3d31e-259">布尔</span><span class="sxs-lookup"><span data-stu-id="3d31e-259">Boolean</span></span>|<span data-ttu-id="3d31e-260">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="3d31e-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="3d31e-261">响应</span><span class="sxs-lookup"><span data-stu-id="3d31e-261">Response</span></span>
<span data-ttu-id="3d31e-262">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d31e-262">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d31e-263">示例</span><span class="sxs-lookup"><span data-stu-id="3d31e-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d31e-264">请求</span><span class="sxs-lookup"><span data-stu-id="3d31e-264">Request</span></span>
<span data-ttu-id="3d31e-265">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d31e-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="3d31e-266">响应</span><span class="sxs-lookup"><span data-stu-id="3d31e-266">Response</span></span>
<span data-ttu-id="3d31e-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d31e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




