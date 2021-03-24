---
title: 更新 depMacOSEnrollmentProfile
description: 更新 depMacOSEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3830625f30ecb81def4b33a68e91999f0a721551
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145892"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="92565-103">更新 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="92565-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="92565-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92565-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92565-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92565-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92565-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92565-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92565-107">更新 [depMacOSEnrollmentProfile 对象](../resources/intune-enrollment-depmacosenrollmentprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="92565-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92565-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="92565-108">Prerequisites</span></span>
<span data-ttu-id="92565-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92565-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92565-111">Permission type</span></span>|<span data-ttu-id="92565-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92565-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92565-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92565-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92565-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92565-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="92565-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92565-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92565-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92565-116">Not supported.</span></span>|
|<span data-ttu-id="92565-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="92565-117">Application</span></span>|<span data-ttu-id="92565-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92565-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92565-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92565-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="92565-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="92565-120">Request headers</span></span>
|<span data-ttu-id="92565-121">标头</span><span class="sxs-lookup"><span data-stu-id="92565-121">Header</span></span>|<span data-ttu-id="92565-122">值</span><span class="sxs-lookup"><span data-stu-id="92565-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92565-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92565-123">Authorization</span></span>|<span data-ttu-id="92565-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92565-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92565-125">接受</span><span class="sxs-lookup"><span data-stu-id="92565-125">Accept</span></span>|<span data-ttu-id="92565-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92565-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92565-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="92565-127">Request body</span></span>
<span data-ttu-id="92565-128">在请求正文中，提供 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92565-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="92565-129">下表显示创建 [depMacOSEnrollmentProfile 时所需的属性](../resources/intune-enrollment-depmacosenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="92565-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="92565-130">属性</span><span class="sxs-lookup"><span data-stu-id="92565-130">Property</span></span>|<span data-ttu-id="92565-131">类型</span><span class="sxs-lookup"><span data-stu-id="92565-131">Type</span></span>|<span data-ttu-id="92565-132">说明</span><span class="sxs-lookup"><span data-stu-id="92565-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92565-133">id</span><span class="sxs-lookup"><span data-stu-id="92565-133">id</span></span>|<span data-ttu-id="92565-134">String</span><span class="sxs-lookup"><span data-stu-id="92565-134">String</span></span>|<span data-ttu-id="92565-135">对象的 GUID 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-136">displayName</span><span class="sxs-lookup"><span data-stu-id="92565-136">displayName</span></span>|<span data-ttu-id="92565-137">String</span><span class="sxs-lookup"><span data-stu-id="92565-137">String</span></span>|<span data-ttu-id="92565-138">配置文件的名称 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-139">说明</span><span class="sxs-lookup"><span data-stu-id="92565-139">description</span></span>|<span data-ttu-id="92565-140">String</span><span class="sxs-lookup"><span data-stu-id="92565-140">String</span></span>|<span data-ttu-id="92565-141">配置文件的说明 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="92565-142">requiresUserAuthentication</span></span>|<span data-ttu-id="92565-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-143">Boolean</span></span>|<span data-ttu-id="92565-144">指示配置文件是否要求用户身份验证 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="92565-145">configurationEndpointUrl</span></span>|<span data-ttu-id="92565-146">String</span><span class="sxs-lookup"><span data-stu-id="92565-146">String</span></span>|<span data-ttu-id="92565-147">用于注册的配置终结点 URL 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="92565-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="92565-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-149">Boolean</span></span>|<span data-ttu-id="92565-150">指示使用 Apple Setup Assistant 而不是公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="92565-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="92565-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="92565-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="92565-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-153">Boolean</span></span>|<span data-ttu-id="92565-154">指示注册助手注册的设备需要公司门户 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92565-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="92565-155">isDefault</span></span>|<span data-ttu-id="92565-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-156">Boolean</span></span>|<span data-ttu-id="92565-157">指示这是否为默认配置文件 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="92565-158">supervisedModeEnabled</span></span>|<span data-ttu-id="92565-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-159">Boolean</span></span>|<span data-ttu-id="92565-160">监督模式，如果为 True，则启用，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="92565-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="92565-161">有关 https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune 其他信息，请参阅 。</span><span class="sxs-lookup"><span data-stu-id="92565-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="92565-162">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="92565-163">supportDepartment</span></span>|<span data-ttu-id="92565-164">String</span><span class="sxs-lookup"><span data-stu-id="92565-164">String</span></span>|<span data-ttu-id="92565-165">支持部门信息 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="92565-166">isMandatory</span></span>|<span data-ttu-id="92565-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-167">Boolean</span></span>|<span data-ttu-id="92565-168">指示配置文件是否必需 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-169">locationDisabled</span></span>|<span data-ttu-id="92565-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-170">Boolean</span></span>|<span data-ttu-id="92565-171">指示位置服务设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="92565-172">supportPhoneNumber</span></span>|<span data-ttu-id="92565-173">String</span><span class="sxs-lookup"><span data-stu-id="92565-173">String</span></span>|<span data-ttu-id="92565-174">支持电话号码 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-175">profileRemovalDisabled</span></span>|<span data-ttu-id="92565-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-176">Boolean</span></span>|<span data-ttu-id="92565-177">指示配置文件删除选项是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="92565-178">restoreBlocked</span></span>|<span data-ttu-id="92565-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-179">Boolean</span></span>|<span data-ttu-id="92565-180">指示是否阻止"还原"设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-181">appleIdDisabled</span></span>|<span data-ttu-id="92565-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-182">Boolean</span></span>|<span data-ttu-id="92565-183">指示 Apple id 设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="92565-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-185">Boolean</span></span>|<span data-ttu-id="92565-186">指示是否禁用"条款和条件"设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-187">touchIdDisabled</span></span>|<span data-ttu-id="92565-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-188">Boolean</span></span>|<span data-ttu-id="92565-189">指示触摸 ID 设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-190">applePayDisabled</span></span>|<span data-ttu-id="92565-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-191">Boolean</span></span>|<span data-ttu-id="92565-192">指示 Apple 付款设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-193">siriDisabled</span></span>|<span data-ttu-id="92565-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-194">Boolean</span></span>|<span data-ttu-id="92565-195">指示是否禁用了 siri 设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-196">diagnosticsDisabled</span></span>|<span data-ttu-id="92565-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-197">Boolean</span></span>|<span data-ttu-id="92565-198">指示诊断设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="92565-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-200">Boolean</span></span>|<span data-ttu-id="92565-201">指示是否禁用显示铃声设置屏幕 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-202">privacyPaneDisabled</span></span>|<span data-ttu-id="92565-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-203">Boolean</span></span>|<span data-ttu-id="92565-204">指示是否禁用隐私屏幕 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="92565-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-206">Boolean</span></span>|<span data-ttu-id="92565-207">指示是否禁用屏幕超时设置 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="92565-208">deviceNameTemplate</span></span>|<span data-ttu-id="92565-209">String</span><span class="sxs-lookup"><span data-stu-id="92565-209">String</span></span>|<span data-ttu-id="92565-210">设置文字或名称模式。</span><span class="sxs-lookup"><span data-stu-id="92565-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="92565-211">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="92565-212">configurationWebUrl</span></span>|<span data-ttu-id="92565-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-213">Boolean</span></span>|<span data-ttu-id="92565-214">设置助理登录的 URL 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92565-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="92565-215">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-215">registrationDisabled</span></span>|<span data-ttu-id="92565-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-216">Boolean</span></span>|<span data-ttu-id="92565-217">指示注册是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="92565-218">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-218">fileVaultDisabled</span></span>|<span data-ttu-id="92565-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-219">Boolean</span></span>|<span data-ttu-id="92565-220">指示文件保管库是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="92565-221">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="92565-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-222">Boolean</span></span>|<span data-ttu-id="92565-223">指示 iCloud Analytics 屏幕是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="92565-224">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-224">passCodeDisabled</span></span>|<span data-ttu-id="92565-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-225">Boolean</span></span>|<span data-ttu-id="92565-226">指示密码设置窗格是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="92565-227">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-227">zoomDisabled</span></span>|<span data-ttu-id="92565-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-228">Boolean</span></span>|<span data-ttu-id="92565-229">指示是否禁用了缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="92565-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="92565-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="92565-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-231">Boolean</span></span>|<span data-ttu-id="92565-232">指示 iCloud 文档和桌面屏幕是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="92565-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="92565-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-234">Boolean</span></span>|<span data-ttu-id="92565-235">指示 iCloud 文档和桌面屏幕是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="92565-236">accessibilityScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="92565-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="92565-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="92565-237">Boolean</span></span>|<span data-ttu-id="92565-238">指示辅助功能屏幕是否被禁用</span><span class="sxs-lookup"><span data-stu-id="92565-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="92565-239">响应</span><span class="sxs-lookup"><span data-stu-id="92565-239">Response</span></span>
<span data-ttu-id="92565-240">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92565-240">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92565-241">示例</span><span class="sxs-lookup"><span data-stu-id="92565-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="92565-242">请求</span><span class="sxs-lookup"><span data-stu-id="92565-242">Request</span></span>
<span data-ttu-id="92565-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92565-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="92565-244">响应</span><span class="sxs-lookup"><span data-stu-id="92565-244">Response</span></span>
<span data-ttu-id="92565-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92565-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




