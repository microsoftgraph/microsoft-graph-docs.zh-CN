---
title: 创建 intuneBrandingProfile
description: 创建新的 intuneBrandingProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5112d2d3ccfa90459fb363588f05c8dd3ceb7aee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457459"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="554ee-103">创建 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="554ee-103">Create intuneBrandingProfile</span></span>

<span data-ttu-id="554ee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="554ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="554ee-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="554ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="554ee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="554ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="554ee-107">创建新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="554ee-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="554ee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="554ee-108">Prerequisites</span></span>
<span data-ttu-id="554ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="554ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="554ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="554ee-111">Permission type</span></span>|<span data-ttu-id="554ee-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="554ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="554ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="554ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="554ee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="554ee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="554ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="554ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="554ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="554ee-116">Not supported.</span></span>|
|<span data-ttu-id="554ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="554ee-117">Application</span></span>|<span data-ttu-id="554ee-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="554ee-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="554ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="554ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="554ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="554ee-120">Request headers</span></span>
|<span data-ttu-id="554ee-121">标头</span><span class="sxs-lookup"><span data-stu-id="554ee-121">Header</span></span>|<span data-ttu-id="554ee-122">值</span><span class="sxs-lookup"><span data-stu-id="554ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="554ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="554ee-123">Authorization</span></span>|<span data-ttu-id="554ee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="554ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="554ee-125">接受</span><span class="sxs-lookup"><span data-stu-id="554ee-125">Accept</span></span>|<span data-ttu-id="554ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="554ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="554ee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="554ee-127">Request body</span></span>
<span data-ttu-id="554ee-128">在请求正文中，提供 intuneBrandingProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="554ee-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="554ee-129">下表显示创建 intuneBrandingProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="554ee-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="554ee-130">属性</span><span class="sxs-lookup"><span data-stu-id="554ee-130">Property</span></span>|<span data-ttu-id="554ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="554ee-131">Type</span></span>|<span data-ttu-id="554ee-132">说明</span><span class="sxs-lookup"><span data-stu-id="554ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="554ee-133">id</span><span class="sxs-lookup"><span data-stu-id="554ee-133">id</span></span>|<span data-ttu-id="554ee-134">String</span><span class="sxs-lookup"><span data-stu-id="554ee-134">String</span></span>|<span data-ttu-id="554ee-135">配置文件键</span><span class="sxs-lookup"><span data-stu-id="554ee-135">Profile Key</span></span>|
|<span data-ttu-id="554ee-136">profileName</span><span class="sxs-lookup"><span data-stu-id="554ee-136">profileName</span></span>|<span data-ttu-id="554ee-137">String</span><span class="sxs-lookup"><span data-stu-id="554ee-137">String</span></span>|<span data-ttu-id="554ee-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="554ee-138">Name of the profile</span></span>|
|<span data-ttu-id="554ee-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="554ee-139">profileDescription</span></span>|<span data-ttu-id="554ee-140">String</span><span class="sxs-lookup"><span data-stu-id="554ee-140">String</span></span>|<span data-ttu-id="554ee-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="554ee-141">Description of the profile</span></span>|
|<span data-ttu-id="554ee-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="554ee-142">isDefaultProfile</span></span>|<span data-ttu-id="554ee-143">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-143">Boolean</span></span>|<span data-ttu-id="554ee-144">一个 Boolean 类型的值，该值表示是否将配置文件用作默认配置文件</span><span class="sxs-lookup"><span data-stu-id="554ee-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="554ee-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="554ee-145">createdDateTime</span></span>|<span data-ttu-id="554ee-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="554ee-146">DateTimeOffset</span></span>|<span data-ttu-id="554ee-147">创建 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="554ee-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="554ee-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="554ee-148">lastModifiedDateTime</span></span>|<span data-ttu-id="554ee-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="554ee-149">DateTimeOffset</span></span>|<span data-ttu-id="554ee-150">上次修改 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="554ee-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="554ee-151">displayName</span><span class="sxs-lookup"><span data-stu-id="554ee-151">displayName</span></span>|<span data-ttu-id="554ee-152">字符串</span><span class="sxs-lookup"><span data-stu-id="554ee-152">String</span></span>|<span data-ttu-id="554ee-153">向最终用户显示的公司/组织名称</span><span class="sxs-lookup"><span data-stu-id="554ee-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="554ee-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="554ee-154">themeColor</span></span>|[<span data-ttu-id="554ee-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="554ee-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="554ee-156">公司门户应用程序和 web 门户中使用的主要主题颜色</span><span class="sxs-lookup"><span data-stu-id="554ee-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="554ee-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="554ee-157">showLogo</span></span>|<span data-ttu-id="554ee-158">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-158">Boolean</span></span>|<span data-ttu-id="554ee-159">Boolean 类型的值，该值表示是否显示管理员提供的徽标图像</span><span class="sxs-lookup"><span data-stu-id="554ee-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="554ee-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="554ee-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="554ee-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="554ee-161">Boolean</span></span>|<span data-ttu-id="554ee-162">一个 Boolean 类型的值，该值表示是否在徽标图像旁边显示管理员提供的显示名称</span><span class="sxs-lookup"><span data-stu-id="554ee-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="554ee-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="554ee-163">themeColorLogo</span></span>|[<span data-ttu-id="554ee-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="554ee-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="554ee-165">在公司门户应用程序中显示的徽标图像，其徽标后面有主题颜色背景</span><span class="sxs-lookup"><span data-stu-id="554ee-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="554ee-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="554ee-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="554ee-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="554ee-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="554ee-168">在公司门户应用程序中显示的徽标图像，徽标后面有浅背景</span><span class="sxs-lookup"><span data-stu-id="554ee-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="554ee-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="554ee-169">landingPageCustomizedImage</span></span>|[<span data-ttu-id="554ee-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="554ee-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="554ee-171">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="554ee-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="554ee-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="554ee-172">contactITName</span></span>|<span data-ttu-id="554ee-173">String</span><span class="sxs-lookup"><span data-stu-id="554ee-173">String</span></span>|<span data-ttu-id="554ee-174">负责 IT 支持的人员/组织的名称</span><span class="sxs-lookup"><span data-stu-id="554ee-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="554ee-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="554ee-175">contactITPhoneNumber</span></span>|<span data-ttu-id="554ee-176">String</span><span class="sxs-lookup"><span data-stu-id="554ee-176">String</span></span>|<span data-ttu-id="554ee-177">负责 IT 支持的个人/组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="554ee-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="554ee-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="554ee-178">contactITEmailAddress</span></span>|<span data-ttu-id="554ee-179">String</span><span class="sxs-lookup"><span data-stu-id="554ee-179">String</span></span>|<span data-ttu-id="554ee-180">负责 IT 支持的个人/组织的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="554ee-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="554ee-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="554ee-181">contactITNotes</span></span>|<span data-ttu-id="554ee-182">String</span><span class="sxs-lookup"><span data-stu-id="554ee-182">String</span></span>|<span data-ttu-id="554ee-183">关于负责 IT 支持的人员/组织的文本注释</span><span class="sxs-lookup"><span data-stu-id="554ee-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="554ee-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="554ee-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="554ee-185">String</span><span class="sxs-lookup"><span data-stu-id="554ee-185">String</span></span>|<span data-ttu-id="554ee-186">指向公司/组织的 IT 支持人员网站的 URL</span><span class="sxs-lookup"><span data-stu-id="554ee-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="554ee-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="554ee-187">onlineSupportSiteName</span></span>|<span data-ttu-id="554ee-188">String</span><span class="sxs-lookup"><span data-stu-id="554ee-188">String</span></span>|<span data-ttu-id="554ee-189">公司/组织的 IT 支持人员网站的显示名称</span><span class="sxs-lookup"><span data-stu-id="554ee-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="554ee-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="554ee-190">privacyUrl</span></span>|<span data-ttu-id="554ee-191">String</span><span class="sxs-lookup"><span data-stu-id="554ee-191">String</span></span>|<span data-ttu-id="554ee-192">指向公司/组织的隐私策略的 URL</span><span class="sxs-lookup"><span data-stu-id="554ee-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="554ee-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="554ee-193">customPrivacyMessage</span></span>|<span data-ttu-id="554ee-194">String</span><span class="sxs-lookup"><span data-stu-id="554ee-194">String</span></span>|<span data-ttu-id="554ee-195">有关管理员在设备上有权访问的内容的文本注释</span><span class="sxs-lookup"><span data-stu-id="554ee-195">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="554ee-196">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="554ee-196">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="554ee-197">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-197">Boolean</span></span>|<span data-ttu-id="554ee-198">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="554ee-198">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="554ee-199">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="554ee-199">isFactoryResetDisabled</span></span>|<span data-ttu-id="554ee-200">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-200">Boolean</span></span>|<span data-ttu-id="554ee-201">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="554ee-201">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="554ee-202">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="554ee-202">companyPortalBlockedActions</span></span>|<span data-ttu-id="554ee-203">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="554ee-203">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="554ee-204">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="554ee-204">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="554ee-205">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="554ee-205">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="554ee-206">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-206">Boolean</span></span>|<span data-ttu-id="554ee-207">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="554ee-207">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="554ee-208">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="554ee-208">showOfficeWebApps</span></span>|<span data-ttu-id="554ee-209">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-209">Boolean</span></span>|<span data-ttu-id="554ee-210">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="554ee-210">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="554ee-211">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="554ee-211">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="554ee-212">布尔</span><span class="sxs-lookup"><span data-stu-id="554ee-212">Boolean</span></span>|<span data-ttu-id="554ee-213">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="554ee-213">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="554ee-214">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="554ee-214">enrollmentAvailability</span></span>|[<span data-ttu-id="554ee-215">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="554ee-215">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="554ee-216">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="554ee-216">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="554ee-217">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="554ee-217">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="554ee-218">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="554ee-218">roleScopeTagIds</span></span>|<span data-ttu-id="554ee-219">String 集合</span><span class="sxs-lookup"><span data-stu-id="554ee-219">String collection</span></span>|<span data-ttu-id="554ee-220">分配给品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="554ee-220">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="554ee-221">响应</span><span class="sxs-lookup"><span data-stu-id="554ee-221">Response</span></span>
<span data-ttu-id="554ee-222">如果成功，此方法在响应`201 Created`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="554ee-222">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="554ee-223">示例</span><span class="sxs-lookup"><span data-stu-id="554ee-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="554ee-224">请求</span><span class="sxs-lookup"><span data-stu-id="554ee-224">Request</span></span>
<span data-ttu-id="554ee-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="554ee-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
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

### <a name="response"></a><span data-ttu-id="554ee-226">响应</span><span class="sxs-lookup"><span data-stu-id="554ee-226">Response</span></span>
<span data-ttu-id="554ee-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="554ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





