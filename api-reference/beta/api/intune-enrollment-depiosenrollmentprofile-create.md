---
title: 创建 depIOSEnrollmentProfile
description: 创建新的 depIOSEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40e506e89a8810db8c638d388ff311b7a4800b6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696732"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="43fd1-103">创建 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="43fd1-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="43fd1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43fd1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43fd1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43fd1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43fd1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43fd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43fd1-107">创建新的 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43fd1-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43fd1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="43fd1-108">Prerequisites</span></span>
<span data-ttu-id="43fd1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43fd1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43fd1-111">Permission type</span></span>|<span data-ttu-id="43fd1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43fd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43fd1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43fd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43fd1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43fd1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43fd1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43fd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43fd1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43fd1-116">Not supported.</span></span>|
|<span data-ttu-id="43fd1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="43fd1-117">Application</span></span>|<span data-ttu-id="43fd1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43fd1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43fd1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43fd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="43fd1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="43fd1-120">Request headers</span></span>
|<span data-ttu-id="43fd1-121">标头</span><span class="sxs-lookup"><span data-stu-id="43fd1-121">Header</span></span>|<span data-ttu-id="43fd1-122">值</span><span class="sxs-lookup"><span data-stu-id="43fd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43fd1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43fd1-123">Authorization</span></span>|<span data-ttu-id="43fd1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43fd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43fd1-125">接受</span><span class="sxs-lookup"><span data-stu-id="43fd1-125">Accept</span></span>|<span data-ttu-id="43fd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43fd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43fd1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43fd1-127">Request body</span></span>
<span data-ttu-id="43fd1-128">在请求正文中，提供 depIOSEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43fd1-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="43fd1-129">下表显示创建 depIOSEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43fd1-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="43fd1-130">属性</span><span class="sxs-lookup"><span data-stu-id="43fd1-130">Property</span></span>|<span data-ttu-id="43fd1-131">类型</span><span class="sxs-lookup"><span data-stu-id="43fd1-131">Type</span></span>|<span data-ttu-id="43fd1-132">说明</span><span class="sxs-lookup"><span data-stu-id="43fd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43fd1-133">id</span><span class="sxs-lookup"><span data-stu-id="43fd1-133">id</span></span>|<span data-ttu-id="43fd1-134">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-134">String</span></span>|<span data-ttu-id="43fd1-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="43fd1-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="43fd1-136">displayName</span></span>|<span data-ttu-id="43fd1-137">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-137">String</span></span>|<span data-ttu-id="43fd1-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="43fd1-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-139">说明</span><span class="sxs-lookup"><span data-stu-id="43fd1-139">description</span></span>|<span data-ttu-id="43fd1-140">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-140">String</span></span>|<span data-ttu-id="43fd1-141">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="43fd1-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="43fd1-142">requiresUserAuthentication</span></span>|<span data-ttu-id="43fd1-143">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-143">Boolean</span></span>|<span data-ttu-id="43fd1-144">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="43fd1-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="43fd1-145">configurationEndpointUrl</span></span>|<span data-ttu-id="43fd1-146">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-146">String</span></span>|<span data-ttu-id="43fd1-147">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="43fd1-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="43fd1-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="43fd1-149">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-149">Boolean</span></span>|<span data-ttu-id="43fd1-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="43fd1-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="43fd1-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43fd1-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="43fd1-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="43fd1-153">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-153">Boolean</span></span>|<span data-ttu-id="43fd1-154">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="43fd1-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43fd1-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="43fd1-155">isDefault</span></span>|<span data-ttu-id="43fd1-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="43fd1-156">Boolean</span></span>|<span data-ttu-id="43fd1-157">指示这是否是从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的默认配置文件</span><span class="sxs-lookup"><span data-stu-id="43fd1-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-158">supervisedModeEnabled</span></span>|<span data-ttu-id="43fd1-159">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-159">Boolean</span></span>|<span data-ttu-id="43fd1-160">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="43fd1-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="43fd1-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="43fd1-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="43fd1-162">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43fd1-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="43fd1-163">supportDepartment</span></span>|<span data-ttu-id="43fd1-164">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-164">String</span></span>|<span data-ttu-id="43fd1-165">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承部门信息</span><span class="sxs-lookup"><span data-stu-id="43fd1-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="43fd1-166">isMandatory</span></span>|<span data-ttu-id="43fd1-167">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-167">Boolean</span></span>|<span data-ttu-id="43fd1-168">指示是否必须从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承配置文件</span><span class="sxs-lookup"><span data-stu-id="43fd1-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-169">locationDisabled</span></span>|<span data-ttu-id="43fd1-170">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-170">Boolean</span></span>|<span data-ttu-id="43fd1-171">指示是否禁用从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="43fd1-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="43fd1-172">supportPhoneNumber</span></span>|<span data-ttu-id="43fd1-173">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-173">String</span></span>|<span data-ttu-id="43fd1-174">支持从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的电话号码</span><span class="sxs-lookup"><span data-stu-id="43fd1-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-175">profileRemovalDisabled</span></span>|<span data-ttu-id="43fd1-176">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-176">Boolean</span></span>|<span data-ttu-id="43fd1-177">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="43fd1-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="43fd1-178">restoreBlocked</span></span>|<span data-ttu-id="43fd1-179">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-179">Boolean</span></span>|<span data-ttu-id="43fd1-180">指示是否阻止从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的还原设置窗格</span><span class="sxs-lookup"><span data-stu-id="43fd1-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-181">appleIdDisabled</span></span>|<span data-ttu-id="43fd1-182">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-182">Boolean</span></span>|<span data-ttu-id="43fd1-183">指示是否禁用了 Apple id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="43fd1-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="43fd1-185">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-185">Boolean</span></span>|<span data-ttu-id="43fd1-186">指示是否已禁用 "条款和条件" 安装窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="43fd1-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-187">touchIdDisabled</span></span>|<span data-ttu-id="43fd1-188">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-188">Boolean</span></span>|<span data-ttu-id="43fd1-189">指示是否禁用了触控 id 设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="43fd1-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-190">applePayDisabled</span></span>|<span data-ttu-id="43fd1-191">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-191">Boolean</span></span>|<span data-ttu-id="43fd1-192">指示是否禁用了 Apple 付费设置窗格从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="43fd1-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-193">siriDisabled</span></span>|<span data-ttu-id="43fd1-194">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-194">Boolean</span></span>|<span data-ttu-id="43fd1-195">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 siri 安装窗格</span><span class="sxs-lookup"><span data-stu-id="43fd1-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-196">diagnosticsDisabled</span></span>|<span data-ttu-id="43fd1-197">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-197">Boolean</span></span>|<span data-ttu-id="43fd1-198">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="43fd1-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="43fd1-200">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-200">Boolean</span></span>|<span data-ttu-id="43fd1-201">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-202">privacyPaneDisabled</span></span>|<span data-ttu-id="43fd1-203">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-203">Boolean</span></span>|<span data-ttu-id="43fd1-204">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="43fd1-206">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-206">Boolean</span></span>|<span data-ttu-id="43fd1-207">指示是否禁用了从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="43fd1-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="43fd1-208">deviceNameTemplate</span></span>|<span data-ttu-id="43fd1-209">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-209">String</span></span>|<span data-ttu-id="43fd1-210">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="43fd1-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="43fd1-211">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43fd1-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="43fd1-212">configurationWebUrl</span></span>|<span data-ttu-id="43fd1-213">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-213">Boolean</span></span>|<span data-ttu-id="43fd1-214">从[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承的设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="43fd1-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="43fd1-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="43fd1-215">iTunesPairingMode</span></span>|[<span data-ttu-id="43fd1-216">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="43fd1-216">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="43fd1-217">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="43fd1-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="43fd1-218">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="43fd1-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="43fd1-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="43fd1-219">managementCertificates</span></span>|<span data-ttu-id="43fd1-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fd1-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="43fd1-221">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="43fd1-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="43fd1-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="43fd1-223">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-223">Boolean</span></span>|<span data-ttu-id="43fd1-224">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="43fd1-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="43fd1-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="43fd1-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="43fd1-226">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-226">Boolean</span></span>|<span data-ttu-id="43fd1-227">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="43fd1-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="43fd1-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="43fd1-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="43fd1-229">Int32</span><span class="sxs-lookup"><span data-stu-id="43fd1-229">Int32</span></span>|<span data-ttu-id="43fd1-230">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="43fd1-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="43fd1-231">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="43fd1-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="43fd1-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="43fd1-232">enableSharedIPad</span></span>|<span data-ttu-id="43fd1-233">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-233">Boolean</span></span>|<span data-ttu-id="43fd1-234">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="43fd1-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="43fd1-235">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="43fd1-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="43fd1-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="43fd1-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="43fd1-237">String</span><span class="sxs-lookup"><span data-stu-id="43fd1-237">String</span></span>|<span data-ttu-id="43fd1-238">如果设置，则指示应使用哪种 Vpp 令牌来部署带设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="43fd1-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="43fd1-239">若要设置此属性，必须设置 "enableAuthenticationViaCompanyPortal"。</span><span class="sxs-lookup"><span data-stu-id="43fd1-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="43fd1-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="43fd1-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="43fd1-241">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-241">Boolean</span></span>|<span data-ttu-id="43fd1-242">通知设备启用单应用模式，并在注册过程中应用应用锁定。</span><span class="sxs-lookup"><span data-stu-id="43fd1-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="43fd1-243">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="43fd1-243">Default is false.</span></span> <span data-ttu-id="43fd1-244">若要设置此属性，必须设置 "enableAuthenticationViaCompanyPortal" 和 "companyPortalVppTokenId"。</span><span class="sxs-lookup"><span data-stu-id="43fd1-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="43fd1-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="43fd1-246">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-246">Boolean</span></span>|<span data-ttu-id="43fd1-247">指示是否禁用 "主页按钮灵敏度" 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="43fd1-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="43fd1-249">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-249">Boolean</span></span>|<span data-ttu-id="43fd1-250">指示是否禁用 iMessage 和 FaceTime 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="43fd1-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="43fd1-252">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-252">Boolean</span></span>|<span data-ttu-id="43fd1-253">指示是否已禁用载入安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="43fd1-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="43fd1-255">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-255">Boolean</span></span>|<span data-ttu-id="43fd1-256">指示是否禁用了 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="43fd1-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="43fd1-258">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-258">Boolean</span></span>|<span data-ttu-id="43fd1-259">指示是否禁用强制 sofware 更新屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="43fd1-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="43fd1-261">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-261">Boolean</span></span>|<span data-ttu-id="43fd1-262">指示是否禁用监视迁移屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="43fd1-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="43fd1-264">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-264">Boolean</span></span>|<span data-ttu-id="43fd1-265">指示是否禁用 Apperance 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="43fd1-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="43fd1-267">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-267">Boolean</span></span>|<span data-ttu-id="43fd1-268">指示是否已禁用 Express 语言屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="43fd1-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="43fd1-270">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-270">Boolean</span></span>|<span data-ttu-id="43fd1-271">指示是否禁用首选语言屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="43fd1-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="43fd1-273">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-273">Boolean</span></span>|<span data-ttu-id="43fd1-274">指示是否禁用设备到设备迁移</span><span class="sxs-lookup"><span data-stu-id="43fd1-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="43fd1-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="43fd1-276">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-276">Boolean</span></span>|<span data-ttu-id="43fd1-277">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="43fd1-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-278">passCodeDisabled</span></span>|<span data-ttu-id="43fd1-279">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-279">Boolean</span></span>|<span data-ttu-id="43fd1-280">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="43fd1-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="43fd1-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-281">zoomDisabled</span></span>|<span data-ttu-id="43fd1-282">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-282">Boolean</span></span>|<span data-ttu-id="43fd1-283">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="43fd1-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="43fd1-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="43fd1-285">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-285">Boolean</span></span>|<span data-ttu-id="43fd1-286">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="43fd1-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="43fd1-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="43fd1-288">布尔</span><span class="sxs-lookup"><span data-stu-id="43fd1-288">Boolean</span></span>|<span data-ttu-id="43fd1-289">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="43fd1-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="43fd1-290">响应</span><span class="sxs-lookup"><span data-stu-id="43fd1-290">Response</span></span>
<span data-ttu-id="43fd1-291">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43fd1-291">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43fd1-292">示例</span><span class="sxs-lookup"><span data-stu-id="43fd1-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="43fd1-293">请求</span><span class="sxs-lookup"><span data-stu-id="43fd1-293">Request</span></span>
<span data-ttu-id="43fd1-294">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43fd1-294">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2108

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
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="43fd1-295">响应</span><span class="sxs-lookup"><span data-stu-id="43fd1-295">Response</span></span>
<span data-ttu-id="43fd1-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43fd1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2157

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
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```





