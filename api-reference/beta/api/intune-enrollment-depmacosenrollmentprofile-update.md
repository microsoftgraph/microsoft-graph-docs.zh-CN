---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94f8b01a0eea89f9186d3718f985c51f2083c7b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467142"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="ecde1-103">更新 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ecde1-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="ecde1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ecde1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecde1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ecde1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecde1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ecde1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecde1-107">更新[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ecde1-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecde1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecde1-108">Prerequisites</span></span>
<span data-ttu-id="ecde1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecde1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecde1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecde1-111">Permission type</span></span>|<span data-ttu-id="ecde1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ecde1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecde1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecde1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecde1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecde1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ecde1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecde1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecde1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecde1-116">Not supported.</span></span>|
|<span data-ttu-id="ecde1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecde1-117">Application</span></span>|<span data-ttu-id="ecde1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecde1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecde1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecde1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ecde1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecde1-120">Request headers</span></span>
|<span data-ttu-id="ecde1-121">标头</span><span class="sxs-lookup"><span data-stu-id="ecde1-121">Header</span></span>|<span data-ttu-id="ecde1-122">值</span><span class="sxs-lookup"><span data-stu-id="ecde1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecde1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecde1-123">Authorization</span></span>|<span data-ttu-id="ecde1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecde1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecde1-125">接受</span><span class="sxs-lookup"><span data-stu-id="ecde1-125">Accept</span></span>|<span data-ttu-id="ecde1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecde1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecde1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecde1-127">Request body</span></span>
<span data-ttu-id="ecde1-128">在请求正文中，提供[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecde1-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="ecde1-129">下表显示创建[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ecde1-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="ecde1-130">属性</span><span class="sxs-lookup"><span data-stu-id="ecde1-130">Property</span></span>|<span data-ttu-id="ecde1-131">类型</span><span class="sxs-lookup"><span data-stu-id="ecde1-131">Type</span></span>|<span data-ttu-id="ecde1-132">说明</span><span class="sxs-lookup"><span data-stu-id="ecde1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecde1-133">id</span><span class="sxs-lookup"><span data-stu-id="ecde1-133">id</span></span>|<span data-ttu-id="ecde1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ecde1-134">String</span></span>|<span data-ttu-id="ecde1-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="ecde1-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ecde1-136">displayName</span></span>|<span data-ttu-id="ecde1-137">String</span><span class="sxs-lookup"><span data-stu-id="ecde1-137">String</span></span>|<span data-ttu-id="ecde1-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="ecde1-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-139">说明</span><span class="sxs-lookup"><span data-stu-id="ecde1-139">description</span></span>|<span data-ttu-id="ecde1-140">String</span><span class="sxs-lookup"><span data-stu-id="ecde1-140">String</span></span>|<span data-ttu-id="ecde1-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="ecde1-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ecde1-142">requiresUserAuthentication</span></span>|<span data-ttu-id="ecde1-143">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-143">Boolean</span></span>|<span data-ttu-id="ecde1-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="ecde1-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ecde1-145">configurationEndpointUrl</span></span>|<span data-ttu-id="ecde1-146">String</span><span class="sxs-lookup"><span data-stu-id="ecde1-146">String</span></span>|<span data-ttu-id="ecde1-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="ecde1-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ecde1-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ecde1-149">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-149">Boolean</span></span>|<span data-ttu-id="ecde1-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="ecde1-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ecde1-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ecde1-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ecde1-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ecde1-153">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-153">Boolean</span></span>|<span data-ttu-id="ecde1-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="ecde1-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ecde1-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="ecde1-155">isDefault</span></span>|<span data-ttu-id="ecde1-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecde1-156">Boolean</span></span>|<span data-ttu-id="ecde1-157">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="ecde1-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-158">supervisedModeEnabled</span></span>|<span data-ttu-id="ecde1-159">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-159">Boolean</span></span>|<span data-ttu-id="ecde1-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="ecde1-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ecde1-161">有关https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="ecde1-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="ecde1-162">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ecde1-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ecde1-163">supportDepartment</span></span>|<span data-ttu-id="ecde1-164">String</span><span class="sxs-lookup"><span data-stu-id="ecde1-164">String</span></span>|<span data-ttu-id="ecde1-165">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="ecde1-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-166">passCodeDisabled</span></span>|<span data-ttu-id="ecde1-167">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-167">Boolean</span></span>|<span data-ttu-id="ecde1-168">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="ecde1-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ecde1-169">isMandatory</span></span>|<span data-ttu-id="ecde1-170">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-170">Boolean</span></span>|<span data-ttu-id="ecde1-171">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="ecde1-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-172">locationDisabled</span></span>|<span data-ttu-id="ecde1-173">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-173">Boolean</span></span>|<span data-ttu-id="ecde1-174">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="ecde1-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ecde1-175">supportPhoneNumber</span></span>|<span data-ttu-id="ecde1-176">String</span><span class="sxs-lookup"><span data-stu-id="ecde1-176">String</span></span>|<span data-ttu-id="ecde1-177">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="ecde1-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-178">profileRemovalDisabled</span></span>|<span data-ttu-id="ecde1-179">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-179">Boolean</span></span>|<span data-ttu-id="ecde1-180">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="ecde1-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ecde1-181">restoreBlocked</span></span>|<span data-ttu-id="ecde1-182">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-182">Boolean</span></span>|<span data-ttu-id="ecde1-183">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="ecde1-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-184">appleIdDisabled</span></span>|<span data-ttu-id="ecde1-185">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-185">Boolean</span></span>|<span data-ttu-id="ecde1-186">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="ecde1-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ecde1-188">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-188">Boolean</span></span>|<span data-ttu-id="ecde1-189">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="ecde1-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-190">touchIdDisabled</span></span>|<span data-ttu-id="ecde1-191">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-191">Boolean</span></span>|<span data-ttu-id="ecde1-192">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="ecde1-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-193">applePayDisabled</span></span>|<span data-ttu-id="ecde1-194">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-194">Boolean</span></span>|<span data-ttu-id="ecde1-195">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="ecde1-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-196">zoomDisabled</span></span>|<span data-ttu-id="ecde1-197">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-197">Boolean</span></span>|<span data-ttu-id="ecde1-198">指示是否禁用了缩放设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="ecde1-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-199">siriDisabled</span></span>|<span data-ttu-id="ecde1-200">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-200">Boolean</span></span>|<span data-ttu-id="ecde1-201">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="ecde1-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-202">diagnosticsDisabled</span></span>|<span data-ttu-id="ecde1-203">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-203">Boolean</span></span>|<span data-ttu-id="ecde1-204">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="ecde1-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="ecde1-206">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-206">Boolean</span></span>|<span data-ttu-id="ecde1-207">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="ecde1-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-208">privacyPaneDisabled</span></span>|<span data-ttu-id="ecde1-209">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-209">Boolean</span></span>|<span data-ttu-id="ecde1-210">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="ecde1-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-211">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="ecde1-212">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-212">Boolean</span></span>|<span data-ttu-id="ecde1-213">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="ecde1-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-214">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="ecde1-214">deviceNameTemplate</span></span>|<span data-ttu-id="ecde1-215">String</span><span class="sxs-lookup"><span data-stu-id="ecde1-215">String</span></span>|<span data-ttu-id="ecde1-216">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="ecde1-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="ecde1-217">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ecde1-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-218">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="ecde1-218">configurationWebUrl</span></span>|<span data-ttu-id="ecde1-219">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-219">Boolean</span></span>|<span data-ttu-id="ecde1-220">从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="ecde1-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ecde1-221">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-221">registrationDisabled</span></span>|<span data-ttu-id="ecde1-222">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-222">Boolean</span></span>|<span data-ttu-id="ecde1-223">指示是否禁用注册</span><span class="sxs-lookup"><span data-stu-id="ecde1-223">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="ecde1-224">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-224">fileVaultDisabled</span></span>|<span data-ttu-id="ecde1-225">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-225">Boolean</span></span>|<span data-ttu-id="ecde1-226">指示是否禁用了文件电子仓库</span><span class="sxs-lookup"><span data-stu-id="ecde1-226">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="ecde1-227">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-227">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="ecde1-228">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-228">Boolean</span></span>|<span data-ttu-id="ecde1-229">指示是否禁用了 iCloud 分析屏幕</span><span class="sxs-lookup"><span data-stu-id="ecde1-229">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="ecde1-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="ecde1-231">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-231">Boolean</span></span>|<span data-ttu-id="ecde1-232">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="ecde1-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="ecde1-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ecde1-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="ecde1-234">布尔</span><span class="sxs-lookup"><span data-stu-id="ecde1-234">Boolean</span></span>|<span data-ttu-id="ecde1-235">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="ecde1-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="ecde1-236">响应</span><span class="sxs-lookup"><span data-stu-id="ecde1-236">Response</span></span>
<span data-ttu-id="ecde1-237">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ecde1-237">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecde1-238">示例</span><span class="sxs-lookup"><span data-stu-id="ecde1-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecde1-239">请求</span><span class="sxs-lookup"><span data-stu-id="ecde1-239">Request</span></span>
<span data-ttu-id="ecde1-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecde1-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1260

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="ecde1-241">响应</span><span class="sxs-lookup"><span data-stu-id="ecde1-241">Response</span></span>
<span data-ttu-id="ecde1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecde1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1309

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```





