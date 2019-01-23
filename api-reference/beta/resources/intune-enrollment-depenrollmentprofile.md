---
title: depEnrollmentProfile 资源类型
description: DepEnrollmentProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61119a97deb41807e6eee66f0ef3376035500190
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395900"
---
# <a name="depenrollmentprofile-resource-type"></a><span data-ttu-id="c3f8c-104">depEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3f8c-104">depEnrollmentProfile resource type</span></span>

> <span data-ttu-id="c3f8c-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3f8c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3f8c-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3f8c-108">DepEnrollmentProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-108">The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="c3f8c-109">相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号</span><span class="sxs-lookup"><span data-stu-id="c3f8c-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="c3f8c-110">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c3f8c-111">方法</span><span class="sxs-lookup"><span data-stu-id="c3f8c-111">Methods</span></span>
|<span data-ttu-id="c3f8c-112">方法</span><span class="sxs-lookup"><span data-stu-id="c3f8c-112">Method</span></span>|<span data-ttu-id="c3f8c-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3f8c-113">Return Type</span></span>|<span data-ttu-id="c3f8c-114">说明</span><span class="sxs-lookup"><span data-stu-id="c3f8c-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3f8c-115">列表 depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="c3f8c-115">List depEnrollmentProfiles</span></span>](../api/intune-enrollment-depenrollmentprofile-list.md)|<span data-ttu-id="c3f8c-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3f8c-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) collection</span></span>|<span data-ttu-id="c3f8c-117">列出属性和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-117">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="c3f8c-118">获取 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-118">Get depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-get.md)|[<span data-ttu-id="c3f8c-119">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-119">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="c3f8c-120">读取属性和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-120">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c3f8c-121">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-121">Create depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-create.md)|[<span data-ttu-id="c3f8c-122">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-122">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="c3f8c-123">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-123">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c3f8c-124">删除 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-124">Delete depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-delete.md)|<span data-ttu-id="c3f8c-125">无</span><span class="sxs-lookup"><span data-stu-id="c3f8c-125">None</span></span>|<span data-ttu-id="c3f8c-126">删除[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-126">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="c3f8c-127">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-127">Update depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-update.md)|[<span data-ttu-id="c3f8c-128">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c3f8c-128">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="c3f8c-129">更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-129">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3f8c-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3f8c-130">Properties</span></span>
|<span data-ttu-id="c3f8c-131">属性</span><span class="sxs-lookup"><span data-stu-id="c3f8c-131">Property</span></span>|<span data-ttu-id="c3f8c-132">类型</span><span class="sxs-lookup"><span data-stu-id="c3f8c-132">Type</span></span>|<span data-ttu-id="c3f8c-133">说明</span><span class="sxs-lookup"><span data-stu-id="c3f8c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3f8c-134">id</span><span class="sxs-lookup"><span data-stu-id="c3f8c-134">id</span></span>|<span data-ttu-id="c3f8c-135">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-135">String</span></span>|<span data-ttu-id="c3f8c-136">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="c3f8c-136">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c3f8c-137">displayName</span></span>|<span data-ttu-id="c3f8c-138">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-138">String</span></span>|<span data-ttu-id="c3f8c-139">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="c3f8c-139">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-140">说明</span><span class="sxs-lookup"><span data-stu-id="c3f8c-140">description</span></span>|<span data-ttu-id="c3f8c-141">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-141">String</span></span>|<span data-ttu-id="c3f8c-142">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="c3f8c-142">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-143">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="c3f8c-143">requiresUserAuthentication</span></span>|<span data-ttu-id="c3f8c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-144">Boolean</span></span>|<span data-ttu-id="c3f8c-145">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="c3f8c-145">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-146">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="c3f8c-146">configurationEndpointUrl</span></span>|<span data-ttu-id="c3f8c-147">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-147">String</span></span>|<span data-ttu-id="c3f8c-148">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-148">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-149">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c3f8c-149">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c3f8c-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-150">Boolean</span></span>|<span data-ttu-id="c3f8c-151">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-151">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="c3f8c-152">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c3f8c-152">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-153">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="c3f8c-153">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="c3f8c-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-154">Boolean</span></span>|<span data-ttu-id="c3f8c-155">指示安装程序注册的助手设备继承[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) ，需要的公司门户</span><span class="sxs-lookup"><span data-stu-id="c3f8c-155">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c3f8c-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="c3f8c-156">isDefault</span></span>|<span data-ttu-id="c3f8c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-157">Boolean</span></span>|<span data-ttu-id="c3f8c-158">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="c3f8c-158">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="c3f8c-159">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-159">supervisedModeEnabled</span></span>|<span data-ttu-id="c3f8c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-160">Boolean</span></span>|<span data-ttu-id="c3f8c-161">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-161">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="c3f8c-162">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-162">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="c3f8c-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="c3f8c-163">supportDepartment</span></span>|<span data-ttu-id="c3f8c-164">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-164">String</span></span>|<span data-ttu-id="c3f8c-165">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="c3f8c-165">Support department information</span></span>|
|<span data-ttu-id="c3f8c-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-166">passCodeDisabled</span></span>|<span data-ttu-id="c3f8c-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-167">Boolean</span></span>|<span data-ttu-id="c3f8c-168">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-168">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="c3f8c-169">isMandatory</span></span>|<span data-ttu-id="c3f8c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-170">Boolean</span></span>|<span data-ttu-id="c3f8c-171">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="c3f8c-171">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="c3f8c-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-172">locationDisabled</span></span>|<span data-ttu-id="c3f8c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-173">Boolean</span></span>|<span data-ttu-id="c3f8c-174">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-174">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c3f8c-175">supportPhoneNumber</span></span>|<span data-ttu-id="c3f8c-176">String</span><span class="sxs-lookup"><span data-stu-id="c3f8c-176">String</span></span>|<span data-ttu-id="c3f8c-177">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="c3f8c-177">Support phone number</span></span>|
|<span data-ttu-id="c3f8c-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="c3f8c-178">iTunesPairingMode</span></span>|[<span data-ttu-id="c3f8c-179">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="c3f8c-179">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="c3f8c-180">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-180">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="c3f8c-181">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-181">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="c3f8c-182">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-182">profileRemovalDisabled</span></span>|<span data-ttu-id="c3f8c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-183">Boolean</span></span>|<span data-ttu-id="c3f8c-184">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="c3f8c-184">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="c3f8c-185">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="c3f8c-185">managementCertificates</span></span>|<span data-ttu-id="c3f8c-186">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3f8c-186">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="c3f8c-187">Apple 配置程序的管理证书</span><span class="sxs-lookup"><span data-stu-id="c3f8c-187">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="c3f8c-188">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c3f8c-188">restoreBlocked</span></span>|<span data-ttu-id="c3f8c-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-189">Boolean</span></span>|<span data-ttu-id="c3f8c-190">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="c3f8c-190">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="c3f8c-191">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-191">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="c3f8c-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-192">Boolean</span></span>|<span data-ttu-id="c3f8c-193">指示是否从 Android 还原被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-193">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="c3f8c-194">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-194">appleIdDisabled</span></span>|<span data-ttu-id="c3f8c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-195">Boolean</span></span>|<span data-ttu-id="c3f8c-196">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-196">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-197">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-197">termsAndConditionsDisabled</span></span>|<span data-ttu-id="c3f8c-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-198">Boolean</span></span>|<span data-ttu-id="c3f8c-199">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="c3f8c-199">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-200">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-200">touchIdDisabled</span></span>|<span data-ttu-id="c3f8c-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-201">Boolean</span></span>|<span data-ttu-id="c3f8c-202">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-202">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-203">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-203">applePayDisabled</span></span>|<span data-ttu-id="c3f8c-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-204">Boolean</span></span>|<span data-ttu-id="c3f8c-205">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-205">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-206">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-206">zoomDisabled</span></span>|<span data-ttu-id="c3f8c-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-207">Boolean</span></span>|<span data-ttu-id="c3f8c-208">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-208">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-209">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-209">siriDisabled</span></span>|<span data-ttu-id="c3f8c-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-210">Boolean</span></span>|<span data-ttu-id="c3f8c-211">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-211">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-212">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-212">diagnosticsDisabled</span></span>|<span data-ttu-id="c3f8c-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-213">Boolean</span></span>|<span data-ttu-id="c3f8c-214">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="c3f8c-214">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="c3f8c-215">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-215">macOSRegistrationDisabled</span></span>|<span data-ttu-id="c3f8c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-216">Boolean</span></span>|<span data-ttu-id="c3f8c-217">指示已禁用 Mac OS 注册功能</span><span class="sxs-lookup"><span data-stu-id="c3f8c-217">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="c3f8c-218">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="c3f8c-218">macOSFileVaultDisabled</span></span>|<span data-ttu-id="c3f8c-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-219">Boolean</span></span>|<span data-ttu-id="c3f8c-220">指示是否禁用 Mac OS 文件存储库</span><span class="sxs-lookup"><span data-stu-id="c3f8c-220">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="c3f8c-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="c3f8c-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="c3f8c-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-222">Boolean</span></span>|<span data-ttu-id="c3f8c-223">指示是否设备需要等待配置确认</span><span class="sxs-lookup"><span data-stu-id="c3f8c-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="c3f8c-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="c3f8c-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="c3f8c-225">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f8c-225">Int32</span></span>|<span data-ttu-id="c3f8c-226">此选项指定的最大可以使用共享的 iPad 的用户数。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="c3f8c-227">仅适用于共享的 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="c3f8c-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="c3f8c-228">enableSharedIPad</span></span>|<span data-ttu-id="c3f8c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f8c-229">Boolean</span></span>|<span data-ttu-id="c3f8c-230">这指示是否要启用多用户方案模式注册设备。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="c3f8c-231">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-231">Only applicable in shared iPads.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3f8c-232">关系</span><span class="sxs-lookup"><span data-stu-id="c3f8c-232">Relationships</span></span>
<span data-ttu-id="c3f8c-233">无</span><span class="sxs-lookup"><span data-stu-id="c3f8c-233">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3f8c-234">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3f8c-234">JSON Representation</span></span>
<span data-ttu-id="c3f8c-235">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3f8c-235">Here is a JSON representation of the resource.</span></span>
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
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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




