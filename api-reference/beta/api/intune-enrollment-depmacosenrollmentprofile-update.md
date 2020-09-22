---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96c0ce04c6193d8b69d52ee2aa42c6306e47944e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093803"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="eb278-103">更新 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="eb278-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="eb278-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb278-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb278-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb278-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb278-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb278-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb278-107">更新 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb278-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb278-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb278-108">Prerequisites</span></span>
<span data-ttu-id="eb278-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb278-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb278-111">Permission type</span></span>|<span data-ttu-id="eb278-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb278-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb278-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb278-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb278-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb278-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb278-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb278-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb278-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb278-116">Not supported.</span></span>|
|<span data-ttu-id="eb278-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb278-117">Application</span></span>|<span data-ttu-id="eb278-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb278-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb278-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb278-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="eb278-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb278-120">Request headers</span></span>
|<span data-ttu-id="eb278-121">标头</span><span class="sxs-lookup"><span data-stu-id="eb278-121">Header</span></span>|<span data-ttu-id="eb278-122">值</span><span class="sxs-lookup"><span data-stu-id="eb278-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb278-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb278-123">Authorization</span></span>|<span data-ttu-id="eb278-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb278-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb278-125">接受</span><span class="sxs-lookup"><span data-stu-id="eb278-125">Accept</span></span>|<span data-ttu-id="eb278-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb278-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb278-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb278-127">Request body</span></span>
<span data-ttu-id="eb278-128">在请求正文中，提供 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb278-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="eb278-129">下表显示创建 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb278-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="eb278-130">属性</span><span class="sxs-lookup"><span data-stu-id="eb278-130">Property</span></span>|<span data-ttu-id="eb278-131">类型</span><span class="sxs-lookup"><span data-stu-id="eb278-131">Type</span></span>|<span data-ttu-id="eb278-132">说明</span><span class="sxs-lookup"><span data-stu-id="eb278-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb278-133">id</span><span class="sxs-lookup"><span data-stu-id="eb278-133">id</span></span>|<span data-ttu-id="eb278-134">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-134">String</span></span>|<span data-ttu-id="eb278-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="eb278-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eb278-136">displayName</span></span>|<span data-ttu-id="eb278-137">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-137">String</span></span>|<span data-ttu-id="eb278-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="eb278-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-139">说明</span><span class="sxs-lookup"><span data-stu-id="eb278-139">description</span></span>|<span data-ttu-id="eb278-140">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-140">String</span></span>|<span data-ttu-id="eb278-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="eb278-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="eb278-142">requiresUserAuthentication</span></span>|<span data-ttu-id="eb278-143">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-143">Boolean</span></span>|<span data-ttu-id="eb278-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="eb278-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="eb278-145">configurationEndpointUrl</span></span>|<span data-ttu-id="eb278-146">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-146">String</span></span>|<span data-ttu-id="eb278-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="eb278-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="eb278-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="eb278-149">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-149">Boolean</span></span>|<span data-ttu-id="eb278-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="eb278-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="eb278-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb278-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="eb278-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="eb278-153">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-153">Boolean</span></span>|<span data-ttu-id="eb278-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="eb278-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb278-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="eb278-155">isDefault</span></span>|<span data-ttu-id="eb278-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb278-156">Boolean</span></span>|<span data-ttu-id="eb278-157">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="eb278-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="eb278-158">supervisedModeEnabled</span></span>|<span data-ttu-id="eb278-159">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-159">Boolean</span></span>|<span data-ttu-id="eb278-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="eb278-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="eb278-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="eb278-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="eb278-162">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb278-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="eb278-163">supportDepartment</span></span>|<span data-ttu-id="eb278-164">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-164">String</span></span>|<span data-ttu-id="eb278-165">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="eb278-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-166">passCodeDisabled</span></span>|<span data-ttu-id="eb278-167">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-167">Boolean</span></span>|<span data-ttu-id="eb278-168">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="eb278-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="eb278-169">isMandatory</span></span>|<span data-ttu-id="eb278-170">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-170">Boolean</span></span>|<span data-ttu-id="eb278-171">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="eb278-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-172">locationDisabled</span></span>|<span data-ttu-id="eb278-173">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-173">Boolean</span></span>|<span data-ttu-id="eb278-174">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="eb278-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="eb278-175">supportPhoneNumber</span></span>|<span data-ttu-id="eb278-176">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-176">String</span></span>|<span data-ttu-id="eb278-177">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="eb278-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-178">profileRemovalDisabled</span></span>|<span data-ttu-id="eb278-179">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-179">Boolean</span></span>|<span data-ttu-id="eb278-180">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="eb278-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="eb278-181">restoreBlocked</span></span>|<span data-ttu-id="eb278-182">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-182">Boolean</span></span>|<span data-ttu-id="eb278-183">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="eb278-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-184">appleIdDisabled</span></span>|<span data-ttu-id="eb278-185">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-185">Boolean</span></span>|<span data-ttu-id="eb278-186">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="eb278-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="eb278-188">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-188">Boolean</span></span>|<span data-ttu-id="eb278-189">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="eb278-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-190">touchIdDisabled</span></span>|<span data-ttu-id="eb278-191">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-191">Boolean</span></span>|<span data-ttu-id="eb278-192">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="eb278-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-193">applePayDisabled</span></span>|<span data-ttu-id="eb278-194">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-194">Boolean</span></span>|<span data-ttu-id="eb278-195">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="eb278-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-196">zoomDisabled</span></span>|<span data-ttu-id="eb278-197">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-197">Boolean</span></span>|<span data-ttu-id="eb278-198">指示是否禁用了缩放设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="eb278-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-199">siriDisabled</span></span>|<span data-ttu-id="eb278-200">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-200">Boolean</span></span>|<span data-ttu-id="eb278-201">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="eb278-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-202">diagnosticsDisabled</span></span>|<span data-ttu-id="eb278-203">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-203">Boolean</span></span>|<span data-ttu-id="eb278-204">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="eb278-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="eb278-206">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-206">Boolean</span></span>|<span data-ttu-id="eb278-207">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="eb278-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-208">privacyPaneDisabled</span></span>|<span data-ttu-id="eb278-209">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-209">Boolean</span></span>|<span data-ttu-id="eb278-210">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="eb278-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-211">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="eb278-212">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-212">Boolean</span></span>|<span data-ttu-id="eb278-213">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="eb278-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-214">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="eb278-214">deviceNameTemplate</span></span>|<span data-ttu-id="eb278-215">字符串</span><span class="sxs-lookup"><span data-stu-id="eb278-215">String</span></span>|<span data-ttu-id="eb278-216">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="eb278-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="eb278-217">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb278-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-218">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="eb278-218">configurationWebUrl</span></span>|<span data-ttu-id="eb278-219">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-219">Boolean</span></span>|<span data-ttu-id="eb278-220">从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="eb278-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="eb278-221">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-221">registrationDisabled</span></span>|<span data-ttu-id="eb278-222">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-222">Boolean</span></span>|<span data-ttu-id="eb278-223">指示是否禁用注册</span><span class="sxs-lookup"><span data-stu-id="eb278-223">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="eb278-224">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-224">fileVaultDisabled</span></span>|<span data-ttu-id="eb278-225">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-225">Boolean</span></span>|<span data-ttu-id="eb278-226">指示是否禁用了文件电子仓库</span><span class="sxs-lookup"><span data-stu-id="eb278-226">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="eb278-227">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-227">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="eb278-228">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-228">Boolean</span></span>|<span data-ttu-id="eb278-229">指示是否禁用了 iCloud 分析屏幕</span><span class="sxs-lookup"><span data-stu-id="eb278-229">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="eb278-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="eb278-231">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-231">Boolean</span></span>|<span data-ttu-id="eb278-232">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="eb278-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="eb278-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="eb278-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="eb278-234">布尔</span><span class="sxs-lookup"><span data-stu-id="eb278-234">Boolean</span></span>|<span data-ttu-id="eb278-235">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="eb278-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="eb278-236">响应</span><span class="sxs-lookup"><span data-stu-id="eb278-236">Response</span></span>
<span data-ttu-id="eb278-237">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb278-237">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb278-238">示例</span><span class="sxs-lookup"><span data-stu-id="eb278-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb278-239">请求</span><span class="sxs-lookup"><span data-stu-id="eb278-239">Request</span></span>
<span data-ttu-id="eb278-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb278-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb278-241">响应</span><span class="sxs-lookup"><span data-stu-id="eb278-241">Response</span></span>
<span data-ttu-id="eb278-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb278-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






