---
title: depEnrollmentProfile 资源类型
description: DepEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 594831e981da3779f075d8481df57dd3cd68ac66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080325"
---
# <a name="depenrollmentprofile-resource-type"></a><span data-ttu-id="ba2ee-104">depEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba2ee-104">depEnrollmentProfile resource type</span></span>

<span data-ttu-id="ba2ee-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2ee-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba2ee-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba2ee-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba2ee-108">DepEnrollmentProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-108">The depEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="ba2ee-109">在相应的设备可以通过 DEP 进行注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="ba2ee-110">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba2ee-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ba2ee-111">方法</span><span class="sxs-lookup"><span data-stu-id="ba2ee-111">Methods</span></span>
|<span data-ttu-id="ba2ee-112">方法</span><span class="sxs-lookup"><span data-stu-id="ba2ee-112">Method</span></span>|<span data-ttu-id="ba2ee-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba2ee-113">Return Type</span></span>|<span data-ttu-id="ba2ee-114">说明</span><span class="sxs-lookup"><span data-stu-id="ba2ee-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba2ee-115">列出 depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="ba2ee-115">List depEnrollmentProfiles</span></span>](../api/intune-enrollment-depenrollmentprofile-list.md)|<span data-ttu-id="ba2ee-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba2ee-116">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) collection</span></span>|<span data-ttu-id="ba2ee-117">列出 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-117">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="ba2ee-118">获取 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-118">Get depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-get.md)|[<span data-ttu-id="ba2ee-119">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-119">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="ba2ee-120">读取 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-120">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="ba2ee-121">创建 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-121">Create depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-create.md)|[<span data-ttu-id="ba2ee-122">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-122">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="ba2ee-123">创建新的 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-123">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="ba2ee-124">删除 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-124">Delete depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-delete.md)|<span data-ttu-id="ba2ee-125">无</span><span class="sxs-lookup"><span data-stu-id="ba2ee-125">None</span></span>|<span data-ttu-id="ba2ee-126">删除 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-126">Deletes a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="ba2ee-127">更新 depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-127">Update depEnrollmentProfile</span></span>](../api/intune-enrollment-depenrollmentprofile-update.md)|[<span data-ttu-id="ba2ee-128">depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ba2ee-128">depEnrollmentProfile</span></span>](../resources/intune-enrollment-depenrollmentprofile.md)|<span data-ttu-id="ba2ee-129">更新 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-129">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba2ee-130">属性</span><span class="sxs-lookup"><span data-stu-id="ba2ee-130">Properties</span></span>
|<span data-ttu-id="ba2ee-131">属性</span><span class="sxs-lookup"><span data-stu-id="ba2ee-131">Property</span></span>|<span data-ttu-id="ba2ee-132">类型</span><span class="sxs-lookup"><span data-stu-id="ba2ee-132">Type</span></span>|<span data-ttu-id="ba2ee-133">说明</span><span class="sxs-lookup"><span data-stu-id="ba2ee-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba2ee-134">id</span><span class="sxs-lookup"><span data-stu-id="ba2ee-134">id</span></span>|<span data-ttu-id="ba2ee-135">String</span><span class="sxs-lookup"><span data-stu-id="ba2ee-135">String</span></span>|<span data-ttu-id="ba2ee-136">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="ba2ee-136">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ba2ee-137">displayName</span></span>|<span data-ttu-id="ba2ee-138">String</span><span class="sxs-lookup"><span data-stu-id="ba2ee-138">String</span></span>|<span data-ttu-id="ba2ee-139">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="ba2ee-139">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-140">说明</span><span class="sxs-lookup"><span data-stu-id="ba2ee-140">description</span></span>|<span data-ttu-id="ba2ee-141">String</span><span class="sxs-lookup"><span data-stu-id="ba2ee-141">String</span></span>|<span data-ttu-id="ba2ee-142">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="ba2ee-142">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-143">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ba2ee-143">requiresUserAuthentication</span></span>|<span data-ttu-id="ba2ee-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-144">Boolean</span></span>|<span data-ttu-id="ba2ee-145">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="ba2ee-145">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-146">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ba2ee-146">configurationEndpointUrl</span></span>|<span data-ttu-id="ba2ee-147">String</span><span class="sxs-lookup"><span data-stu-id="ba2ee-147">String</span></span>|<span data-ttu-id="ba2ee-148">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="ba2ee-148">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-149">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ba2ee-149">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ba2ee-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-150">Boolean</span></span>|<span data-ttu-id="ba2ee-151">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-151">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ba2ee-152">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba2ee-152">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-153">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ba2ee-153">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ba2ee-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-154">Boolean</span></span>|<span data-ttu-id="ba2ee-155">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="ba2ee-155">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba2ee-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="ba2ee-156">isDefault</span></span>|<span data-ttu-id="ba2ee-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-157">Boolean</span></span>|<span data-ttu-id="ba2ee-158">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="ba2ee-158">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ba2ee-159">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-159">supervisedModeEnabled</span></span>|<span data-ttu-id="ba2ee-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-160">Boolean</span></span>|<span data-ttu-id="ba2ee-161">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-161">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ba2ee-162">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-162">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ba2ee-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ba2ee-163">supportDepartment</span></span>|<span data-ttu-id="ba2ee-164">String</span><span class="sxs-lookup"><span data-stu-id="ba2ee-164">String</span></span>|<span data-ttu-id="ba2ee-165">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="ba2ee-165">Support department information</span></span>|
|<span data-ttu-id="ba2ee-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-166">passCodeDisabled</span></span>|<span data-ttu-id="ba2ee-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-167">Boolean</span></span>|<span data-ttu-id="ba2ee-168">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-168">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ba2ee-169">isMandatory</span></span>|<span data-ttu-id="ba2ee-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-170">Boolean</span></span>|<span data-ttu-id="ba2ee-171">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="ba2ee-171">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ba2ee-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-172">locationDisabled</span></span>|<span data-ttu-id="ba2ee-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-173">Boolean</span></span>|<span data-ttu-id="ba2ee-174">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-174">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ba2ee-175">supportPhoneNumber</span></span>|<span data-ttu-id="ba2ee-176">String</span><span class="sxs-lookup"><span data-stu-id="ba2ee-176">String</span></span>|<span data-ttu-id="ba2ee-177">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="ba2ee-177">Support phone number</span></span>|
|<span data-ttu-id="ba2ee-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ba2ee-178">iTunesPairingMode</span></span>|[<span data-ttu-id="ba2ee-179">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ba2ee-179">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="ba2ee-180">指示 iTunes 配对模式。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-180">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="ba2ee-181">可取值为：`disallow`、`allow`、`requiresCertificate`。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-181">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="ba2ee-182">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-182">profileRemovalDisabled</span></span>|<span data-ttu-id="ba2ee-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-183">Boolean</span></span>|<span data-ttu-id="ba2ee-184">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="ba2ee-184">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ba2ee-185">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="ba2ee-185">managementCertificates</span></span>|<span data-ttu-id="ba2ee-186">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba2ee-186">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="ba2ee-187">Apple 配置器的管理证书</span><span class="sxs-lookup"><span data-stu-id="ba2ee-187">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="ba2ee-188">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ba2ee-188">restoreBlocked</span></span>|<span data-ttu-id="ba2ee-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-189">Boolean</span></span>|<span data-ttu-id="ba2ee-190">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-190">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ba2ee-191">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-191">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="ba2ee-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-192">Boolean</span></span>|<span data-ttu-id="ba2ee-193">指示是否禁用从 Android 还原</span><span class="sxs-lookup"><span data-stu-id="ba2ee-193">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="ba2ee-194">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-194">appleIdDisabled</span></span>|<span data-ttu-id="ba2ee-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-195">Boolean</span></span>|<span data-ttu-id="ba2ee-196">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-196">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-197">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-197">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ba2ee-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-198">Boolean</span></span>|<span data-ttu-id="ba2ee-199">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-199">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-200">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-200">touchIdDisabled</span></span>|<span data-ttu-id="ba2ee-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-201">Boolean</span></span>|<span data-ttu-id="ba2ee-202">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-202">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-203">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-203">applePayDisabled</span></span>|<span data-ttu-id="ba2ee-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-204">Boolean</span></span>|<span data-ttu-id="ba2ee-205">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-205">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-206">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-206">zoomDisabled</span></span>|<span data-ttu-id="ba2ee-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-207">Boolean</span></span>|<span data-ttu-id="ba2ee-208">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-208">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-209">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-209">siriDisabled</span></span>|<span data-ttu-id="ba2ee-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-210">Boolean</span></span>|<span data-ttu-id="ba2ee-211">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-211">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-212">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-212">diagnosticsDisabled</span></span>|<span data-ttu-id="ba2ee-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-213">Boolean</span></span>|<span data-ttu-id="ba2ee-214">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="ba2ee-214">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="ba2ee-215">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-215">macOSRegistrationDisabled</span></span>|<span data-ttu-id="ba2ee-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-216">Boolean</span></span>|<span data-ttu-id="ba2ee-217">指示是否禁用 Mac OS 注册</span><span class="sxs-lookup"><span data-stu-id="ba2ee-217">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="ba2ee-218">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="ba2ee-218">macOSFileVaultDisabled</span></span>|<span data-ttu-id="ba2ee-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-219">Boolean</span></span>|<span data-ttu-id="ba2ee-220">指示是否禁用 Mac OS 文件保管库</span><span class="sxs-lookup"><span data-stu-id="ba2ee-220">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="ba2ee-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="ba2ee-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="ba2ee-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-222">Boolean</span></span>|<span data-ttu-id="ba2ee-223">指示设备是否需要等待已配置的确认</span><span class="sxs-lookup"><span data-stu-id="ba2ee-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="ba2ee-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="ba2ee-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="ba2ee-225">Int32</span><span class="sxs-lookup"><span data-stu-id="ba2ee-225">Int32</span></span>|<span data-ttu-id="ba2ee-226">这指定了可以使用共享 iPad 的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="ba2ee-227">仅适用于共享 iPad 模式。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="ba2ee-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="ba2ee-228">enableSharedIPad</span></span>|<span data-ttu-id="ba2ee-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba2ee-229">Boolean</span></span>|<span data-ttu-id="ba2ee-230">这表示设备是否要在启用多用户方案的模式中进行注册。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="ba2ee-231">仅适用于共享 Ipad。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-231">Only applicable in shared iPads.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba2ee-232">关系</span><span class="sxs-lookup"><span data-stu-id="ba2ee-232">Relationships</span></span>
<span data-ttu-id="ba2ee-233">无</span><span class="sxs-lookup"><span data-stu-id="ba2ee-233">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba2ee-234">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba2ee-234">JSON Representation</span></span>
<span data-ttu-id="ba2ee-235">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba2ee-235">Here is a JSON representation of the resource.</span></span>
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






