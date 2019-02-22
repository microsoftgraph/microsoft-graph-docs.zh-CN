---
title: depEnrollmentProfile 资源类型
description: depEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ecc14dcd7cf2d171259c76592352ff13bb6ed1d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166421"
---
# <a name="depenrollmentprofile-resource-type"></a><span data-ttu-id="3f330-104">depEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f330-104">depEnrollmentProfile resource type</span></span>

> <span data-ttu-id="3f330-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f330-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f330-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f330-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f330-107">depEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="3f330-107">The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="3f330-108">在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。</span><span class="sxs-lookup"><span data-stu-id="3f330-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="3f330-109">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3f330-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3f330-110">方法</span><span class="sxs-lookup"><span data-stu-id="3f330-110">Methods</span></span>
|<span data-ttu-id="3f330-111">方法</span><span class="sxs-lookup"><span data-stu-id="3f330-111">Method</span></span>|<span data-ttu-id="3f330-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f330-112">Return Type</span></span>|<span data-ttu-id="3f330-113">说明</span><span class="sxs-lookup"><span data-stu-id="3f330-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f330-114">列出 depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="3f330-114">List depEnrollmentProfiles</span></span>](../api/intune-enrollment-depenrollmentprofile-list.md)|<span data-ttu-id="3f330-115">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f330-115">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) collection</span></span>|<span data-ttu-id="3f330-116">列出[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f330-116">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="3f330-117">获取 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-117">Get depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-get.md)|[<span data-ttu-id="3f330-118">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-118">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="3f330-119">读取[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f330-119">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="3f330-120">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-120">Create depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-create.md)|[<span data-ttu-id="3f330-121">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-121">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="3f330-122">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f330-122">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="3f330-123">删除 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-123">Delete depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-delete.md)|<span data-ttu-id="3f330-124">无</span><span class="sxs-lookup"><span data-stu-id="3f330-124">None</span></span>|<span data-ttu-id="3f330-125">删除[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="3f330-125">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="3f330-126">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-126">Update depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-update.md)|[<span data-ttu-id="3f330-127">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3f330-127">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="3f330-128">更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f330-128">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f330-129">属性</span><span class="sxs-lookup"><span data-stu-id="3f330-129">Properties</span></span>
|<span data-ttu-id="3f330-130">属性</span><span class="sxs-lookup"><span data-stu-id="3f330-130">Property</span></span>|<span data-ttu-id="3f330-131">类型</span><span class="sxs-lookup"><span data-stu-id="3f330-131">Type</span></span>|<span data-ttu-id="3f330-132">说明</span><span class="sxs-lookup"><span data-stu-id="3f330-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f330-133">id</span><span class="sxs-lookup"><span data-stu-id="3f330-133">id</span></span>|<span data-ttu-id="3f330-134">String</span><span class="sxs-lookup"><span data-stu-id="3f330-134">String</span></span>|<span data-ttu-id="3f330-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="3f330-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3f330-136">displayName</span></span>|<span data-ttu-id="3f330-137">字符串</span><span class="sxs-lookup"><span data-stu-id="3f330-137">String</span></span>|<span data-ttu-id="3f330-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="3f330-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-139">说明</span><span class="sxs-lookup"><span data-stu-id="3f330-139">description</span></span>|<span data-ttu-id="3f330-140">字符串</span><span class="sxs-lookup"><span data-stu-id="3f330-140">String</span></span>|<span data-ttu-id="3f330-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="3f330-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="3f330-142">requiresUserAuthentication</span></span>|<span data-ttu-id="3f330-143">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-143">Boolean</span></span>|<span data-ttu-id="3f330-144">指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="3f330-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="3f330-145">configurationEndpointUrl</span></span>|<span data-ttu-id="3f330-146">字符串</span><span class="sxs-lookup"><span data-stu-id="3f330-146">String</span></span>|<span data-ttu-id="3f330-147">用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="3f330-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="3f330-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="3f330-149">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-149">Boolean</span></span>|<span data-ttu-id="3f330-150">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="3f330-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="3f330-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3f330-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="3f330-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="3f330-153">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-153">Boolean</span></span>|<span data-ttu-id="3f330-154">指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="3f330-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3f330-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="3f330-155">isDefault</span></span>|<span data-ttu-id="3f330-156">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-156">Boolean</span></span>|<span data-ttu-id="3f330-157">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="3f330-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="3f330-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="3f330-158">supervisedModeEnabled</span></span>|<span data-ttu-id="3f330-159">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-159">Boolean</span></span>|<span data-ttu-id="3f330-160">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="3f330-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="3f330-161">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="3f330-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="3f330-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="3f330-162">supportDepartment</span></span>|<span data-ttu-id="3f330-163">字符串</span><span class="sxs-lookup"><span data-stu-id="3f330-163">String</span></span>|<span data-ttu-id="3f330-164">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="3f330-164">Support department information</span></span>|
|<span data-ttu-id="3f330-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-165">passCodeDisabled</span></span>|<span data-ttu-id="3f330-166">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-166">Boolean</span></span>|<span data-ttu-id="3f330-167">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="3f330-168">isMandatory</span></span>|<span data-ttu-id="3f330-169">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-169">Boolean</span></span>|<span data-ttu-id="3f330-170">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="3f330-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="3f330-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-171">locationDisabled</span></span>|<span data-ttu-id="3f330-172">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-172">Boolean</span></span>|<span data-ttu-id="3f330-173">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3f330-174">supportPhoneNumber</span></span>|<span data-ttu-id="3f330-175">字符串</span><span class="sxs-lookup"><span data-stu-id="3f330-175">String</span></span>|<span data-ttu-id="3f330-176">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="3f330-176">Support phone number</span></span>|
|<span data-ttu-id="3f330-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="3f330-177">iTunesPairingMode</span></span>|[<span data-ttu-id="3f330-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="3f330-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="3f330-179">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="3f330-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="3f330-180">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="3f330-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="3f330-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-181">profileRemovalDisabled</span></span>|<span data-ttu-id="3f330-182">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-182">Boolean</span></span>|<span data-ttu-id="3f330-183">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="3f330-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="3f330-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="3f330-184">managementCertificates</span></span>|<span data-ttu-id="3f330-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f330-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="3f330-186">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="3f330-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="3f330-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3f330-187">restoreBlocked</span></span>|<span data-ttu-id="3f330-188">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-188">Boolean</span></span>|<span data-ttu-id="3f330-189">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="3f330-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="3f330-191">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-191">Boolean</span></span>|<span data-ttu-id="3f330-192">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="3f330-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="3f330-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-193">appleIdDisabled</span></span>|<span data-ttu-id="3f330-194">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-194">Boolean</span></span>|<span data-ttu-id="3f330-195">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="3f330-197">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-197">Boolean</span></span>|<span data-ttu-id="3f330-198">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-199">touchIdDisabled</span></span>|<span data-ttu-id="3f330-200">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-200">Boolean</span></span>|<span data-ttu-id="3f330-201">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-202">applePayDisabled</span></span>|<span data-ttu-id="3f330-203">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-203">Boolean</span></span>|<span data-ttu-id="3f330-204">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-205">zoomDisabled</span></span>|<span data-ttu-id="3f330-206">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-206">Boolean</span></span>|<span data-ttu-id="3f330-207">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-208">siriDisabled</span></span>|<span data-ttu-id="3f330-209">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-209">Boolean</span></span>|<span data-ttu-id="3f330-210">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-211">diagnosticsDisabled</span></span>|<span data-ttu-id="3f330-212">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-212">Boolean</span></span>|<span data-ttu-id="3f330-213">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="3f330-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="3f330-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="3f330-215">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-215">Boolean</span></span>|<span data-ttu-id="3f330-216">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="3f330-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="3f330-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="3f330-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="3f330-218">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-218">Boolean</span></span>|<span data-ttu-id="3f330-219">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="3f330-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="3f330-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="3f330-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="3f330-221">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-221">Boolean</span></span>|<span data-ttu-id="3f330-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="3f330-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="3f330-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="3f330-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="3f330-224">Int32</span><span class="sxs-lookup"><span data-stu-id="3f330-224">Int32</span></span>|<span data-ttu-id="3f330-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="3f330-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="3f330-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="3f330-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="3f330-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="3f330-227">enableSharedIPad</span></span>|<span data-ttu-id="3f330-228">布尔</span><span class="sxs-lookup"><span data-stu-id="3f330-228">Boolean</span></span>|<span data-ttu-id="3f330-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="3f330-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="3f330-230">仅适用于共享 ipad。</span><span class="sxs-lookup"><span data-stu-id="3f330-230">Only applicable in shared iPads.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f330-231">关系</span><span class="sxs-lookup"><span data-stu-id="3f330-231">Relationships</span></span>
<span data-ttu-id="3f330-232">无</span><span class="sxs-lookup"><span data-stu-id="3f330-232">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f330-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f330-233">JSON Representation</span></span>
<span data-ttu-id="3f330-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f330-234">Here is a JSON representation of the resource.</span></span>
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




