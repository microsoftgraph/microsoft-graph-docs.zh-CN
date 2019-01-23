---
title: 更新 depIOSEnrollmentProfile
description: 更新 depIOSEnrollmentProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e36951d69f3047c69ccfc0d1e0a72247a0715db9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400590"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="65b15-103">更新 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="65b15-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="65b15-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="65b15-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="65b15-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65b15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65b15-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65b15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65b15-107">更新[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65b15-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65b15-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="65b15-108">Prerequisites</span></span>
<span data-ttu-id="65b15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="65b15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="65b15-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65b15-111">Permission type</span></span>|<span data-ttu-id="65b15-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65b15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65b15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65b15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65b15-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b15-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65b15-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65b15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65b15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65b15-116">Not supported.</span></span>|
|<span data-ttu-id="65b15-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65b15-117">Application</span></span>|<span data-ttu-id="65b15-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="65b15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65b15-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65b15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="65b15-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65b15-120">Request headers</span></span>
|<span data-ttu-id="65b15-121">标头</span><span class="sxs-lookup"><span data-stu-id="65b15-121">Header</span></span>|<span data-ttu-id="65b15-122">值</span><span class="sxs-lookup"><span data-stu-id="65b15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65b15-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b15-123">Authorization</span></span>|<span data-ttu-id="65b15-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65b15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65b15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65b15-125">Accept</span></span>|<span data-ttu-id="65b15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65b15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b15-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65b15-127">Request body</span></span>
<span data-ttu-id="65b15-128">在请求正文中，提供[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65b15-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="65b15-129">下表显示时创建[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65b15-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="65b15-130">属性</span><span class="sxs-lookup"><span data-stu-id="65b15-130">Property</span></span>|<span data-ttu-id="65b15-131">类型</span><span class="sxs-lookup"><span data-stu-id="65b15-131">Type</span></span>|<span data-ttu-id="65b15-132">说明</span><span class="sxs-lookup"><span data-stu-id="65b15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b15-133">id</span><span class="sxs-lookup"><span data-stu-id="65b15-133">id</span></span>|<span data-ttu-id="65b15-134">String</span><span class="sxs-lookup"><span data-stu-id="65b15-134">String</span></span>|<span data-ttu-id="65b15-135">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="65b15-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-136">displayName</span><span class="sxs-lookup"><span data-stu-id="65b15-136">displayName</span></span>|<span data-ttu-id="65b15-137">String</span><span class="sxs-lookup"><span data-stu-id="65b15-137">String</span></span>|<span data-ttu-id="65b15-138">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="65b15-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-139">说明</span><span class="sxs-lookup"><span data-stu-id="65b15-139">description</span></span>|<span data-ttu-id="65b15-140">String</span><span class="sxs-lookup"><span data-stu-id="65b15-140">String</span></span>|<span data-ttu-id="65b15-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="65b15-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="65b15-142">requiresUserAuthentication</span></span>|<span data-ttu-id="65b15-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-143">Boolean</span></span>|<span data-ttu-id="65b15-144">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="65b15-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="65b15-145">configurationEndpointUrl</span></span>|<span data-ttu-id="65b15-146">String</span><span class="sxs-lookup"><span data-stu-id="65b15-146">String</span></span>|<span data-ttu-id="65b15-147">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="65b15-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="65b15-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-149">Boolean</span></span>|<span data-ttu-id="65b15-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="65b15-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="65b15-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="65b15-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="65b15-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-153">Boolean</span></span>|<span data-ttu-id="65b15-154">指示安装程序注册的助手设备继承[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) ，需要的公司门户</span><span class="sxs-lookup"><span data-stu-id="65b15-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65b15-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="65b15-155">isDefault</span></span>|<span data-ttu-id="65b15-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-156">Boolean</span></span>|<span data-ttu-id="65b15-157">指示是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的默认配置文件继承</span><span class="sxs-lookup"><span data-stu-id="65b15-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="65b15-158">supervisedModeEnabled</span></span>|<span data-ttu-id="65b15-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-159">Boolean</span></span>|<span data-ttu-id="65b15-160">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="65b15-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="65b15-161">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="65b15-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="65b15-162">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="65b15-163">supportDepartment</span></span>|<span data-ttu-id="65b15-164">String</span><span class="sxs-lookup"><span data-stu-id="65b15-164">String</span></span>|<span data-ttu-id="65b15-165">从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)支持部门信息继承</span><span class="sxs-lookup"><span data-stu-id="65b15-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-166">passCodeDisabled</span></span>|<span data-ttu-id="65b15-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-167">Boolean</span></span>|<span data-ttu-id="65b15-168">指示是否密码设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="65b15-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="65b15-169">isMandatory</span></span>|<span data-ttu-id="65b15-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-170">Boolean</span></span>|<span data-ttu-id="65b15-171">指示是否强制继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)配置文件</span><span class="sxs-lookup"><span data-stu-id="65b15-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-172">locationDisabled</span></span>|<span data-ttu-id="65b15-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-173">Boolean</span></span>|<span data-ttu-id="65b15-174">指示是否服务设置窗格中的位置禁用[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="65b15-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="65b15-175">supportPhoneNumber</span></span>|<span data-ttu-id="65b15-176">String</span><span class="sxs-lookup"><span data-stu-id="65b15-176">String</span></span>|<span data-ttu-id="65b15-177">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的电话号码继承</span><span class="sxs-lookup"><span data-stu-id="65b15-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-178">profileRemovalDisabled</span></span>|<span data-ttu-id="65b15-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-179">Boolean</span></span>|<span data-ttu-id="65b15-180">指示是否已禁用配置文件删除选项继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="65b15-181">restoreBlocked</span></span>|<span data-ttu-id="65b15-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-182">Boolean</span></span>|<span data-ttu-id="65b15-183">指示是否还原设置窗格被阻止继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-184">appleIdDisabled</span></span>|<span data-ttu-id="65b15-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-185">Boolean</span></span>|<span data-ttu-id="65b15-186">指示是否 Apple id 设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="65b15-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="65b15-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-188">Boolean</span></span>|<span data-ttu-id="65b15-189">指示是否已禁用条款和条件设置窗格继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-190">touchIdDisabled</span></span>|<span data-ttu-id="65b15-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-191">Boolean</span></span>|<span data-ttu-id="65b15-192">指示是否触摸 id 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-193">applePayDisabled</span></span>|<span data-ttu-id="65b15-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-194">Boolean</span></span>|<span data-ttu-id="65b15-195">指示是否 Apple 付薪设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-196">zoomDisabled</span></span>|<span data-ttu-id="65b15-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-197">Boolean</span></span>|<span data-ttu-id="65b15-198">指示是否缩放设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-199">siriDisabled</span></span>|<span data-ttu-id="65b15-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-200">Boolean</span></span>|<span data-ttu-id="65b15-201">指示是否 siri 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-202">diagnosticsDisabled</span></span>|<span data-ttu-id="65b15-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-203">Boolean</span></span>|<span data-ttu-id="65b15-204">指示安装程序窗格是的诊断是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="65b15-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="65b15-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-206">Boolean</span></span>|<span data-ttu-id="65b15-207">指示是否禁用 displaytone 设置屏幕继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-208">privacyPaneDisabled</span></span>|<span data-ttu-id="65b15-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-209">Boolean</span></span>|<span data-ttu-id="65b15-210">指示是否禁用隐私屏幕继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="65b15-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="65b15-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="65b15-211">iTunesPairingMode</span></span>|[<span data-ttu-id="65b15-212">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="65b15-212">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="65b15-213">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="65b15-213">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="65b15-214">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="65b15-214">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="65b15-215">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="65b15-215">managementCertificates</span></span>|<span data-ttu-id="65b15-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="65b15-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="65b15-217">Apple 配置程序的管理证书</span><span class="sxs-lookup"><span data-stu-id="65b15-217">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="65b15-218">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-218">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="65b15-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-219">Boolean</span></span>|<span data-ttu-id="65b15-220">指示是否从 Android 还原被禁用</span><span class="sxs-lookup"><span data-stu-id="65b15-220">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="65b15-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="65b15-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="65b15-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-222">Boolean</span></span>|<span data-ttu-id="65b15-223">指示是否设备需要等待配置确认</span><span class="sxs-lookup"><span data-stu-id="65b15-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="65b15-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="65b15-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="65b15-225">Int32</span><span class="sxs-lookup"><span data-stu-id="65b15-225">Int32</span></span>|<span data-ttu-id="65b15-226">此选项指定的最大可以使用共享的 iPad 的用户数。</span><span class="sxs-lookup"><span data-stu-id="65b15-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="65b15-227">仅适用于共享的 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="65b15-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="65b15-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="65b15-228">enableSharedIPad</span></span>|<span data-ttu-id="65b15-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-229">Boolean</span></span>|<span data-ttu-id="65b15-230">这指示是否要启用多用户方案模式注册设备。</span><span class="sxs-lookup"><span data-stu-id="65b15-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="65b15-231">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="65b15-231">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="65b15-232">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="65b15-232">companyPortalVppTokenId</span></span>|<span data-ttu-id="65b15-233">String</span><span class="sxs-lookup"><span data-stu-id="65b15-233">String</span></span>|<span data-ttu-id="65b15-234">如果设置，则指示用于部署具有设备许可的公司门户的 Vpp 令牌。</span><span class="sxs-lookup"><span data-stu-id="65b15-234">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="65b15-235">要设置此属性，必须设置 enableAuthenticationViaCompanyPortal。</span><span class="sxs-lookup"><span data-stu-id="65b15-235">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="65b15-236">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="65b15-236">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="65b15-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-237">Boolean</span></span>|<span data-ttu-id="65b15-238">通知要启用单个应用程序模式并应用在注册期间应用锁的设备。</span><span class="sxs-lookup"><span data-stu-id="65b15-238">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="65b15-239">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="65b15-239">Default is false.</span></span> <span data-ttu-id="65b15-240">必须为要设置此属性设置 enableAuthenticationViaCompanyPortal' 和 'companyPortalVppTokenId。</span><span class="sxs-lookup"><span data-stu-id="65b15-240">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="65b15-241">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-241">homeButtonScreenDisabled</span></span>|<span data-ttu-id="65b15-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-242">Boolean</span></span>|<span data-ttu-id="65b15-243">指示是否已禁用主页按钮敏感度屏幕</span><span class="sxs-lookup"><span data-stu-id="65b15-243">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="65b15-244">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-244">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="65b15-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-245">Boolean</span></span>|<span data-ttu-id="65b15-246">指示如果 iMessage 并禁用 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="65b15-246">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="65b15-247">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-247">onBoardingScreenDisabled</span></span>|<span data-ttu-id="65b15-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-248">Boolean</span></span>|<span data-ttu-id="65b15-249">指示是否禁用欢迎使用安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="65b15-249">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="65b15-250">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-250">screenTimeScreenDisabled</span></span>|<span data-ttu-id="65b15-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-251">Boolean</span></span>|<span data-ttu-id="65b15-252">指示是否禁用屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="65b15-252">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="65b15-253">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-253">simSetupScreenDisabled</span></span>|<span data-ttu-id="65b15-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-254">Boolean</span></span>|<span data-ttu-id="65b15-255">指示是否禁用 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="65b15-255">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="65b15-256">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-256">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="65b15-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-257">Boolean</span></span>|<span data-ttu-id="65b15-258">指示是否必需的软件更新屏幕上被禁用</span><span class="sxs-lookup"><span data-stu-id="65b15-258">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="65b15-259">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="65b15-259">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="65b15-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="65b15-260">Boolean</span></span>|<span data-ttu-id="65b15-261">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="65b15-261">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="65b15-262">响应</span><span class="sxs-lookup"><span data-stu-id="65b15-262">Response</span></span>
<span data-ttu-id="65b15-263">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65b15-263">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65b15-264">示例</span><span class="sxs-lookup"><span data-stu-id="65b15-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="65b15-265">请求</span><span class="sxs-lookup"><span data-stu-id="65b15-265">Request</span></span>
<span data-ttu-id="65b15-266">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65b15-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65b15-267">响应</span><span class="sxs-lookup"><span data-stu-id="65b15-267">Response</span></span>
<span data-ttu-id="65b15-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65b15-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




