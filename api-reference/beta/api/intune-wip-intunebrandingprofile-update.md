---
title: 更新 intuneBrandingProfile
description: 更新 intuneBrandingProfile 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: caaac4d731181efe19731eed6b0340e8d08b98ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799707"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="da7bb-103">更新 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="da7bb-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="da7bb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da7bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da7bb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da7bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da7bb-106">更新[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da7bb-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da7bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da7bb-107">Prerequisites</span></span>
<span data-ttu-id="da7bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da7bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da7bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da7bb-110">Permission type</span></span>|<span data-ttu-id="da7bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da7bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da7bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da7bb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7bb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da7bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da7bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da7bb-115">Not supported.</span></span>|
|<span data-ttu-id="da7bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da7bb-116">Application</span></span>|<span data-ttu-id="da7bb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7bb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da7bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="da7bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da7bb-119">Request headers</span></span>
|<span data-ttu-id="da7bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="da7bb-120">Header</span></span>|<span data-ttu-id="da7bb-121">值</span><span class="sxs-lookup"><span data-stu-id="da7bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da7bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da7bb-122">Authorization</span></span>|<span data-ttu-id="da7bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da7bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da7bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="da7bb-124">Accept</span></span>|<span data-ttu-id="da7bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da7bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da7bb-126">Request body</span></span>
<span data-ttu-id="da7bb-127">在请求正文中，提供[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da7bb-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="da7bb-128">下表显示创建[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da7bb-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="da7bb-129">属性</span><span class="sxs-lookup"><span data-stu-id="da7bb-129">Property</span></span>|<span data-ttu-id="da7bb-130">类型</span><span class="sxs-lookup"><span data-stu-id="da7bb-130">Type</span></span>|<span data-ttu-id="da7bb-131">说明</span><span class="sxs-lookup"><span data-stu-id="da7bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da7bb-132">id</span><span class="sxs-lookup"><span data-stu-id="da7bb-132">id</span></span>|<span data-ttu-id="da7bb-133">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-133">String</span></span>|<span data-ttu-id="da7bb-134">配置文件键</span><span class="sxs-lookup"><span data-stu-id="da7bb-134">Profile Key</span></span>|
|<span data-ttu-id="da7bb-135">profileName</span><span class="sxs-lookup"><span data-stu-id="da7bb-135">profileName</span></span>|<span data-ttu-id="da7bb-136">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-136">String</span></span>|<span data-ttu-id="da7bb-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="da7bb-137">Name of the profile</span></span>|
|<span data-ttu-id="da7bb-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="da7bb-138">profileDescription</span></span>|<span data-ttu-id="da7bb-139">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-139">String</span></span>|<span data-ttu-id="da7bb-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="da7bb-140">Description of the profile</span></span>|
|<span data-ttu-id="da7bb-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="da7bb-141">isDefaultProfile</span></span>|<span data-ttu-id="da7bb-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-142">Boolean</span></span>|<span data-ttu-id="da7bb-143">一个 Boolean 类型的值，该值表示是否将配置文件用作默认配置文件</span><span class="sxs-lookup"><span data-stu-id="da7bb-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="da7bb-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da7bb-144">createdDateTime</span></span>|<span data-ttu-id="da7bb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7bb-145">DateTimeOffset</span></span>|<span data-ttu-id="da7bb-146">创建 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="da7bb-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="da7bb-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da7bb-147">lastModifiedDateTime</span></span>|<span data-ttu-id="da7bb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7bb-148">DateTimeOffset</span></span>|<span data-ttu-id="da7bb-149">上次修改 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="da7bb-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="da7bb-150">displayName</span><span class="sxs-lookup"><span data-stu-id="da7bb-150">displayName</span></span>|<span data-ttu-id="da7bb-151">字符串</span><span class="sxs-lookup"><span data-stu-id="da7bb-151">String</span></span>|<span data-ttu-id="da7bb-152">向最终用户显示的公司/组织名称</span><span class="sxs-lookup"><span data-stu-id="da7bb-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="da7bb-153">themeColor</span><span class="sxs-lookup"><span data-stu-id="da7bb-153">themeColor</span></span>|[<span data-ttu-id="da7bb-154">rgbColor</span><span class="sxs-lookup"><span data-stu-id="da7bb-154">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="da7bb-155">公司门户应用程序和 web 门户中使用的主要主题颜色</span><span class="sxs-lookup"><span data-stu-id="da7bb-155">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="da7bb-156">showLogo</span><span class="sxs-lookup"><span data-stu-id="da7bb-156">showLogo</span></span>|<span data-ttu-id="da7bb-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-157">Boolean</span></span>|<span data-ttu-id="da7bb-158">Boolean 类型的值，该值表示是否显示管理员提供的徽标图像</span><span class="sxs-lookup"><span data-stu-id="da7bb-158">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="da7bb-159">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="da7bb-159">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="da7bb-160">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-160">Boolean</span></span>|<span data-ttu-id="da7bb-161">一个 Boolean 类型的值，该值表示是否在徽标图像旁边显示管理员提供的显示名称</span><span class="sxs-lookup"><span data-stu-id="da7bb-161">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="da7bb-162">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="da7bb-162">themeColorLogo</span></span>|[<span data-ttu-id="da7bb-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da7bb-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="da7bb-164">在公司门户应用程序中显示的徽标图像，其徽标后面有主题颜色背景</span><span class="sxs-lookup"><span data-stu-id="da7bb-164">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="da7bb-165">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="da7bb-165">lightBackgroundLogo</span></span>|[<span data-ttu-id="da7bb-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da7bb-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="da7bb-167">在公司门户应用程序中显示的徽标图像，徽标后面有浅背景</span><span class="sxs-lookup"><span data-stu-id="da7bb-167">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="da7bb-168">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="da7bb-168">landingPageCustomizedImage</span></span>|[<span data-ttu-id="da7bb-169">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da7bb-169">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="da7bb-170">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="da7bb-170">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="da7bb-171">contactITName</span><span class="sxs-lookup"><span data-stu-id="da7bb-171">contactITName</span></span>|<span data-ttu-id="da7bb-172">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-172">String</span></span>|<span data-ttu-id="da7bb-173">负责 IT 支持的人员/组织的名称</span><span class="sxs-lookup"><span data-stu-id="da7bb-173">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="da7bb-174">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="da7bb-174">contactITPhoneNumber</span></span>|<span data-ttu-id="da7bb-175">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-175">String</span></span>|<span data-ttu-id="da7bb-176">负责 IT 支持的个人/组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="da7bb-176">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="da7bb-177">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="da7bb-177">contactITEmailAddress</span></span>|<span data-ttu-id="da7bb-178">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-178">String</span></span>|<span data-ttu-id="da7bb-179">负责 IT 支持的个人/组织的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="da7bb-179">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="da7bb-180">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="da7bb-180">contactITNotes</span></span>|<span data-ttu-id="da7bb-181">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-181">String</span></span>|<span data-ttu-id="da7bb-182">关于负责 IT 支持的人员/组织的文本注释</span><span class="sxs-lookup"><span data-stu-id="da7bb-182">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="da7bb-183">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="da7bb-183">onlineSupportSiteUrl</span></span>|<span data-ttu-id="da7bb-184">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-184">String</span></span>|<span data-ttu-id="da7bb-185">指向公司/组织的 IT 支持人员网站的 URL</span><span class="sxs-lookup"><span data-stu-id="da7bb-185">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="da7bb-186">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="da7bb-186">onlineSupportSiteName</span></span>|<span data-ttu-id="da7bb-187">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-187">String</span></span>|<span data-ttu-id="da7bb-188">公司/组织的 IT 支持人员网站的显示名称</span><span class="sxs-lookup"><span data-stu-id="da7bb-188">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="da7bb-189">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="da7bb-189">privacyUrl</span></span>|<span data-ttu-id="da7bb-190">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-190">String</span></span>|<span data-ttu-id="da7bb-191">指向公司/组织的隐私策略的 URL</span><span class="sxs-lookup"><span data-stu-id="da7bb-191">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="da7bb-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="da7bb-192">customPrivacyMessage</span></span>|<span data-ttu-id="da7bb-193">String</span><span class="sxs-lookup"><span data-stu-id="da7bb-193">String</span></span>|<span data-ttu-id="da7bb-194">有关管理员在设备上有权访问的内容的文本注释</span><span class="sxs-lookup"><span data-stu-id="da7bb-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="da7bb-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="da7bb-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="da7bb-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-196">Boolean</span></span>|<span data-ttu-id="da7bb-197">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="da7bb-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="da7bb-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="da7bb-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="da7bb-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-199">Boolean</span></span>|<span data-ttu-id="da7bb-200">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="da7bb-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="da7bb-201">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="da7bb-201">companyPortalBlockedActions</span></span>|<span data-ttu-id="da7bb-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="da7bb-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="da7bb-203">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="da7bb-203">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="da7bb-204">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="da7bb-204">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="da7bb-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-205">Boolean</span></span>|<span data-ttu-id="da7bb-206">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-206">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="da7bb-207">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="da7bb-207">showOfficeWebApps</span></span>|<span data-ttu-id="da7bb-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-208">Boolean</span></span>|<span data-ttu-id="da7bb-209">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-209">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="da7bb-210">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="da7bb-210">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="da7bb-211">布尔值</span><span class="sxs-lookup"><span data-stu-id="da7bb-211">Boolean</span></span>|<span data-ttu-id="da7bb-212">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="da7bb-212">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="da7bb-213">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="da7bb-213">enrollmentAvailability</span></span>|[<span data-ttu-id="da7bb-214">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="da7bb-214">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="da7bb-215">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="da7bb-215">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="da7bb-216">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="da7bb-216">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="da7bb-217">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da7bb-217">roleScopeTagIds</span></span>|<span data-ttu-id="da7bb-218">String collection</span><span class="sxs-lookup"><span data-stu-id="da7bb-218">String collection</span></span>|<span data-ttu-id="da7bb-219">分配给品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="da7bb-219">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="da7bb-220">响应</span><span class="sxs-lookup"><span data-stu-id="da7bb-220">Response</span></span>
<span data-ttu-id="da7bb-221">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da7bb-221">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7bb-222">示例</span><span class="sxs-lookup"><span data-stu-id="da7bb-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="da7bb-223">请求</span><span class="sxs-lookup"><span data-stu-id="da7bb-223">Request</span></span>
<span data-ttu-id="da7bb-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da7bb-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1792

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="da7bb-225">响应</span><span class="sxs-lookup"><span data-stu-id="da7bb-225">Response</span></span>
<span data-ttu-id="da7bb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da7bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




