---
title: 更新 depIOSEnrollmentProfile
description: 更新 depIOSEnrollmentProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3141aaf65cb7d7fca01cf9a9849aaed7ee310bbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533952"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="d73a5-103">更新 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d73a5-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="d73a5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d73a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d73a5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d73a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d73a5-106">更新[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d73a5-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d73a5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d73a5-107">Prerequisites</span></span>
<span data-ttu-id="d73a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d73a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d73a5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d73a5-110">Permission type</span></span>|<span data-ttu-id="d73a5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d73a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d73a5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d73a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d73a5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d73a5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d73a5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d73a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d73a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73a5-115">Not supported.</span></span>|
|<span data-ttu-id="d73a5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d73a5-116">Application</span></span>|<span data-ttu-id="d73a5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d73a5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d73a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d73a5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d73a5-119">Request headers</span></span>
|<span data-ttu-id="d73a5-120">标头</span><span class="sxs-lookup"><span data-stu-id="d73a5-120">Header</span></span>|<span data-ttu-id="d73a5-121">值</span><span class="sxs-lookup"><span data-stu-id="d73a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d73a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d73a5-122">Authorization</span></span>|<span data-ttu-id="d73a5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d73a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d73a5-124">接受</span><span class="sxs-lookup"><span data-stu-id="d73a5-124">Accept</span></span>|<span data-ttu-id="d73a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d73a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d73a5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d73a5-126">Request body</span></span>
<span data-ttu-id="d73a5-127">在请求正文中, 提供[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d73a5-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d73a5-128">下表显示创建[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d73a5-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="d73a5-129">属性</span><span class="sxs-lookup"><span data-stu-id="d73a5-129">Property</span></span>|<span data-ttu-id="d73a5-130">类型</span><span class="sxs-lookup"><span data-stu-id="d73a5-130">Type</span></span>|<span data-ttu-id="d73a5-131">说明</span><span class="sxs-lookup"><span data-stu-id="d73a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d73a5-132">id</span><span class="sxs-lookup"><span data-stu-id="d73a5-132">id</span></span>|<span data-ttu-id="d73a5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d73a5-133">String</span></span>|<span data-ttu-id="d73a5-134">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="d73a5-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d73a5-135">displayName</span></span>|<span data-ttu-id="d73a5-136">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-136">String</span></span>|<span data-ttu-id="d73a5-137">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="d73a5-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-138">description</span><span class="sxs-lookup"><span data-stu-id="d73a5-138">description</span></span>|<span data-ttu-id="d73a5-139">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-139">String</span></span>|<span data-ttu-id="d73a5-140">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="d73a5-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d73a5-141">requiresUserAuthentication</span></span>|<span data-ttu-id="d73a5-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-142">Boolean</span></span>|<span data-ttu-id="d73a5-143">指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="d73a5-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d73a5-144">configurationEndpointUrl</span></span>|<span data-ttu-id="d73a5-145">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-145">String</span></span>|<span data-ttu-id="d73a5-146">用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="d73a5-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d73a5-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d73a5-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-148">Boolean</span></span>|<span data-ttu-id="d73a5-149">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d73a5-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d73a5-150">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d73a5-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d73a5-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d73a5-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-152">Boolean</span></span>|<span data-ttu-id="d73a5-153">指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="d73a5-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d73a5-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="d73a5-154">isDefault</span></span>|<span data-ttu-id="d73a5-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="d73a5-155">Boolean</span></span>|<span data-ttu-id="d73a5-156">指示这是否是从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="d73a5-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-157">supervisedModeEnabled</span></span>|<span data-ttu-id="d73a5-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-158">Boolean</span></span>|<span data-ttu-id="d73a5-159">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="d73a5-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d73a5-160">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="d73a5-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="d73a5-161">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d73a5-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="d73a5-162">supportDepartment</span></span>|<span data-ttu-id="d73a5-163">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-163">String</span></span>|<span data-ttu-id="d73a5-164">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="d73a5-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-165">passCodeDisabled</span></span>|<span data-ttu-id="d73a5-166">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-166">Boolean</span></span>|<span data-ttu-id="d73a5-167">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="d73a5-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="d73a5-168">isMandatory</span></span>|<span data-ttu-id="d73a5-169">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-169">Boolean</span></span>|<span data-ttu-id="d73a5-170">指示是否必须从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="d73a5-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-171">locationDisabled</span></span>|<span data-ttu-id="d73a5-172">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-172">Boolean</span></span>|<span data-ttu-id="d73a5-173">指示是否禁用从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="d73a5-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d73a5-174">supportPhoneNumber</span></span>|<span data-ttu-id="d73a5-175">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-175">String</span></span>|<span data-ttu-id="d73a5-176">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="d73a5-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-177">profileRemovalDisabled</span></span>|<span data-ttu-id="d73a5-178">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-178">Boolean</span></span>|<span data-ttu-id="d73a5-179">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="d73a5-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d73a5-180">restoreBlocked</span></span>|<span data-ttu-id="d73a5-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-181">Boolean</span></span>|<span data-ttu-id="d73a5-182">指示是否阻止从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="d73a5-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-183">appleIdDisabled</span></span>|<span data-ttu-id="d73a5-184">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-184">Boolean</span></span>|<span data-ttu-id="d73a5-185">指示是否禁用了 Apple id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="d73a5-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d73a5-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-187">Boolean</span></span>|<span data-ttu-id="d73a5-188">指示是否已禁用 "条款和条件" 安装窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="d73a5-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-189">touchIdDisabled</span></span>|<span data-ttu-id="d73a5-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-190">Boolean</span></span>|<span data-ttu-id="d73a5-191">指示是否禁用了触控 id 设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="d73a5-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-192">applePayDisabled</span></span>|<span data-ttu-id="d73a5-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-193">Boolean</span></span>|<span data-ttu-id="d73a5-194">指示是否禁用了 Apple 付费设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="d73a5-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-195">zoomDisabled</span></span>|<span data-ttu-id="d73a5-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-196">Boolean</span></span>|<span data-ttu-id="d73a5-197">指示是否禁用了缩放设置窗格从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="d73a5-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-198">siriDisabled</span></span>|<span data-ttu-id="d73a5-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-199">Boolean</span></span>|<span data-ttu-id="d73a5-200">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="d73a5-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-201">diagnosticsDisabled</span></span>|<span data-ttu-id="d73a5-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-202">Boolean</span></span>|<span data-ttu-id="d73a5-203">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="d73a5-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="d73a5-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-205">Boolean</span></span>|<span data-ttu-id="d73a5-206">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-207">privacyPaneDisabled</span></span>|<span data-ttu-id="d73a5-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-208">Boolean</span></span>|<span data-ttu-id="d73a5-209">指示是否禁用了从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="d73a5-210">deviceNameTemplate</span></span>|<span data-ttu-id="d73a5-211">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-211">String</span></span>|<span data-ttu-id="d73a5-212">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="d73a5-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="d73a5-213">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d73a5-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d73a5-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d73a5-214">iTunesPairingMode</span></span>|[<span data-ttu-id="d73a5-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d73a5-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="d73a5-216">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="d73a5-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d73a5-217">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="d73a5-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d73a5-218">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="d73a5-218">managementCertificates</span></span>|<span data-ttu-id="d73a5-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="d73a5-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d73a5-220">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="d73a5-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d73a5-221">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d73a5-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-222">Boolean</span></span>|<span data-ttu-id="d73a5-223">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="d73a5-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d73a5-224">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="d73a5-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d73a5-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-225">Boolean</span></span>|<span data-ttu-id="d73a5-226">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="d73a5-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d73a5-227">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="d73a5-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d73a5-228">Int32</span><span class="sxs-lookup"><span data-stu-id="d73a5-228">Int32</span></span>|<span data-ttu-id="d73a5-229">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="d73a5-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d73a5-230">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="d73a5-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d73a5-231">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="d73a5-231">enableSharedIPad</span></span>|<span data-ttu-id="d73a5-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-232">Boolean</span></span>|<span data-ttu-id="d73a5-233">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="d73a5-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d73a5-234">仅适用于共享 ipad。</span><span class="sxs-lookup"><span data-stu-id="d73a5-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="d73a5-235">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="d73a5-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="d73a5-236">String</span><span class="sxs-lookup"><span data-stu-id="d73a5-236">String</span></span>|<span data-ttu-id="d73a5-237">如果设置, 则指示应使用哪种 Vpp 令牌来部署带设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="d73a5-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="d73a5-238">若要设置此属性, 必须设置 "enableAuthenticationViaCompanyPortal"。</span><span class="sxs-lookup"><span data-stu-id="d73a5-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="d73a5-239">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="d73a5-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="d73a5-240">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-240">Boolean</span></span>|<span data-ttu-id="d73a5-241">通知设备启用单应用模式, 并在注册过程中应用应用锁定。</span><span class="sxs-lookup"><span data-stu-id="d73a5-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="d73a5-242">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="d73a5-242">Default is false.</span></span> <span data-ttu-id="d73a5-243">若要设置此属性, 必须设置 "enableAuthenticationViaCompanyPortal" 和 "companyPortalVppTokenId"。</span><span class="sxs-lookup"><span data-stu-id="d73a5-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="d73a5-244">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="d73a5-245">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-245">Boolean</span></span>|<span data-ttu-id="d73a5-246">指示是否禁用 "主页按钮灵敏度" 屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="d73a5-247">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="d73a5-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-248">Boolean</span></span>|<span data-ttu-id="d73a5-249">指示是否禁用 iMessage 和 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="d73a5-250">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="d73a5-251">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-251">Boolean</span></span>|<span data-ttu-id="d73a5-252">指示是否已禁用载入安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="d73a5-253">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="d73a5-254">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-254">Boolean</span></span>|<span data-ttu-id="d73a5-255">指示是否禁用屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="d73a5-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="d73a5-256">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="d73a5-257">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-257">Boolean</span></span>|<span data-ttu-id="d73a5-258">指示是否禁用了 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="d73a5-259">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="d73a5-260">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-260">Boolean</span></span>|<span data-ttu-id="d73a5-261">指示是否禁用强制 sofware 更新屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="d73a5-262">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d73a5-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="d73a5-263">布尔值</span><span class="sxs-lookup"><span data-stu-id="d73a5-263">Boolean</span></span>|<span data-ttu-id="d73a5-264">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="d73a5-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="d73a5-265">响应</span><span class="sxs-lookup"><span data-stu-id="d73a5-265">Response</span></span>
<span data-ttu-id="d73a5-266">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d73a5-266">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d73a5-267">示例</span><span class="sxs-lookup"><span data-stu-id="d73a5-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="d73a5-268">请求</span><span class="sxs-lookup"><span data-stu-id="d73a5-268">Request</span></span>
<span data-ttu-id="d73a5-269">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d73a5-269">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1791

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
  "deviceNameTemplate": "Device Name Template value",
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

### <a name="response"></a><span data-ttu-id="d73a5-270">响应</span><span class="sxs-lookup"><span data-stu-id="d73a5-270">Response</span></span>
<span data-ttu-id="d73a5-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d73a5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

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
  "deviceNameTemplate": "Device Name Template value",
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





