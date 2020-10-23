---
title: 创建 depMacOSEnrollmentProfile
description: 创建新的 depMacOSEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83cf72da8a1e04c2a4226b8433e75b74b8250509
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722583"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="cbe5e-103">创建 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cbe5e-103">Create depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="cbe5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbe5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbe5e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbe5e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbe5e-107">创建新的 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbe5e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbe5e-108">Prerequisites</span></span>
<span data-ttu-id="cbe5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbe5e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbe5e-111">Permission type</span></span>|<span data-ttu-id="cbe5e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbe5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbe5e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbe5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbe5e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbe5e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cbe5e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbe5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbe5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-116">Not supported.</span></span>|
|<span data-ttu-id="cbe5e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbe5e-117">Application</span></span>|<span data-ttu-id="cbe5e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbe5e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbe5e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbe5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cbe5e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbe5e-120">Request headers</span></span>
|<span data-ttu-id="cbe5e-121">标头</span><span class="sxs-lookup"><span data-stu-id="cbe5e-121">Header</span></span>|<span data-ttu-id="cbe5e-122">值</span><span class="sxs-lookup"><span data-stu-id="cbe5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbe5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbe5e-123">Authorization</span></span>|<span data-ttu-id="cbe5e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbe5e-125">接受</span><span class="sxs-lookup"><span data-stu-id="cbe5e-125">Accept</span></span>|<span data-ttu-id="cbe5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbe5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbe5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbe5e-127">Request body</span></span>
<span data-ttu-id="cbe5e-128">在请求正文中，提供 depMacOSEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="cbe5e-129">下表显示创建 depMacOSEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="cbe5e-130">属性</span><span class="sxs-lookup"><span data-stu-id="cbe5e-130">Property</span></span>|<span data-ttu-id="cbe5e-131">类型</span><span class="sxs-lookup"><span data-stu-id="cbe5e-131">Type</span></span>|<span data-ttu-id="cbe5e-132">说明</span><span class="sxs-lookup"><span data-stu-id="cbe5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbe5e-133">id</span><span class="sxs-lookup"><span data-stu-id="cbe5e-133">id</span></span>|<span data-ttu-id="cbe5e-134">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-134">String</span></span>|<span data-ttu-id="cbe5e-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="cbe5e-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cbe5e-136">displayName</span></span>|<span data-ttu-id="cbe5e-137">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-137">String</span></span>|<span data-ttu-id="cbe5e-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cbe5e-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-139">说明</span><span class="sxs-lookup"><span data-stu-id="cbe5e-139">description</span></span>|<span data-ttu-id="cbe5e-140">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-140">String</span></span>|<span data-ttu-id="cbe5e-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cbe5e-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="cbe5e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="cbe5e-143">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-143">Boolean</span></span>|<span data-ttu-id="cbe5e-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="cbe5e-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="cbe5e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="cbe5e-146">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-146">String</span></span>|<span data-ttu-id="cbe5e-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="cbe5e-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cbe5e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cbe5e-149">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-149">Boolean</span></span>|<span data-ttu-id="cbe5e-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="cbe5e-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="cbe5e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="cbe5e-153">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-153">Boolean</span></span>|<span data-ttu-id="cbe5e-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="cbe5e-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="cbe5e-155">isDefault</span></span>|<span data-ttu-id="cbe5e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbe5e-156">Boolean</span></span>|<span data-ttu-id="cbe5e-157">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="cbe5e-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-158">supervisedModeEnabled</span></span>|<span data-ttu-id="cbe5e-159">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-159">Boolean</span></span>|<span data-ttu-id="cbe5e-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="cbe5e-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="cbe5e-162">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="cbe5e-163">supportDepartment</span></span>|<span data-ttu-id="cbe5e-164">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-164">String</span></span>|<span data-ttu-id="cbe5e-165">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="cbe5e-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="cbe5e-166">isMandatory</span></span>|<span data-ttu-id="cbe5e-167">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-167">Boolean</span></span>|<span data-ttu-id="cbe5e-168">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="cbe5e-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-169">locationDisabled</span></span>|<span data-ttu-id="cbe5e-170">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-170">Boolean</span></span>|<span data-ttu-id="cbe5e-171">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="cbe5e-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="cbe5e-172">supportPhoneNumber</span></span>|<span data-ttu-id="cbe5e-173">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-173">String</span></span>|<span data-ttu-id="cbe5e-174">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="cbe5e-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-175">profileRemovalDisabled</span></span>|<span data-ttu-id="cbe5e-176">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-176">Boolean</span></span>|<span data-ttu-id="cbe5e-177">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="cbe5e-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="cbe5e-178">restoreBlocked</span></span>|<span data-ttu-id="cbe5e-179">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-179">Boolean</span></span>|<span data-ttu-id="cbe5e-180">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="cbe5e-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-181">appleIdDisabled</span></span>|<span data-ttu-id="cbe5e-182">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-182">Boolean</span></span>|<span data-ttu-id="cbe5e-183">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="cbe5e-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="cbe5e-185">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-185">Boolean</span></span>|<span data-ttu-id="cbe5e-186">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="cbe5e-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-187">touchIdDisabled</span></span>|<span data-ttu-id="cbe5e-188">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-188">Boolean</span></span>|<span data-ttu-id="cbe5e-189">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="cbe5e-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-190">applePayDisabled</span></span>|<span data-ttu-id="cbe5e-191">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-191">Boolean</span></span>|<span data-ttu-id="cbe5e-192">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="cbe5e-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-193">siriDisabled</span></span>|<span data-ttu-id="cbe5e-194">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-194">Boolean</span></span>|<span data-ttu-id="cbe5e-195">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="cbe5e-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-196">diagnosticsDisabled</span></span>|<span data-ttu-id="cbe5e-197">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-197">Boolean</span></span>|<span data-ttu-id="cbe5e-198">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="cbe5e-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="cbe5e-200">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-200">Boolean</span></span>|<span data-ttu-id="cbe5e-201">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="cbe5e-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-202">privacyPaneDisabled</span></span>|<span data-ttu-id="cbe5e-203">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-203">Boolean</span></span>|<span data-ttu-id="cbe5e-204">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="cbe5e-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="cbe5e-206">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-206">Boolean</span></span>|<span data-ttu-id="cbe5e-207">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="cbe5e-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="cbe5e-208">deviceNameTemplate</span></span>|<span data-ttu-id="cbe5e-209">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-209">String</span></span>|<span data-ttu-id="cbe5e-210">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="cbe5e-211">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="cbe5e-212">configurationWebUrl</span></span>|<span data-ttu-id="cbe5e-213">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-213">Boolean</span></span>|<span data-ttu-id="cbe5e-214">从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="cbe5e-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cbe5e-215">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-215">registrationDisabled</span></span>|<span data-ttu-id="cbe5e-216">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-216">Boolean</span></span>|<span data-ttu-id="cbe5e-217">指示是否禁用注册</span><span class="sxs-lookup"><span data-stu-id="cbe5e-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="cbe5e-218">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-218">fileVaultDisabled</span></span>|<span data-ttu-id="cbe5e-219">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-219">Boolean</span></span>|<span data-ttu-id="cbe5e-220">指示是否禁用了文件电子仓库</span><span class="sxs-lookup"><span data-stu-id="cbe5e-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="cbe5e-221">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="cbe5e-222">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-222">Boolean</span></span>|<span data-ttu-id="cbe5e-223">指示是否禁用了 iCloud 分析屏幕</span><span class="sxs-lookup"><span data-stu-id="cbe5e-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="cbe5e-224">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-224">passCodeDisabled</span></span>|<span data-ttu-id="cbe5e-225">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-225">Boolean</span></span>|<span data-ttu-id="cbe5e-226">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="cbe5e-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="cbe5e-227">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-227">zoomDisabled</span></span>|<span data-ttu-id="cbe5e-228">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-228">Boolean</span></span>|<span data-ttu-id="cbe5e-229">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="cbe5e-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="cbe5e-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="cbe5e-231">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-231">Boolean</span></span>|<span data-ttu-id="cbe5e-232">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="cbe5e-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="cbe5e-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="cbe5e-234">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-234">Boolean</span></span>|<span data-ttu-id="cbe5e-235">指示是否禁用了 iCloud 文档和桌面屏幕</span><span class="sxs-lookup"><span data-stu-id="cbe5e-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="cbe5e-236">accessibilityScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="cbe5e-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="cbe5e-237">布尔</span><span class="sxs-lookup"><span data-stu-id="cbe5e-237">Boolean</span></span>|<span data-ttu-id="cbe5e-238">指示是否禁用辅助功能屏幕</span><span class="sxs-lookup"><span data-stu-id="cbe5e-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="cbe5e-239">响应</span><span class="sxs-lookup"><span data-stu-id="cbe5e-239">Response</span></span>
<span data-ttu-id="cbe5e-240">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-240">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbe5e-241">示例</span><span class="sxs-lookup"><span data-stu-id="cbe5e-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbe5e-242">请求</span><span class="sxs-lookup"><span data-stu-id="cbe5e-242">Request</span></span>
<span data-ttu-id="cbe5e-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1300

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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
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
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="cbe5e-244">响应</span><span class="sxs-lookup"><span data-stu-id="cbe5e-244">Response</span></span>
<span data-ttu-id="cbe5e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbe5e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1349

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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
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
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true
}
```





