---
title: depEnrollmentProfile 资源类型
description: depEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4a365ee8a83820789ecdbf199df5997b6e683e0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806095"
---
# <a name="depenrollmentprofile-resource-type"></a><span data-ttu-id="d80d2-104">depEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d80d2-104">depEnrollmentProfile resource type</span></span>

> <span data-ttu-id="d80d2-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d80d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d80d2-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d80d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d80d2-107">depEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="d80d2-107">The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="d80d2-108">在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。</span><span class="sxs-lookup"><span data-stu-id="d80d2-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="d80d2-109">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d80d2-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d80d2-110">方法</span><span class="sxs-lookup"><span data-stu-id="d80d2-110">Methods</span></span>
|<span data-ttu-id="d80d2-111">方法</span><span class="sxs-lookup"><span data-stu-id="d80d2-111">Method</span></span>|<span data-ttu-id="d80d2-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d80d2-112">Return Type</span></span>|<span data-ttu-id="d80d2-113">说明</span><span class="sxs-lookup"><span data-stu-id="d80d2-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d80d2-114">列出 depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="d80d2-114">List depEnrollmentProfiles</span></span>](../api/intune-enrollment-depenrollmentprofile-list.md)|<span data-ttu-id="d80d2-115">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="d80d2-115">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) collection</span></span>|<span data-ttu-id="d80d2-116">列出[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d80d2-116">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="d80d2-117">获取 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-117">Get depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-get.md)|[<span data-ttu-id="d80d2-118">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-118">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="d80d2-119">读取[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d80d2-119">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d80d2-120">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-120">Create depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-create.md)|[<span data-ttu-id="d80d2-121">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-121">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="d80d2-122">创建新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d80d2-122">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d80d2-123">删除 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-123">Delete depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-delete.md)|<span data-ttu-id="d80d2-124">无</span><span class="sxs-lookup"><span data-stu-id="d80d2-124">None</span></span>|<span data-ttu-id="d80d2-125">删除[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="d80d2-125">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="d80d2-126">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-126">Update depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-update.md)|[<span data-ttu-id="d80d2-127">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d80d2-127">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="d80d2-128">更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d80d2-128">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d80d2-129">属性</span><span class="sxs-lookup"><span data-stu-id="d80d2-129">Properties</span></span>
|<span data-ttu-id="d80d2-130">属性</span><span class="sxs-lookup"><span data-stu-id="d80d2-130">Property</span></span>|<span data-ttu-id="d80d2-131">类型</span><span class="sxs-lookup"><span data-stu-id="d80d2-131">Type</span></span>|<span data-ttu-id="d80d2-132">说明</span><span class="sxs-lookup"><span data-stu-id="d80d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d80d2-133">id</span><span class="sxs-lookup"><span data-stu-id="d80d2-133">id</span></span>|<span data-ttu-id="d80d2-134">String</span><span class="sxs-lookup"><span data-stu-id="d80d2-134">String</span></span>|<span data-ttu-id="d80d2-135">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="d80d2-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d80d2-136">displayName</span></span>|<span data-ttu-id="d80d2-137">String</span><span class="sxs-lookup"><span data-stu-id="d80d2-137">String</span></span>|<span data-ttu-id="d80d2-138">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="d80d2-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-139">description</span><span class="sxs-lookup"><span data-stu-id="d80d2-139">description</span></span>|<span data-ttu-id="d80d2-140">String</span><span class="sxs-lookup"><span data-stu-id="d80d2-140">String</span></span>|<span data-ttu-id="d80d2-141">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="d80d2-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d80d2-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d80d2-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-143">Boolean</span></span>|<span data-ttu-id="d80d2-144">指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="d80d2-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d80d2-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d80d2-146">String</span><span class="sxs-lookup"><span data-stu-id="d80d2-146">String</span></span>|<span data-ttu-id="d80d2-147">用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="d80d2-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d80d2-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d80d2-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-149">Boolean</span></span>|<span data-ttu-id="d80d2-150">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d80d2-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d80d2-151">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d80d2-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d80d2-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d80d2-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-153">Boolean</span></span>|<span data-ttu-id="d80d2-154">指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="d80d2-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d80d2-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="d80d2-155">isDefault</span></span>|<span data-ttu-id="d80d2-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80d2-156">Boolean</span></span>|<span data-ttu-id="d80d2-157">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="d80d2-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="d80d2-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-158">supervisedModeEnabled</span></span>|<span data-ttu-id="d80d2-159">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-159">Boolean</span></span>|<span data-ttu-id="d80d2-160">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="d80d2-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d80d2-161">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="d80d2-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="d80d2-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="d80d2-162">supportDepartment</span></span>|<span data-ttu-id="d80d2-163">String</span><span class="sxs-lookup"><span data-stu-id="d80d2-163">String</span></span>|<span data-ttu-id="d80d2-164">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="d80d2-164">Support department information</span></span>|
|<span data-ttu-id="d80d2-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-165">passCodeDisabled</span></span>|<span data-ttu-id="d80d2-166">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-166">Boolean</span></span>|<span data-ttu-id="d80d2-167">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="d80d2-168">isMandatory</span></span>|<span data-ttu-id="d80d2-169">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-169">Boolean</span></span>|<span data-ttu-id="d80d2-170">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="d80d2-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="d80d2-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-171">locationDisabled</span></span>|<span data-ttu-id="d80d2-172">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-172">Boolean</span></span>|<span data-ttu-id="d80d2-173">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d80d2-174">supportPhoneNumber</span></span>|<span data-ttu-id="d80d2-175">String</span><span class="sxs-lookup"><span data-stu-id="d80d2-175">String</span></span>|<span data-ttu-id="d80d2-176">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="d80d2-176">Support phone number</span></span>|
|<span data-ttu-id="d80d2-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d80d2-177">iTunesPairingMode</span></span>|[<span data-ttu-id="d80d2-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d80d2-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="d80d2-179">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="d80d2-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d80d2-180">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="d80d2-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d80d2-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-181">profileRemovalDisabled</span></span>|<span data-ttu-id="d80d2-182">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-182">Boolean</span></span>|<span data-ttu-id="d80d2-183">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="d80d2-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="d80d2-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="d80d2-184">managementCertificates</span></span>|<span data-ttu-id="d80d2-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合</span><span class="sxs-lookup"><span data-stu-id="d80d2-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d80d2-186">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="d80d2-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d80d2-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d80d2-187">restoreBlocked</span></span>|<span data-ttu-id="d80d2-188">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-188">Boolean</span></span>|<span data-ttu-id="d80d2-189">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="d80d2-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d80d2-191">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-191">Boolean</span></span>|<span data-ttu-id="d80d2-192">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="d80d2-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d80d2-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-193">appleIdDisabled</span></span>|<span data-ttu-id="d80d2-194">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-194">Boolean</span></span>|<span data-ttu-id="d80d2-195">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d80d2-197">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-197">Boolean</span></span>|<span data-ttu-id="d80d2-198">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-199">touchIdDisabled</span></span>|<span data-ttu-id="d80d2-200">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-200">Boolean</span></span>|<span data-ttu-id="d80d2-201">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-202">applePayDisabled</span></span>|<span data-ttu-id="d80d2-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-203">Boolean</span></span>|<span data-ttu-id="d80d2-204">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-205">zoomDisabled</span></span>|<span data-ttu-id="d80d2-206">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-206">Boolean</span></span>|<span data-ttu-id="d80d2-207">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-208">siriDisabled</span></span>|<span data-ttu-id="d80d2-209">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-209">Boolean</span></span>|<span data-ttu-id="d80d2-210">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-211">diagnosticsDisabled</span></span>|<span data-ttu-id="d80d2-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-212">Boolean</span></span>|<span data-ttu-id="d80d2-213">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="d80d2-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="d80d2-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="d80d2-215">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-215">Boolean</span></span>|<span data-ttu-id="d80d2-216">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="d80d2-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="d80d2-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="d80d2-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="d80d2-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-218">Boolean</span></span>|<span data-ttu-id="d80d2-219">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="d80d2-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="d80d2-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="d80d2-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d80d2-221">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-221">Boolean</span></span>|<span data-ttu-id="d80d2-222">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="d80d2-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d80d2-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="d80d2-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d80d2-224">Int32</span><span class="sxs-lookup"><span data-stu-id="d80d2-224">Int32</span></span>|<span data-ttu-id="d80d2-225">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="d80d2-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d80d2-226">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="d80d2-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d80d2-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="d80d2-227">enableSharedIPad</span></span>|<span data-ttu-id="d80d2-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="d80d2-228">Boolean</span></span>|<span data-ttu-id="d80d2-229">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="d80d2-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d80d2-230">仅适用于共享 ipad。</span><span class="sxs-lookup"><span data-stu-id="d80d2-230">Only applicable in shared iPads.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d80d2-231">关系</span><span class="sxs-lookup"><span data-stu-id="d80d2-231">Relationships</span></span>
<span data-ttu-id="d80d2-232">无</span><span class="sxs-lookup"><span data-stu-id="d80d2-232">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d80d2-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d80d2-233">JSON Representation</span></span>
<span data-ttu-id="d80d2-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d80d2-234">Here is a JSON representation of the resource.</span></span>
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





