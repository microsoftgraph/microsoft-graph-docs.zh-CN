---
title: 创建 depIOSEnrollmentProfile
description: 创建新的 depIOSEnrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 70d992cc70904f350bc43826febf127e28719cd7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973585"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="cee30-103">创建 depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee30-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="cee30-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cee30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cee30-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cee30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cee30-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cee30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cee30-107">创建新的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cee30-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cee30-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cee30-108">Prerequisites</span></span>
<span data-ttu-id="cee30-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cee30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee30-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cee30-111">Permission type</span></span>|<span data-ttu-id="cee30-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cee30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cee30-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cee30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cee30-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee30-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cee30-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cee30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cee30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cee30-116">Not supported.</span></span>|
|<span data-ttu-id="cee30-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cee30-117">Application</span></span>|<span data-ttu-id="cee30-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cee30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cee30-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cee30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cee30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cee30-120">Request headers</span></span>
|<span data-ttu-id="cee30-121">标头</span><span class="sxs-lookup"><span data-stu-id="cee30-121">Header</span></span>|<span data-ttu-id="cee30-122">值</span><span class="sxs-lookup"><span data-stu-id="cee30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cee30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cee30-123">Authorization</span></span>|<span data-ttu-id="cee30-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cee30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cee30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cee30-125">Accept</span></span>|<span data-ttu-id="cee30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cee30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cee30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cee30-127">Request body</span></span>
<span data-ttu-id="cee30-128">在请求正文中，提供 depIOSEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cee30-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="cee30-129">下表显示时创建 depIOSEnrollmentProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cee30-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="cee30-130">属性</span><span class="sxs-lookup"><span data-stu-id="cee30-130">Property</span></span>|<span data-ttu-id="cee30-131">类型</span><span class="sxs-lookup"><span data-stu-id="cee30-131">Type</span></span>|<span data-ttu-id="cee30-132">说明</span><span class="sxs-lookup"><span data-stu-id="cee30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee30-133">id</span><span class="sxs-lookup"><span data-stu-id="cee30-133">id</span></span>|<span data-ttu-id="cee30-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-134">String</span></span>|<span data-ttu-id="cee30-135">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="cee30-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cee30-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cee30-136">displayName</span></span>|<span data-ttu-id="cee30-137">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-137">String</span></span>|<span data-ttu-id="cee30-138">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cee30-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cee30-139">说明</span><span class="sxs-lookup"><span data-stu-id="cee30-139">description</span></span>|<span data-ttu-id="cee30-140">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-140">String</span></span>|<span data-ttu-id="cee30-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cee30-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cee30-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="cee30-142">requiresUserAuthentication</span></span>|<span data-ttu-id="cee30-143">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-143">Boolean</span></span>|<span data-ttu-id="cee30-144">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="cee30-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cee30-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="cee30-145">configurationEndpointUrl</span></span>|<span data-ttu-id="cee30-146">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-146">String</span></span>|<span data-ttu-id="cee30-147">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cee30-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cee30-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cee30-149">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-149">Boolean</span></span>|<span data-ttu-id="cee30-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="cee30-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="cee30-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cee30-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="cee30-152">isDefault</span></span>|<span data-ttu-id="cee30-153">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-153">Boolean</span></span>|<span data-ttu-id="cee30-154">指示是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的默认配置文件继承</span><span class="sxs-lookup"><span data-stu-id="cee30-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="cee30-155">supervisedModeEnabled</span></span>|<span data-ttu-id="cee30-156">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-156">Boolean</span></span>|<span data-ttu-id="cee30-157">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="cee30-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="cee30-158">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="cee30-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="cee30-159">继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="cee30-160">supportDepartment</span></span>|<span data-ttu-id="cee30-161">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-161">String</span></span>|<span data-ttu-id="cee30-162">从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)支持部门信息继承</span><span class="sxs-lookup"><span data-stu-id="cee30-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-163">passCodeDisabled</span></span>|<span data-ttu-id="cee30-164">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-164">Boolean</span></span>|<span data-ttu-id="cee30-165">指示是否密码设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="cee30-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="cee30-166">isMandatory</span></span>|<span data-ttu-id="cee30-167">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-167">Boolean</span></span>|<span data-ttu-id="cee30-168">指示是否强制继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)配置文件</span><span class="sxs-lookup"><span data-stu-id="cee30-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-169">locationDisabled</span></span>|<span data-ttu-id="cee30-170">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-170">Boolean</span></span>|<span data-ttu-id="cee30-171">指示是否服务设置窗格中的位置禁用[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)继承</span><span class="sxs-lookup"><span data-stu-id="cee30-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="cee30-172">supportPhoneNumber</span></span>|<span data-ttu-id="cee30-173">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-173">String</span></span>|<span data-ttu-id="cee30-174">支持从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)的电话号码继承</span><span class="sxs-lookup"><span data-stu-id="cee30-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-175">profileRemovalDisabled</span></span>|<span data-ttu-id="cee30-176">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-176">Boolean</span></span>|<span data-ttu-id="cee30-177">指示是否已禁用配置文件删除选项继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="cee30-178">restoreBlocked</span></span>|<span data-ttu-id="cee30-179">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-179">Boolean</span></span>|<span data-ttu-id="cee30-180">指示是否还原设置窗格被阻止继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-181">appleIdDisabled</span></span>|<span data-ttu-id="cee30-182">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-182">Boolean</span></span>|<span data-ttu-id="cee30-183">指示是否 Apple id 设置窗格将从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="cee30-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="cee30-185">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-185">Boolean</span></span>|<span data-ttu-id="cee30-186">指示是否已禁用条款和条件设置窗格继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-187">touchIdDisabled</span></span>|<span data-ttu-id="cee30-188">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-188">Boolean</span></span>|<span data-ttu-id="cee30-189">指示是否触摸 id 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-190">applePayDisabled</span></span>|<span data-ttu-id="cee30-191">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-191">Boolean</span></span>|<span data-ttu-id="cee30-192">指示是否 Apple 付薪设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-193">zoomDisabled</span></span>|<span data-ttu-id="cee30-194">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-194">Boolean</span></span>|<span data-ttu-id="cee30-195">指示是否缩放设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-196">siriDisabled</span></span>|<span data-ttu-id="cee30-197">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-197">Boolean</span></span>|<span data-ttu-id="cee30-198">指示是否 siri 设置窗格被禁用继承自[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee30-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-199">diagnosticsDisabled</span></span>|<span data-ttu-id="cee30-200">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-200">Boolean</span></span>|<span data-ttu-id="cee30-201">指示安装程序窗格是的诊断是否从[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)禁用继承</span><span class="sxs-lookup"><span data-stu-id="cee30-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cee30-202">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="cee30-202">iTunesPairingMode</span></span>|[<span data-ttu-id="cee30-203">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="cee30-203">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="cee30-204">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="cee30-204">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="cee30-205">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="cee30-205">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="cee30-206">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="cee30-206">managementCertificates</span></span>|<span data-ttu-id="cee30-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="cee30-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="cee30-208">Apple 配置程序的管理证书</span><span class="sxs-lookup"><span data-stu-id="cee30-208">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="cee30-209">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="cee30-209">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="cee30-210">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-210">Boolean</span></span>|<span data-ttu-id="cee30-211">指示是否从 Android 还原被禁用</span><span class="sxs-lookup"><span data-stu-id="cee30-211">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="cee30-212">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="cee30-212">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="cee30-213">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-213">Boolean</span></span>|<span data-ttu-id="cee30-214">指示是否设备需要等待配置确认</span><span class="sxs-lookup"><span data-stu-id="cee30-214">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="cee30-215">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="cee30-215">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="cee30-216">Int32</span><span class="sxs-lookup"><span data-stu-id="cee30-216">Int32</span></span>|<span data-ttu-id="cee30-217">此选项指定的最大可以使用共享的 iPad 的用户数。</span><span class="sxs-lookup"><span data-stu-id="cee30-217">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="cee30-218">仅适用于共享的 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="cee30-218">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="cee30-219">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="cee30-219">enableSharedIPad</span></span>|<span data-ttu-id="cee30-220">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-220">Boolean</span></span>|<span data-ttu-id="cee30-221">这指示是否要启用多用户方案模式注册设备。</span><span class="sxs-lookup"><span data-stu-id="cee30-221">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="cee30-222">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="cee30-222">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="cee30-223">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="cee30-223">companyPortalVppTokenId</span></span>|<span data-ttu-id="cee30-224">字符串</span><span class="sxs-lookup"><span data-stu-id="cee30-224">String</span></span>|<span data-ttu-id="cee30-225">如果设置，则指示用于部署具有设备许可的公司门户的 Vpp 令牌。</span><span class="sxs-lookup"><span data-stu-id="cee30-225">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="cee30-226">要设置此属性，必须设置 enableAuthenticationViaCompanyPortal。</span><span class="sxs-lookup"><span data-stu-id="cee30-226">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="cee30-227">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="cee30-227">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="cee30-228">布尔</span><span class="sxs-lookup"><span data-stu-id="cee30-228">Boolean</span></span>|<span data-ttu-id="cee30-229">通知要启用单个应用程序模式并应用在注册期间应用锁的设备。</span><span class="sxs-lookup"><span data-stu-id="cee30-229">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="cee30-230">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="cee30-230">Default is false.</span></span> <span data-ttu-id="cee30-231">必须为要设置此属性设置 enableAuthenticationViaCompanyPortal' 和 'companyPortalVppTokenId。</span><span class="sxs-lookup"><span data-stu-id="cee30-231">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|



## <a name="response"></a><span data-ttu-id="cee30-232">响应</span><span class="sxs-lookup"><span data-stu-id="cee30-232">Response</span></span>
<span data-ttu-id="cee30-233">如果成功，此方法返回`201 Created`响应代码和响应正文中的[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cee30-233">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cee30-234">示例</span><span class="sxs-lookup"><span data-stu-id="cee30-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="cee30-235">请求</span><span class="sxs-lookup"><span data-stu-id="cee30-235">Request</span></span>
<span data-ttu-id="cee30-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cee30-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1329

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a><span data-ttu-id="cee30-237">响应</span><span class="sxs-lookup"><span data-stu-id="cee30-237">Response</span></span>
<span data-ttu-id="cee30-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cee30-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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
  "enableSingleAppEnrollmentMode": true
}
```





