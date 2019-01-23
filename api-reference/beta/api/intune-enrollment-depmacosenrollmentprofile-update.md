---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f86e520160e988e72aaa2473b256613a997cae0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420113"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="d8ffb-103">更新 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d8ffb-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="d8ffb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8ffb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8ffb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8ffb-107">更新[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8ffb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8ffb-108">Prerequisites</span></span>
<span data-ttu-id="d8ffb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8ffb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8ffb-111">Permission type</span></span>|<span data-ttu-id="d8ffb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8ffb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8ffb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8ffb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8ffb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ffb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8ffb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8ffb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8ffb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-116">Not supported.</span></span>|
|<span data-ttu-id="d8ffb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8ffb-117">Application</span></span>|<span data-ttu-id="d8ffb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ffb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8ffb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d8ffb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8ffb-120">Request headers</span></span>
|<span data-ttu-id="d8ffb-121">标头</span><span class="sxs-lookup"><span data-stu-id="d8ffb-121">Header</span></span>|<span data-ttu-id="d8ffb-122">值</span><span class="sxs-lookup"><span data-stu-id="d8ffb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8ffb-123">授权</span><span class="sxs-lookup"><span data-stu-id="d8ffb-123">Authorization</span></span>|<span data-ttu-id="d8ffb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8ffb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8ffb-125">Accept</span></span>|<span data-ttu-id="d8ffb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ffb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ffb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8ffb-127">Request body</span></span>
<span data-ttu-id="d8ffb-128">在请求正文中，提供[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d8ffb-129">下表显示时创建[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="d8ffb-130">属性</span><span class="sxs-lookup"><span data-stu-id="d8ffb-130">Property</span></span>|<span data-ttu-id="d8ffb-131">类型</span><span class="sxs-lookup"><span data-stu-id="d8ffb-131">Type</span></span>|<span data-ttu-id="d8ffb-132">说明</span><span class="sxs-lookup"><span data-stu-id="d8ffb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ffb-133">id</span><span class="sxs-lookup"><span data-stu-id="d8ffb-133">id</span></span>|<span data-ttu-id="d8ffb-134">String</span><span class="sxs-lookup"><span data-stu-id="d8ffb-134">String</span></span>|<span data-ttu-id="d8ffb-135">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="d8ffb-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d8ffb-136">displayName</span></span>|<span data-ttu-id="d8ffb-137">String</span><span class="sxs-lookup"><span data-stu-id="d8ffb-137">String</span></span>|<span data-ttu-id="d8ffb-138">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="d8ffb-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-139">说明</span><span class="sxs-lookup"><span data-stu-id="d8ffb-139">description</span></span>|<span data-ttu-id="d8ffb-140">String</span><span class="sxs-lookup"><span data-stu-id="d8ffb-140">String</span></span>|<span data-ttu-id="d8ffb-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="d8ffb-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d8ffb-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d8ffb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-143">Boolean</span></span>|<span data-ttu-id="d8ffb-144">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d8ffb-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d8ffb-146">String</span><span class="sxs-lookup"><span data-stu-id="d8ffb-146">String</span></span>|<span data-ttu-id="d8ffb-147">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d8ffb-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d8ffb-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-149">Boolean</span></span>|<span data-ttu-id="d8ffb-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d8ffb-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d8ffb-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d8ffb-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-153">Boolean</span></span>|<span data-ttu-id="d8ffb-154">指示安装程序注册的助手设备继承[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) ，需要的公司门户</span><span class="sxs-lookup"><span data-stu-id="d8ffb-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="d8ffb-155">isDefault</span></span>|<span data-ttu-id="d8ffb-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-156">Boolean</span></span>|<span data-ttu-id="d8ffb-157">指示是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的默认配置文件继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-158">supervisedModeEnabled</span></span>|<span data-ttu-id="d8ffb-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-159">Boolean</span></span>|<span data-ttu-id="d8ffb-160">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d8ffb-161">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="d8ffb-162">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="d8ffb-163">supportDepartment</span></span>|<span data-ttu-id="d8ffb-164">String</span><span class="sxs-lookup"><span data-stu-id="d8ffb-164">String</span></span>|<span data-ttu-id="d8ffb-165">从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)支持部门信息继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-166">passCodeDisabled</span></span>|<span data-ttu-id="d8ffb-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-167">Boolean</span></span>|<span data-ttu-id="d8ffb-168">指示是否密码设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="d8ffb-169">isMandatory</span></span>|<span data-ttu-id="d8ffb-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-170">Boolean</span></span>|<span data-ttu-id="d8ffb-171">指示是否强制继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)配置文件</span><span class="sxs-lookup"><span data-stu-id="d8ffb-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-172">locationDisabled</span></span>|<span data-ttu-id="d8ffb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-173">Boolean</span></span>|<span data-ttu-id="d8ffb-174">指示是否服务设置窗格中的位置禁用[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d8ffb-175">supportPhoneNumber</span></span>|<span data-ttu-id="d8ffb-176">String</span><span class="sxs-lookup"><span data-stu-id="d8ffb-176">String</span></span>|<span data-ttu-id="d8ffb-177">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的电话号码继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-178">profileRemovalDisabled</span></span>|<span data-ttu-id="d8ffb-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-179">Boolean</span></span>|<span data-ttu-id="d8ffb-180">指示是否已禁用配置文件删除选项继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d8ffb-181">restoreBlocked</span></span>|<span data-ttu-id="d8ffb-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-182">Boolean</span></span>|<span data-ttu-id="d8ffb-183">指示是否还原设置窗格被阻止继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-184">appleIdDisabled</span></span>|<span data-ttu-id="d8ffb-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-185">Boolean</span></span>|<span data-ttu-id="d8ffb-186">指示是否 Apple id 设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d8ffb-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-188">Boolean</span></span>|<span data-ttu-id="d8ffb-189">指示是否已禁用条款和条件设置窗格继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-190">touchIdDisabled</span></span>|<span data-ttu-id="d8ffb-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-191">Boolean</span></span>|<span data-ttu-id="d8ffb-192">指示是否触摸 id 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-193">applePayDisabled</span></span>|<span data-ttu-id="d8ffb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-194">Boolean</span></span>|<span data-ttu-id="d8ffb-195">指示是否 Apple 付薪设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-196">zoomDisabled</span></span>|<span data-ttu-id="d8ffb-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-197">Boolean</span></span>|<span data-ttu-id="d8ffb-198">指示是否缩放设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-199">siriDisabled</span></span>|<span data-ttu-id="d8ffb-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-200">Boolean</span></span>|<span data-ttu-id="d8ffb-201">指示是否 siri 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-202">diagnosticsDisabled</span></span>|<span data-ttu-id="d8ffb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-203">Boolean</span></span>|<span data-ttu-id="d8ffb-204">指示安装程序窗格是的诊断是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="d8ffb-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="d8ffb-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-206">Boolean</span></span>|<span data-ttu-id="d8ffb-207">指示是否禁用 displaytone 设置屏幕继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-208">privacyPaneDisabled</span></span>|<span data-ttu-id="d8ffb-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-209">Boolean</span></span>|<span data-ttu-id="d8ffb-210">指示是否禁用隐私屏幕继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8ffb-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d8ffb-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-211">registrationDisabled</span></span>|<span data-ttu-id="d8ffb-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-212">Boolean</span></span>|<span data-ttu-id="d8ffb-213">指示已禁用注册功能</span><span class="sxs-lookup"><span data-stu-id="d8ffb-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="d8ffb-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-214">fileVaultDisabled</span></span>|<span data-ttu-id="d8ffb-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-215">Boolean</span></span>|<span data-ttu-id="d8ffb-216">指示是否禁用文件存储库</span><span class="sxs-lookup"><span data-stu-id="d8ffb-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="d8ffb-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d8ffb-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="d8ffb-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ffb-218">Boolean</span></span>|<span data-ttu-id="d8ffb-219">指示是否禁用 iCloud 分析屏幕</span><span class="sxs-lookup"><span data-stu-id="d8ffb-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="d8ffb-220">响应</span><span class="sxs-lookup"><span data-stu-id="d8ffb-220">Response</span></span>
<span data-ttu-id="d8ffb-221">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-221">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ffb-222">示例</span><span class="sxs-lookup"><span data-stu-id="d8ffb-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8ffb-223">请求</span><span class="sxs-lookup"><span data-stu-id="d8ffb-223">Request</span></span>
<span data-ttu-id="d8ffb-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1061

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="d8ffb-225">响应</span><span class="sxs-lookup"><span data-stu-id="d8ffb-225">Response</span></span>
<span data-ttu-id="d8ffb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8ffb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```




