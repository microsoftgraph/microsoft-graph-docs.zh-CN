---
title: 更新 depIOSEnrollmentProfile
description: 更新 depIOSEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6052f3896e6f9311034b1ea2efcb0e1f084cb18a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135787"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="128a3-103">更新 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="128a3-103">Update depIOSEnrollmentProfile</span></span>

<span data-ttu-id="128a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="128a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="128a3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="128a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="128a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="128a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="128a3-107">更新 [depIOSEnrollmentProfile 对象](../resources/intune-enrollment-depiosenrollmentprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="128a3-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="128a3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="128a3-108">Prerequisites</span></span>
<span data-ttu-id="128a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="128a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="128a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="128a3-111">Permission type</span></span>|<span data-ttu-id="128a3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="128a3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="128a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="128a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="128a3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128a3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="128a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="128a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="128a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="128a3-116">Not supported.</span></span>|
|<span data-ttu-id="128a3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="128a3-117">Application</span></span>|<span data-ttu-id="128a3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128a3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="128a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="128a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="128a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="128a3-120">Request headers</span></span>
|<span data-ttu-id="128a3-121">标头</span><span class="sxs-lookup"><span data-stu-id="128a3-121">Header</span></span>|<span data-ttu-id="128a3-122">值</span><span class="sxs-lookup"><span data-stu-id="128a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="128a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="128a3-123">Authorization</span></span>|<span data-ttu-id="128a3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="128a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="128a3-125">接受</span><span class="sxs-lookup"><span data-stu-id="128a3-125">Accept</span></span>|<span data-ttu-id="128a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="128a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="128a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="128a3-127">Request body</span></span>
<span data-ttu-id="128a3-128">在请求正文中，提供 [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="128a3-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="128a3-129">下表显示创建 [depIOSEnrollmentProfile 时所需的属性](../resources/intune-enrollment-depiosenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="128a3-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="128a3-130">属性</span><span class="sxs-lookup"><span data-stu-id="128a3-130">Property</span></span>|<span data-ttu-id="128a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="128a3-131">Type</span></span>|<span data-ttu-id="128a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="128a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="128a3-133">id</span><span class="sxs-lookup"><span data-stu-id="128a3-133">id</span></span>|<span data-ttu-id="128a3-134">String</span><span class="sxs-lookup"><span data-stu-id="128a3-134">String</span></span>|<span data-ttu-id="128a3-135">对象的 GUID 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="128a3-136">displayName</span></span>|<span data-ttu-id="128a3-137">String</span><span class="sxs-lookup"><span data-stu-id="128a3-137">String</span></span>|<span data-ttu-id="128a3-138">配置文件的名称 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-139">说明</span><span class="sxs-lookup"><span data-stu-id="128a3-139">description</span></span>|<span data-ttu-id="128a3-140">String</span><span class="sxs-lookup"><span data-stu-id="128a3-140">String</span></span>|<span data-ttu-id="128a3-141">配置文件的说明 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="128a3-142">requiresUserAuthentication</span></span>|<span data-ttu-id="128a3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-143">Boolean</span></span>|<span data-ttu-id="128a3-144">指示配置文件是否要求用户身份验证 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="128a3-145">configurationEndpointUrl</span></span>|<span data-ttu-id="128a3-146">String</span><span class="sxs-lookup"><span data-stu-id="128a3-146">String</span></span>|<span data-ttu-id="128a3-147">用于注册的配置终结点 URL 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="128a3-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="128a3-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-149">Boolean</span></span>|<span data-ttu-id="128a3-150">指示使用 Apple Setup Assistant 而不是公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="128a3-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="128a3-151">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="128a3-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="128a3-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-153">Boolean</span></span>|<span data-ttu-id="128a3-154">指示注册助手注册的设备需要公司门户 继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="128a3-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="128a3-155">isDefault</span></span>|<span data-ttu-id="128a3-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-156">Boolean</span></span>|<span data-ttu-id="128a3-157">指示这是否为默认配置文件 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="128a3-158">supervisedModeEnabled</span></span>|<span data-ttu-id="128a3-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-159">Boolean</span></span>|<span data-ttu-id="128a3-160">监督模式，如果为 True，则启用，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="128a3-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="128a3-161">有关 https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune 其他信息，请参阅 。</span><span class="sxs-lookup"><span data-stu-id="128a3-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="128a3-162">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="128a3-163">supportDepartment</span></span>|<span data-ttu-id="128a3-164">String</span><span class="sxs-lookup"><span data-stu-id="128a3-164">String</span></span>|<span data-ttu-id="128a3-165">支持部门信息 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="128a3-166">isMandatory</span></span>|<span data-ttu-id="128a3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-167">Boolean</span></span>|<span data-ttu-id="128a3-168">指示配置文件是否必需 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-169">locationDisabled</span></span>|<span data-ttu-id="128a3-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-170">Boolean</span></span>|<span data-ttu-id="128a3-171">指示位置服务设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="128a3-172">supportPhoneNumber</span></span>|<span data-ttu-id="128a3-173">String</span><span class="sxs-lookup"><span data-stu-id="128a3-173">String</span></span>|<span data-ttu-id="128a3-174">支持电话号码 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-175">profileRemovalDisabled</span></span>|<span data-ttu-id="128a3-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-176">Boolean</span></span>|<span data-ttu-id="128a3-177">指示配置文件删除选项是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="128a3-178">restoreBlocked</span></span>|<span data-ttu-id="128a3-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-179">Boolean</span></span>|<span data-ttu-id="128a3-180">指示是否阻止"还原"设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-181">appleIdDisabled</span></span>|<span data-ttu-id="128a3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-182">Boolean</span></span>|<span data-ttu-id="128a3-183">指示 Apple id 设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="128a3-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-185">Boolean</span></span>|<span data-ttu-id="128a3-186">指示是否禁用"条款和条件"设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-187">touchIdDisabled</span></span>|<span data-ttu-id="128a3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-188">Boolean</span></span>|<span data-ttu-id="128a3-189">指示触摸 ID 设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-190">applePayDisabled</span></span>|<span data-ttu-id="128a3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-191">Boolean</span></span>|<span data-ttu-id="128a3-192">指示 Apple 付款设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-193">siriDisabled</span></span>|<span data-ttu-id="128a3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-194">Boolean</span></span>|<span data-ttu-id="128a3-195">指示是否禁用了 siri 设置窗格 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-196">diagnosticsDisabled</span></span>|<span data-ttu-id="128a3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-197">Boolean</span></span>|<span data-ttu-id="128a3-198">指示诊断设置窗格是否被禁用 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="128a3-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-200">Boolean</span></span>|<span data-ttu-id="128a3-201">指示是否禁用显示铃声设置屏幕 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-202">privacyPaneDisabled</span></span>|<span data-ttu-id="128a3-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-203">Boolean</span></span>|<span data-ttu-id="128a3-204">指示是否禁用隐私屏幕 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="128a3-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-206">Boolean</span></span>|<span data-ttu-id="128a3-207">指示是否禁用屏幕超时设置 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="128a3-208">deviceNameTemplate</span></span>|<span data-ttu-id="128a3-209">String</span><span class="sxs-lookup"><span data-stu-id="128a3-209">String</span></span>|<span data-ttu-id="128a3-210">设置文字或名称模式。</span><span class="sxs-lookup"><span data-stu-id="128a3-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="128a3-211">继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="128a3-212">configurationWebUrl</span></span>|<span data-ttu-id="128a3-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-213">Boolean</span></span>|<span data-ttu-id="128a3-214">设置助理登录的 URL 继承自 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="128a3-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="128a3-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="128a3-215">iTunesPairingMode</span></span>|[<span data-ttu-id="128a3-216">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="128a3-216">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="128a3-217">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="128a3-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="128a3-218">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="128a3-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="128a3-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="128a3-219">managementCertificates</span></span>|<span data-ttu-id="128a3-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="128a3-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="128a3-221">Apple Configurator 的管理证书</span><span class="sxs-lookup"><span data-stu-id="128a3-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="128a3-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="128a3-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-223">Boolean</span></span>|<span data-ttu-id="128a3-224">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="128a3-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="128a3-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="128a3-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="128a3-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-226">Boolean</span></span>|<span data-ttu-id="128a3-227">指示设备是否需要等待配置的确认</span><span class="sxs-lookup"><span data-stu-id="128a3-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="128a3-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="128a3-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="128a3-229">Int32</span><span class="sxs-lookup"><span data-stu-id="128a3-229">Int32</span></span>|<span data-ttu-id="128a3-230">这指定可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="128a3-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="128a3-231">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="128a3-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="128a3-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="128a3-232">enableSharedIPad</span></span>|<span data-ttu-id="128a3-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-233">Boolean</span></span>|<span data-ttu-id="128a3-234">这指示设备是否将在支持多用户方案的模式下注册。</span><span class="sxs-lookup"><span data-stu-id="128a3-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="128a3-235">仅适用于共享 iPad。</span><span class="sxs-lookup"><span data-stu-id="128a3-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="128a3-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="128a3-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="128a3-237">String</span><span class="sxs-lookup"><span data-stu-id="128a3-237">String</span></span>|<span data-ttu-id="128a3-238">如果设置，则指示应该使用哪个 Vpp 令牌来部署具有设备许可的公司门户。</span><span class="sxs-lookup"><span data-stu-id="128a3-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="128a3-239">必须设置"enableAuthenticationViaCompanyPortal"才能设置此属性。</span><span class="sxs-lookup"><span data-stu-id="128a3-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="128a3-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="128a3-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="128a3-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-241">Boolean</span></span>|<span data-ttu-id="128a3-242">指示设备在注册期间启用单个应用模式和应用锁。</span><span class="sxs-lookup"><span data-stu-id="128a3-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="128a3-243">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="128a3-243">Default is false.</span></span> <span data-ttu-id="128a3-244">必须设置"enableAuthenticationViaCompanyPortal"和"companyPortalVppTokenId"才能设置此属性。</span><span class="sxs-lookup"><span data-stu-id="128a3-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="128a3-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="128a3-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-246">Boolean</span></span>|<span data-ttu-id="128a3-247">指示是否禁用了"开始"按钮敏感度屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="128a3-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="128a3-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-249">Boolean</span></span>|<span data-ttu-id="128a3-250">指示 iMessage 和 FaceTime 屏幕是否被禁用</span><span class="sxs-lookup"><span data-stu-id="128a3-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="128a3-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="128a3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-252">Boolean</span></span>|<span data-ttu-id="128a3-253">指示载入设置屏幕是否处于禁用状态</span><span class="sxs-lookup"><span data-stu-id="128a3-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="128a3-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="128a3-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-255">Boolean</span></span>|<span data-ttu-id="128a3-256">指示是否禁用 SIMSetup 屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="128a3-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="128a3-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-258">Boolean</span></span>|<span data-ttu-id="128a3-259">指示是否禁用了必需的软件更新屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="128a3-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="128a3-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-261">Boolean</span></span>|<span data-ttu-id="128a3-262">指示监视迁移屏幕是否被禁用</span><span class="sxs-lookup"><span data-stu-id="128a3-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="128a3-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="128a3-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-264">Boolean</span></span>|<span data-ttu-id="128a3-265">指示是否禁用 Apperance 屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="128a3-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="128a3-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-267">Boolean</span></span>|<span data-ttu-id="128a3-268">指示是否禁用 Express Language 屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="128a3-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="128a3-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-270">Boolean</span></span>|<span data-ttu-id="128a3-271">指示是否禁用首选语言屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="128a3-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="128a3-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-273">Boolean</span></span>|<span data-ttu-id="128a3-274">指示设备到设备迁移是否被禁用</span><span class="sxs-lookup"><span data-stu-id="128a3-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="128a3-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="128a3-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-276">Boolean</span></span>|<span data-ttu-id="128a3-277">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="128a3-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-278">passCodeDisabled</span></span>|<span data-ttu-id="128a3-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-279">Boolean</span></span>|<span data-ttu-id="128a3-280">指示密码设置窗格是否被禁用</span><span class="sxs-lookup"><span data-stu-id="128a3-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="128a3-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-281">zoomDisabled</span></span>|<span data-ttu-id="128a3-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-282">Boolean</span></span>|<span data-ttu-id="128a3-283">指示是否禁用了缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="128a3-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="128a3-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="128a3-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-285">Boolean</span></span>|<span data-ttu-id="128a3-286">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="128a3-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="128a3-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="128a3-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="128a3-288">Boolean</span></span>|<span data-ttu-id="128a3-289">指示是否禁用 Weclome 屏幕</span><span class="sxs-lookup"><span data-stu-id="128a3-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="128a3-290">响应</span><span class="sxs-lookup"><span data-stu-id="128a3-290">Response</span></span>
<span data-ttu-id="128a3-291">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="128a3-291">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="128a3-292">示例</span><span class="sxs-lookup"><span data-stu-id="128a3-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="128a3-293">请求</span><span class="sxs-lookup"><span data-stu-id="128a3-293">Request</span></span>
<span data-ttu-id="128a3-294">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="128a3-294">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="128a3-295">响应</span><span class="sxs-lookup"><span data-stu-id="128a3-295">Response</span></span>
<span data-ttu-id="128a3-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="128a3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




