---
title: depEnrollmentProfile 资源类型
description: DepEnrollmentProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: da2bd0415abfeefb6e7a330663ed51cb9e5de271
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849082"
---
# <a name="depenrollmentprofile-resource-type"></a><span data-ttu-id="60d26-104">depEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="60d26-104">depEnrollmentProfile resource type</span></span>

> <span data-ttu-id="60d26-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="60d26-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60d26-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60d26-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60d26-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="60d26-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60d26-108">DepEnrollmentProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="60d26-108">The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="60d26-109">相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号</span><span class="sxs-lookup"><span data-stu-id="60d26-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="60d26-110">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="60d26-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="60d26-111">方法</span><span class="sxs-lookup"><span data-stu-id="60d26-111">Methods</span></span>
|<span data-ttu-id="60d26-112">方法</span><span class="sxs-lookup"><span data-stu-id="60d26-112">Method</span></span>|<span data-ttu-id="60d26-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="60d26-113">Return Type</span></span>|<span data-ttu-id="60d26-114">说明</span><span class="sxs-lookup"><span data-stu-id="60d26-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60d26-115">列表 depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="60d26-115">List depEnrollmentProfiles</span></span>](../api/intune-enrollment-depenrollmentprofile-list.md)|<span data-ttu-id="60d26-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="60d26-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) collection</span></span>|<span data-ttu-id="60d26-117">列出属性和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="60d26-117">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="60d26-118">获取 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-118">Get depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-get.md)|[<span data-ttu-id="60d26-119">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-119">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="60d26-120">读取属性和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="60d26-120">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="60d26-121">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-121">Create depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-create.md)|[<span data-ttu-id="60d26-122">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-122">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="60d26-123">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60d26-123">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="60d26-124">删除 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-124">Delete depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-delete.md)|<span data-ttu-id="60d26-125">无</span><span class="sxs-lookup"><span data-stu-id="60d26-125">None</span></span>|<span data-ttu-id="60d26-126">删除[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="60d26-126">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="60d26-127">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-127">Update depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-update.md)|[<span data-ttu-id="60d26-128">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="60d26-128">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="60d26-129">更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60d26-129">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60d26-130">属性</span><span class="sxs-lookup"><span data-stu-id="60d26-130">Properties</span></span>
|<span data-ttu-id="60d26-131">属性</span><span class="sxs-lookup"><span data-stu-id="60d26-131">Property</span></span>|<span data-ttu-id="60d26-132">类型</span><span class="sxs-lookup"><span data-stu-id="60d26-132">Type</span></span>|<span data-ttu-id="60d26-133">说明</span><span class="sxs-lookup"><span data-stu-id="60d26-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60d26-134">id</span><span class="sxs-lookup"><span data-stu-id="60d26-134">id</span></span>|<span data-ttu-id="60d26-135">字符串</span><span class="sxs-lookup"><span data-stu-id="60d26-135">String</span></span>|<span data-ttu-id="60d26-136">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="60d26-136">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="60d26-137">displayName</span><span class="sxs-lookup"><span data-stu-id="60d26-137">displayName</span></span>|<span data-ttu-id="60d26-138">字符串</span><span class="sxs-lookup"><span data-stu-id="60d26-138">String</span></span>|<span data-ttu-id="60d26-139">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="60d26-139">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="60d26-140">说明</span><span class="sxs-lookup"><span data-stu-id="60d26-140">description</span></span>|<span data-ttu-id="60d26-141">字符串</span><span class="sxs-lookup"><span data-stu-id="60d26-141">String</span></span>|<span data-ttu-id="60d26-142">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="60d26-142">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="60d26-143">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="60d26-143">requiresUserAuthentication</span></span>|<span data-ttu-id="60d26-144">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-144">Boolean</span></span>|<span data-ttu-id="60d26-145">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="60d26-145">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="60d26-146">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="60d26-146">configurationEndpointUrl</span></span>|<span data-ttu-id="60d26-147">字符串</span><span class="sxs-lookup"><span data-stu-id="60d26-147">String</span></span>|<span data-ttu-id="60d26-148">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="60d26-148">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="60d26-149">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="60d26-149">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="60d26-150">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-150">Boolean</span></span>|<span data-ttu-id="60d26-151">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="60d26-151">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="60d26-152">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="60d26-152">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="60d26-153">isDefault</span><span class="sxs-lookup"><span data-stu-id="60d26-153">isDefault</span></span>|<span data-ttu-id="60d26-154">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-154">Boolean</span></span>|<span data-ttu-id="60d26-155">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="60d26-155">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="60d26-156">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="60d26-156">supervisedModeEnabled</span></span>|<span data-ttu-id="60d26-157">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-157">Boolean</span></span>|<span data-ttu-id="60d26-158">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="60d26-158">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="60d26-159">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="60d26-159">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="60d26-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="60d26-160">supportDepartment</span></span>|<span data-ttu-id="60d26-161">字符串</span><span class="sxs-lookup"><span data-stu-id="60d26-161">String</span></span>|<span data-ttu-id="60d26-162">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="60d26-162">Support department information</span></span>|
|<span data-ttu-id="60d26-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-163">passCodeDisabled</span></span>|<span data-ttu-id="60d26-164">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-164">Boolean</span></span>|<span data-ttu-id="60d26-165">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-165">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="60d26-166">isMandatory</span></span>|<span data-ttu-id="60d26-167">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-167">Boolean</span></span>|<span data-ttu-id="60d26-168">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="60d26-168">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="60d26-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-169">locationDisabled</span></span>|<span data-ttu-id="60d26-170">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-170">Boolean</span></span>|<span data-ttu-id="60d26-171">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-171">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="60d26-172">supportPhoneNumber</span></span>|<span data-ttu-id="60d26-173">字符串</span><span class="sxs-lookup"><span data-stu-id="60d26-173">String</span></span>|<span data-ttu-id="60d26-174">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="60d26-174">Support phone number</span></span>|
|<span data-ttu-id="60d26-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="60d26-175">iTunesPairingMode</span></span>|[<span data-ttu-id="60d26-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="60d26-176">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="60d26-177">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="60d26-177">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="60d26-178">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="60d26-178">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="60d26-179">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-179">profileRemovalDisabled</span></span>|<span data-ttu-id="60d26-180">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-180">Boolean</span></span>|<span data-ttu-id="60d26-181">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="60d26-181">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="60d26-182">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="60d26-182">managementCertificates</span></span>|<span data-ttu-id="60d26-183">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="60d26-183">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="60d26-184">Apple 配置程序的管理证书</span><span class="sxs-lookup"><span data-stu-id="60d26-184">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="60d26-185">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="60d26-185">restoreBlocked</span></span>|<span data-ttu-id="60d26-186">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-186">Boolean</span></span>|<span data-ttu-id="60d26-187">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="60d26-187">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="60d26-188">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-188">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="60d26-189">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-189">Boolean</span></span>|<span data-ttu-id="60d26-190">指示是否从 Android 还原被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-190">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="60d26-191">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-191">appleIdDisabled</span></span>|<span data-ttu-id="60d26-192">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-192">Boolean</span></span>|<span data-ttu-id="60d26-193">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-193">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-194">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-194">termsAndConditionsDisabled</span></span>|<span data-ttu-id="60d26-195">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-195">Boolean</span></span>|<span data-ttu-id="60d26-196">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="60d26-196">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-197">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-197">touchIdDisabled</span></span>|<span data-ttu-id="60d26-198">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-198">Boolean</span></span>|<span data-ttu-id="60d26-199">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-199">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-200">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-200">applePayDisabled</span></span>|<span data-ttu-id="60d26-201">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-201">Boolean</span></span>|<span data-ttu-id="60d26-202">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-202">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-203">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-203">zoomDisabled</span></span>|<span data-ttu-id="60d26-204">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-204">Boolean</span></span>|<span data-ttu-id="60d26-205">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-205">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-206">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-206">siriDisabled</span></span>|<span data-ttu-id="60d26-207">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-207">Boolean</span></span>|<span data-ttu-id="60d26-208">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-208">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-209">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-209">diagnosticsDisabled</span></span>|<span data-ttu-id="60d26-210">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-210">Boolean</span></span>|<span data-ttu-id="60d26-211">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="60d26-211">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="60d26-212">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-212">macOSRegistrationDisabled</span></span>|<span data-ttu-id="60d26-213">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-213">Boolean</span></span>|<span data-ttu-id="60d26-214">指示已禁用 Mac OS 注册功能</span><span class="sxs-lookup"><span data-stu-id="60d26-214">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="60d26-215">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="60d26-215">macOSFileVaultDisabled</span></span>|<span data-ttu-id="60d26-216">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-216">Boolean</span></span>|<span data-ttu-id="60d26-217">指示是否禁用 Mac OS 文件存储库</span><span class="sxs-lookup"><span data-stu-id="60d26-217">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="60d26-218">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="60d26-218">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="60d26-219">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-219">Boolean</span></span>|<span data-ttu-id="60d26-220">指示是否设备需要等待配置确认</span><span class="sxs-lookup"><span data-stu-id="60d26-220">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="60d26-221">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="60d26-221">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="60d26-222">Int32</span><span class="sxs-lookup"><span data-stu-id="60d26-222">Int32</span></span>|<span data-ttu-id="60d26-223">此选项指定的最大可以使用共享的 iPad 的用户数。</span><span class="sxs-lookup"><span data-stu-id="60d26-223">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="60d26-224">仅适用于共享的 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="60d26-224">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="60d26-225">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="60d26-225">enableSharedIPad</span></span>|<span data-ttu-id="60d26-226">布尔</span><span class="sxs-lookup"><span data-stu-id="60d26-226">Boolean</span></span>|<span data-ttu-id="60d26-227">这指示是否要启用多用户方案模式注册设备。</span><span class="sxs-lookup"><span data-stu-id="60d26-227">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="60d26-228">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="60d26-228">Only applicable in shared iPads.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60d26-229">Relationships</span><span class="sxs-lookup"><span data-stu-id="60d26-229">Relationships</span></span>
<span data-ttu-id="60d26-230">无</span><span class="sxs-lookup"><span data-stu-id="60d26-230">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60d26-231">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60d26-231">JSON Representation</span></span>
<span data-ttu-id="60d26-232">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60d26-232">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```





