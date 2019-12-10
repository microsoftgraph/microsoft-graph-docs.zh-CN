---
title: 更新 intuneBrandingProfile
description: 更新 intuneBrandingProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cd72b310ad29e5ff32520945d63a80f7fb1b370
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938472"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="fa6d1-103">更新 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="fa6d1-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="fa6d1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa6d1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa6d1-106">更新[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa6d1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa6d1-107">Prerequisites</span></span>
<span data-ttu-id="fa6d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa6d1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa6d1-110">Permission type</span></span>|<span data-ttu-id="fa6d1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa6d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa6d1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa6d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa6d1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa6d1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa6d1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa6d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa6d1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-115">Not supported.</span></span>|
|<span data-ttu-id="fa6d1-116">Application</span><span class="sxs-lookup"><span data-stu-id="fa6d1-116">Application</span></span>|<span data-ttu-id="fa6d1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa6d1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa6d1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa6d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="fa6d1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa6d1-119">Request headers</span></span>
|<span data-ttu-id="fa6d1-120">标头</span><span class="sxs-lookup"><span data-stu-id="fa6d1-120">Header</span></span>|<span data-ttu-id="fa6d1-121">值</span><span class="sxs-lookup"><span data-stu-id="fa6d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa6d1-122">授权</span><span class="sxs-lookup"><span data-stu-id="fa6d1-122">Authorization</span></span>|<span data-ttu-id="fa6d1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa6d1-124">接受</span><span class="sxs-lookup"><span data-stu-id="fa6d1-124">Accept</span></span>|<span data-ttu-id="fa6d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa6d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa6d1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa6d1-126">Request body</span></span>
<span data-ttu-id="fa6d1-127">在请求正文中，提供[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="fa6d1-128">下表显示创建[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="fa6d1-129">属性</span><span class="sxs-lookup"><span data-stu-id="fa6d1-129">Property</span></span>|<span data-ttu-id="fa6d1-130">类型</span><span class="sxs-lookup"><span data-stu-id="fa6d1-130">Type</span></span>|<span data-ttu-id="fa6d1-131">说明</span><span class="sxs-lookup"><span data-stu-id="fa6d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa6d1-132">id</span><span class="sxs-lookup"><span data-stu-id="fa6d1-132">id</span></span>|<span data-ttu-id="fa6d1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-133">String</span></span>|<span data-ttu-id="fa6d1-134">配置文件键</span><span class="sxs-lookup"><span data-stu-id="fa6d1-134">Profile Key</span></span>|
|<span data-ttu-id="fa6d1-135">profileName</span><span class="sxs-lookup"><span data-stu-id="fa6d1-135">profileName</span></span>|<span data-ttu-id="fa6d1-136">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-136">String</span></span>|<span data-ttu-id="fa6d1-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="fa6d1-137">Name of the profile</span></span>|
|<span data-ttu-id="fa6d1-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="fa6d1-138">profileDescription</span></span>|<span data-ttu-id="fa6d1-139">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-139">String</span></span>|<span data-ttu-id="fa6d1-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="fa6d1-140">Description of the profile</span></span>|
|<span data-ttu-id="fa6d1-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="fa6d1-141">isDefaultProfile</span></span>|<span data-ttu-id="fa6d1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d1-142">Boolean</span></span>|<span data-ttu-id="fa6d1-143">一个 Boolean 类型的值，该值表示是否将配置文件用作默认配置文件</span><span class="sxs-lookup"><span data-stu-id="fa6d1-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="fa6d1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa6d1-144">createdDateTime</span></span>|<span data-ttu-id="fa6d1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa6d1-145">DateTimeOffset</span></span>|<span data-ttu-id="fa6d1-146">创建 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="fa6d1-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="fa6d1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa6d1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="fa6d1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa6d1-148">DateTimeOffset</span></span>|<span data-ttu-id="fa6d1-149">上次修改 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="fa6d1-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="fa6d1-150">displayName</span><span class="sxs-lookup"><span data-stu-id="fa6d1-150">displayName</span></span>|<span data-ttu-id="fa6d1-151">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-151">String</span></span>|<span data-ttu-id="fa6d1-152">向最终用户显示的公司/组织名称</span><span class="sxs-lookup"><span data-stu-id="fa6d1-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="fa6d1-153">themeColor</span><span class="sxs-lookup"><span data-stu-id="fa6d1-153">themeColor</span></span>|[<span data-ttu-id="fa6d1-154">rgbColor</span><span class="sxs-lookup"><span data-stu-id="fa6d1-154">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="fa6d1-155">公司门户应用程序和 web 门户中使用的主要主题颜色</span><span class="sxs-lookup"><span data-stu-id="fa6d1-155">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="fa6d1-156">showLogo</span><span class="sxs-lookup"><span data-stu-id="fa6d1-156">showLogo</span></span>|<span data-ttu-id="fa6d1-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d1-157">Boolean</span></span>|<span data-ttu-id="fa6d1-158">Boolean 类型的值，该值表示是否显示管理员提供的徽标图像</span><span class="sxs-lookup"><span data-stu-id="fa6d1-158">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="fa6d1-159">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="fa6d1-159">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="fa6d1-160">布尔值</span><span class="sxs-lookup"><span data-stu-id="fa6d1-160">Boolean</span></span>|<span data-ttu-id="fa6d1-161">一个 Boolean 类型的值，该值表示是否在徽标图像旁边显示管理员提供的显示名称</span><span class="sxs-lookup"><span data-stu-id="fa6d1-161">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="fa6d1-162">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="fa6d1-162">themeColorLogo</span></span>|[<span data-ttu-id="fa6d1-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fa6d1-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fa6d1-164">在公司门户应用程序中显示的徽标图像，其徽标后面有主题颜色背景</span><span class="sxs-lookup"><span data-stu-id="fa6d1-164">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="fa6d1-165">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="fa6d1-165">lightBackgroundLogo</span></span>|[<span data-ttu-id="fa6d1-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fa6d1-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fa6d1-167">在公司门户应用程序中显示的徽标图像，徽标后面有浅背景</span><span class="sxs-lookup"><span data-stu-id="fa6d1-167">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="fa6d1-168">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="fa6d1-168">landingPageCustomizedImage</span></span>|[<span data-ttu-id="fa6d1-169">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fa6d1-169">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fa6d1-170">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="fa6d1-170">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="fa6d1-171">contactITName</span><span class="sxs-lookup"><span data-stu-id="fa6d1-171">contactITName</span></span>|<span data-ttu-id="fa6d1-172">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-172">String</span></span>|<span data-ttu-id="fa6d1-173">负责 IT 支持的人员/组织的名称</span><span class="sxs-lookup"><span data-stu-id="fa6d1-173">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="fa6d1-174">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fa6d1-174">contactITPhoneNumber</span></span>|<span data-ttu-id="fa6d1-175">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-175">String</span></span>|<span data-ttu-id="fa6d1-176">负责 IT 支持的个人/组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="fa6d1-176">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="fa6d1-177">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fa6d1-177">contactITEmailAddress</span></span>|<span data-ttu-id="fa6d1-178">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-178">String</span></span>|<span data-ttu-id="fa6d1-179">负责 IT 支持的个人/组织的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="fa6d1-179">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="fa6d1-180">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="fa6d1-180">contactITNotes</span></span>|<span data-ttu-id="fa6d1-181">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-181">String</span></span>|<span data-ttu-id="fa6d1-182">关于负责 IT 支持的人员/组织的文本注释</span><span class="sxs-lookup"><span data-stu-id="fa6d1-182">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="fa6d1-183">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="fa6d1-183">onlineSupportSiteUrl</span></span>|<span data-ttu-id="fa6d1-184">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-184">String</span></span>|<span data-ttu-id="fa6d1-185">指向公司/组织的 IT 支持人员网站的 URL</span><span class="sxs-lookup"><span data-stu-id="fa6d1-185">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="fa6d1-186">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="fa6d1-186">onlineSupportSiteName</span></span>|<span data-ttu-id="fa6d1-187">String</span><span class="sxs-lookup"><span data-stu-id="fa6d1-187">String</span></span>|<span data-ttu-id="fa6d1-188">公司/组织的 IT 支持人员网站的显示名称</span><span class="sxs-lookup"><span data-stu-id="fa6d1-188">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="fa6d1-189">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="fa6d1-189">privacyUrl</span></span>|<span data-ttu-id="fa6d1-190">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-190">String</span></span>|<span data-ttu-id="fa6d1-191">指向公司/组织的隐私策略的 URL</span><span class="sxs-lookup"><span data-stu-id="fa6d1-191">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="fa6d1-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="fa6d1-192">customPrivacyMessage</span></span>|<span data-ttu-id="fa6d1-193">字符串</span><span class="sxs-lookup"><span data-stu-id="fa6d1-193">String</span></span>|<span data-ttu-id="fa6d1-194">有关管理员在设备上有权访问的内容的文本注释</span><span class="sxs-lookup"><span data-stu-id="fa6d1-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="fa6d1-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="fa6d1-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="fa6d1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d1-196">Boolean</span></span>|<span data-ttu-id="fa6d1-197">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="fa6d1-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="fa6d1-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="fa6d1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d1-199">Boolean</span></span>|<span data-ttu-id="fa6d1-200">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="fa6d1-201">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="fa6d1-201">companyPortalBlockedActions</span></span>|<span data-ttu-id="fa6d1-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="fa6d1-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="fa6d1-203">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-203">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="fa6d1-204">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="fa6d1-204">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="fa6d1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d1-205">Boolean</span></span>|<span data-ttu-id="fa6d1-206">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="fa6d1-206">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="fa6d1-207">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="fa6d1-207">showOfficeWebApps</span></span>|<span data-ttu-id="fa6d1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d1-208">Boolean</span></span>|<span data-ttu-id="fa6d1-209">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="fa6d1-209">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|



## <a name="response"></a><span data-ttu-id="fa6d1-210">响应</span><span class="sxs-lookup"><span data-stu-id="fa6d1-210">Response</span></span>
<span data-ttu-id="fa6d1-211">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-211">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa6d1-212">示例</span><span class="sxs-lookup"><span data-stu-id="fa6d1-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa6d1-213">请求</span><span class="sxs-lookup"><span data-stu-id="fa6d1-213">Request</span></span>
<span data-ttu-id="fa6d1-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1620

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
  "showOfficeWebApps": true
}
```

### <a name="response"></a><span data-ttu-id="fa6d1-215">响应</span><span class="sxs-lookup"><span data-stu-id="fa6d1-215">Response</span></span>
<span data-ttu-id="fa6d1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa6d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1792

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
  "showOfficeWebApps": true
}
```





