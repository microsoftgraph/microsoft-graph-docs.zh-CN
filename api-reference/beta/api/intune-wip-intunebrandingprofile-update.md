---
title: 更新 intuneBrandingProfile
description: 更新 intuneBrandingProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aaad8b8c79ba0600df26e0081d0c6a9450ae03ba
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793085"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="41957-103">更新 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="41957-103">Update intuneBrandingProfile</span></span>

<span data-ttu-id="41957-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41957-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41957-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41957-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41957-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41957-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41957-107">更新 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41957-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41957-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41957-108">Prerequisites</span></span>
<span data-ttu-id="41957-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41957-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41957-111">Permission type</span></span>|<span data-ttu-id="41957-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41957-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41957-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41957-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41957-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41957-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41957-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41957-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41957-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41957-116">Not supported.</span></span>|
|<span data-ttu-id="41957-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41957-117">Application</span></span>|<span data-ttu-id="41957-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41957-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41957-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41957-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="41957-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41957-120">Request headers</span></span>
|<span data-ttu-id="41957-121">标头</span><span class="sxs-lookup"><span data-stu-id="41957-121">Header</span></span>|<span data-ttu-id="41957-122">值</span><span class="sxs-lookup"><span data-stu-id="41957-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41957-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41957-123">Authorization</span></span>|<span data-ttu-id="41957-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41957-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41957-125">接受</span><span class="sxs-lookup"><span data-stu-id="41957-125">Accept</span></span>|<span data-ttu-id="41957-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41957-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41957-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41957-127">Request body</span></span>
<span data-ttu-id="41957-128">在请求正文中，提供 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41957-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="41957-129">下表显示创建 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41957-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="41957-130">属性</span><span class="sxs-lookup"><span data-stu-id="41957-130">Property</span></span>|<span data-ttu-id="41957-131">类型</span><span class="sxs-lookup"><span data-stu-id="41957-131">Type</span></span>|<span data-ttu-id="41957-132">说明</span><span class="sxs-lookup"><span data-stu-id="41957-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41957-133">id</span><span class="sxs-lookup"><span data-stu-id="41957-133">id</span></span>|<span data-ttu-id="41957-134">String</span><span class="sxs-lookup"><span data-stu-id="41957-134">String</span></span>|<span data-ttu-id="41957-135">配置文件键</span><span class="sxs-lookup"><span data-stu-id="41957-135">Profile Key</span></span>|
|<span data-ttu-id="41957-136">profileName</span><span class="sxs-lookup"><span data-stu-id="41957-136">profileName</span></span>|<span data-ttu-id="41957-137">String</span><span class="sxs-lookup"><span data-stu-id="41957-137">String</span></span>|<span data-ttu-id="41957-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="41957-138">Name of the profile</span></span>|
|<span data-ttu-id="41957-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="41957-139">profileDescription</span></span>|<span data-ttu-id="41957-140">String</span><span class="sxs-lookup"><span data-stu-id="41957-140">String</span></span>|<span data-ttu-id="41957-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="41957-141">Description of the profile</span></span>|
|<span data-ttu-id="41957-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="41957-142">isDefaultProfile</span></span>|<span data-ttu-id="41957-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-143">Boolean</span></span>|<span data-ttu-id="41957-144">一个 Boolean 类型的值，该值表示是否将配置文件用作默认配置文件</span><span class="sxs-lookup"><span data-stu-id="41957-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="41957-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41957-145">createdDateTime</span></span>|<span data-ttu-id="41957-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41957-146">DateTimeOffset</span></span>|<span data-ttu-id="41957-147">创建 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="41957-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="41957-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41957-148">lastModifiedDateTime</span></span>|<span data-ttu-id="41957-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41957-149">DateTimeOffset</span></span>|<span data-ttu-id="41957-150">上次修改 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="41957-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="41957-151">displayName</span><span class="sxs-lookup"><span data-stu-id="41957-151">displayName</span></span>|<span data-ttu-id="41957-152">String</span><span class="sxs-lookup"><span data-stu-id="41957-152">String</span></span>|<span data-ttu-id="41957-153">向最终用户显示的公司/组织名称</span><span class="sxs-lookup"><span data-stu-id="41957-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="41957-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="41957-154">themeColor</span></span>|[<span data-ttu-id="41957-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="41957-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="41957-156">公司门户应用程序和 web 门户中使用的主要主题颜色</span><span class="sxs-lookup"><span data-stu-id="41957-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="41957-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="41957-157">showLogo</span></span>|<span data-ttu-id="41957-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-158">Boolean</span></span>|<span data-ttu-id="41957-159">Boolean 类型的值，该值表示是否显示管理员提供的徽标图像</span><span class="sxs-lookup"><span data-stu-id="41957-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="41957-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="41957-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="41957-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-161">Boolean</span></span>|<span data-ttu-id="41957-162">一个 Boolean 类型的值，该值表示是否在徽标图像旁边显示管理员提供的显示名称</span><span class="sxs-lookup"><span data-stu-id="41957-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="41957-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="41957-163">themeColorLogo</span></span>|[<span data-ttu-id="41957-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="41957-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="41957-165">在公司门户应用程序中显示的徽标图像，其徽标后面有主题颜色背景</span><span class="sxs-lookup"><span data-stu-id="41957-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="41957-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="41957-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="41957-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="41957-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="41957-168">在公司门户应用程序中显示的徽标图像，徽标后面有浅背景</span><span class="sxs-lookup"><span data-stu-id="41957-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="41957-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="41957-169">landingPageCustomizedImage</span></span>|[<span data-ttu-id="41957-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="41957-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="41957-171">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="41957-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="41957-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="41957-172">contactITName</span></span>|<span data-ttu-id="41957-173">String</span><span class="sxs-lookup"><span data-stu-id="41957-173">String</span></span>|<span data-ttu-id="41957-174">负责 IT 支持的人员/组织的名称</span><span class="sxs-lookup"><span data-stu-id="41957-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="41957-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="41957-175">contactITPhoneNumber</span></span>|<span data-ttu-id="41957-176">String</span><span class="sxs-lookup"><span data-stu-id="41957-176">String</span></span>|<span data-ttu-id="41957-177">负责 IT 支持的个人/组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="41957-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="41957-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="41957-178">contactITEmailAddress</span></span>|<span data-ttu-id="41957-179">String</span><span class="sxs-lookup"><span data-stu-id="41957-179">String</span></span>|<span data-ttu-id="41957-180">负责 IT 支持的个人/组织的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="41957-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="41957-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="41957-181">contactITNotes</span></span>|<span data-ttu-id="41957-182">String</span><span class="sxs-lookup"><span data-stu-id="41957-182">String</span></span>|<span data-ttu-id="41957-183">关于负责 IT 支持的人员/组织的文本注释</span><span class="sxs-lookup"><span data-stu-id="41957-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="41957-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="41957-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="41957-185">String</span><span class="sxs-lookup"><span data-stu-id="41957-185">String</span></span>|<span data-ttu-id="41957-186">指向公司/组织的 IT 支持人员网站的 URL</span><span class="sxs-lookup"><span data-stu-id="41957-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="41957-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="41957-187">onlineSupportSiteName</span></span>|<span data-ttu-id="41957-188">String</span><span class="sxs-lookup"><span data-stu-id="41957-188">String</span></span>|<span data-ttu-id="41957-189">公司/组织的 IT 支持人员网站的显示名称</span><span class="sxs-lookup"><span data-stu-id="41957-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="41957-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="41957-190">privacyUrl</span></span>|<span data-ttu-id="41957-191">String</span><span class="sxs-lookup"><span data-stu-id="41957-191">String</span></span>|<span data-ttu-id="41957-192">指向公司/组织的隐私策略的 URL</span><span class="sxs-lookup"><span data-stu-id="41957-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="41957-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="41957-193">customPrivacyMessage</span></span>|<span data-ttu-id="41957-194">String</span><span class="sxs-lookup"><span data-stu-id="41957-194">String</span></span>|<span data-ttu-id="41957-195">有关管理员在设备上没有访问权限的文本注释</span><span class="sxs-lookup"><span data-stu-id="41957-195">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="41957-196">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="41957-196">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="41957-197">String</span><span class="sxs-lookup"><span data-stu-id="41957-197">String</span></span>|<span data-ttu-id="41957-198">有关管理员在设备上有权访问的内容的文本注释</span><span class="sxs-lookup"><span data-stu-id="41957-198">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="41957-199">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="41957-199">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="41957-200">String</span><span class="sxs-lookup"><span data-stu-id="41957-200">String</span></span>|<span data-ttu-id="41957-201">有关管理员在设备上没有访问权限的文本注释</span><span class="sxs-lookup"><span data-stu-id="41957-201">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="41957-202">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="41957-202">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="41957-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-203">Boolean</span></span>|<span data-ttu-id="41957-204">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="41957-204">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="41957-205">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="41957-205">isFactoryResetDisabled</span></span>|<span data-ttu-id="41957-206">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-206">Boolean</span></span>|<span data-ttu-id="41957-207">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="41957-207">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="41957-208">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="41957-208">companyPortalBlockedActions</span></span>|<span data-ttu-id="41957-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41957-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="41957-210">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="41957-210">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="41957-211">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="41957-211">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="41957-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-212">Boolean</span></span>|<span data-ttu-id="41957-213">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-213">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="41957-214">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="41957-214">showOfficeWebApps</span></span>|<span data-ttu-id="41957-215">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-215">Boolean</span></span>|<span data-ttu-id="41957-216">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-216">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="41957-217">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="41957-217">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="41957-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="41957-218">Boolean</span></span>|<span data-ttu-id="41957-219">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="41957-219">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="41957-220">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="41957-220">enrollmentAvailability</span></span>|[<span data-ttu-id="41957-221">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="41957-221">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="41957-222">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="41957-222">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="41957-223">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="41957-223">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="41957-224">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41957-224">roleScopeTagIds</span></span>|<span data-ttu-id="41957-225">字符串集合</span><span class="sxs-lookup"><span data-stu-id="41957-225">String collection</span></span>|<span data-ttu-id="41957-226">分配给品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="41957-226">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="41957-227">响应</span><span class="sxs-lookup"><span data-stu-id="41957-227">Response</span></span>
<span data-ttu-id="41957-228">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41957-228">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41957-229">示例</span><span class="sxs-lookup"><span data-stu-id="41957-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="41957-230">请求</span><span class="sxs-lookup"><span data-stu-id="41957-230">Request</span></span>
<span data-ttu-id="41957-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41957-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1940

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
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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

### <a name="response"></a><span data-ttu-id="41957-232">响应</span><span class="sxs-lookup"><span data-stu-id="41957-232">Response</span></span>
<span data-ttu-id="41957-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41957-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2112

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
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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



