---
title: 创建 intuneBrandingProfile
description: 创建新的 intuneBrandingProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7cff26042555067056683dac65ad98d2e9d51df
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195312"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="73813-103">创建 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="73813-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="73813-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73813-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73813-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73813-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73813-106">创建新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73813-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73813-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="73813-107">Prerequisites</span></span>
<span data-ttu-id="73813-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73813-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="73813-110">Permission type</span></span>|<span data-ttu-id="73813-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73813-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73813-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73813-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73813-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73813-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73813-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73813-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73813-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="73813-115">Not supported.</span></span>|
|<span data-ttu-id="73813-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="73813-116">Application</span></span>|<span data-ttu-id="73813-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73813-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73813-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73813-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="73813-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73813-119">Request headers</span></span>
|<span data-ttu-id="73813-120">标头</span><span class="sxs-lookup"><span data-stu-id="73813-120">Header</span></span>|<span data-ttu-id="73813-121">值</span><span class="sxs-lookup"><span data-stu-id="73813-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73813-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73813-122">Authorization</span></span>|<span data-ttu-id="73813-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73813-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73813-124">接受</span><span class="sxs-lookup"><span data-stu-id="73813-124">Accept</span></span>|<span data-ttu-id="73813-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73813-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73813-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73813-126">Request body</span></span>
<span data-ttu-id="73813-127">在请求正文中，提供 intuneBrandingProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73813-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="73813-128">下表显示创建 intuneBrandingProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73813-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="73813-129">属性</span><span class="sxs-lookup"><span data-stu-id="73813-129">Property</span></span>|<span data-ttu-id="73813-130">类型</span><span class="sxs-lookup"><span data-stu-id="73813-130">Type</span></span>|<span data-ttu-id="73813-131">说明</span><span class="sxs-lookup"><span data-stu-id="73813-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73813-132">id</span><span class="sxs-lookup"><span data-stu-id="73813-132">id</span></span>|<span data-ttu-id="73813-133">String</span><span class="sxs-lookup"><span data-stu-id="73813-133">String</span></span>|<span data-ttu-id="73813-134">配置文件键</span><span class="sxs-lookup"><span data-stu-id="73813-134">Profile Key</span></span>|
|<span data-ttu-id="73813-135">profileName</span><span class="sxs-lookup"><span data-stu-id="73813-135">profileName</span></span>|<span data-ttu-id="73813-136">String</span><span class="sxs-lookup"><span data-stu-id="73813-136">String</span></span>|<span data-ttu-id="73813-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="73813-137">Name of the profile</span></span>|
|<span data-ttu-id="73813-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="73813-138">profileDescription</span></span>|<span data-ttu-id="73813-139">String</span><span class="sxs-lookup"><span data-stu-id="73813-139">String</span></span>|<span data-ttu-id="73813-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="73813-140">Description of the profile</span></span>|
|<span data-ttu-id="73813-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="73813-141">isDefaultProfile</span></span>|<span data-ttu-id="73813-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="73813-142">Boolean</span></span>|<span data-ttu-id="73813-143">一个 Boolean 类型的值，该值表示是否将配置文件用作默认配置文件</span><span class="sxs-lookup"><span data-stu-id="73813-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="73813-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73813-144">createdDateTime</span></span>|<span data-ttu-id="73813-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73813-145">DateTimeOffset</span></span>|<span data-ttu-id="73813-146">创建 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="73813-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="73813-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73813-147">lastModifiedDateTime</span></span>|<span data-ttu-id="73813-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73813-148">DateTimeOffset</span></span>|<span data-ttu-id="73813-149">上次修改 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="73813-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="73813-150">displayName</span><span class="sxs-lookup"><span data-stu-id="73813-150">displayName</span></span>|<span data-ttu-id="73813-151">字符串</span><span class="sxs-lookup"><span data-stu-id="73813-151">String</span></span>|<span data-ttu-id="73813-152">向最终用户显示的公司/组织名称</span><span class="sxs-lookup"><span data-stu-id="73813-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="73813-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="73813-153">contactITName</span></span>|<span data-ttu-id="73813-154">String</span><span class="sxs-lookup"><span data-stu-id="73813-154">String</span></span>|<span data-ttu-id="73813-155">负责 IT 支持的人员/组织的名称</span><span class="sxs-lookup"><span data-stu-id="73813-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="73813-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="73813-156">contactITPhoneNumber</span></span>|<span data-ttu-id="73813-157">String</span><span class="sxs-lookup"><span data-stu-id="73813-157">String</span></span>|<span data-ttu-id="73813-158">负责 IT 支持的个人/组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="73813-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="73813-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="73813-159">contactITEmailAddress</span></span>|<span data-ttu-id="73813-160">String</span><span class="sxs-lookup"><span data-stu-id="73813-160">String</span></span>|<span data-ttu-id="73813-161">负责 IT 支持的个人/组织的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="73813-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="73813-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="73813-162">contactITNotes</span></span>|<span data-ttu-id="73813-163">String</span><span class="sxs-lookup"><span data-stu-id="73813-163">String</span></span>|<span data-ttu-id="73813-164">关于负责 IT 支持的人员/组织的文本注释</span><span class="sxs-lookup"><span data-stu-id="73813-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="73813-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="73813-165">privacyUrl</span></span>|<span data-ttu-id="73813-166">String</span><span class="sxs-lookup"><span data-stu-id="73813-166">String</span></span>|<span data-ttu-id="73813-167">指向公司/组织的隐私策略的 URL</span><span class="sxs-lookup"><span data-stu-id="73813-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="73813-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="73813-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="73813-169">String</span><span class="sxs-lookup"><span data-stu-id="73813-169">String</span></span>|<span data-ttu-id="73813-170">指向公司/组织的 IT 支持人员网站的 URL</span><span class="sxs-lookup"><span data-stu-id="73813-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="73813-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="73813-171">onlineSupportSiteName</span></span>|<span data-ttu-id="73813-172">String</span><span class="sxs-lookup"><span data-stu-id="73813-172">String</span></span>|<span data-ttu-id="73813-173">公司/组织的 IT 支持人员网站的显示名称</span><span class="sxs-lookup"><span data-stu-id="73813-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="73813-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="73813-174">themeColor</span></span>|[<span data-ttu-id="73813-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="73813-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="73813-176">公司门户应用程序和 web 门户中使用的主要主题颜色</span><span class="sxs-lookup"><span data-stu-id="73813-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="73813-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="73813-177">showLogo</span></span>|<span data-ttu-id="73813-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="73813-178">Boolean</span></span>|<span data-ttu-id="73813-179">Boolean 类型的值，该值表示是否显示管理员提供的徽标图像</span><span class="sxs-lookup"><span data-stu-id="73813-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="73813-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="73813-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="73813-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="73813-181">Boolean</span></span>|<span data-ttu-id="73813-182">一个 Boolean 类型的值，该值表示是否在徽标图像旁边显示管理员提供的显示名称</span><span class="sxs-lookup"><span data-stu-id="73813-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="73813-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="73813-183">themeColorLogo</span></span>|[<span data-ttu-id="73813-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73813-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73813-185">在公司门户应用程序中显示的徽标图像，其徽标后面有主题颜色背景</span><span class="sxs-lookup"><span data-stu-id="73813-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="73813-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="73813-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="73813-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73813-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73813-188">在公司门户应用程序中显示的徽标图像，徽标后面有浅背景</span><span class="sxs-lookup"><span data-stu-id="73813-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="73813-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="73813-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="73813-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73813-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73813-191">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="73813-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="73813-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="73813-192">customPrivacyMessage</span></span>|<span data-ttu-id="73813-193">String</span><span class="sxs-lookup"><span data-stu-id="73813-193">String</span></span>|<span data-ttu-id="73813-194">有关管理员在设备上有权访问的内容的文本注释</span><span class="sxs-lookup"><span data-stu-id="73813-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="73813-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="73813-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="73813-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="73813-196">Boolean</span></span>|<span data-ttu-id="73813-197">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="73813-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="73813-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="73813-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="73813-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="73813-199">Boolean</span></span>|<span data-ttu-id="73813-200">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="73813-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|



## <a name="response"></a><span data-ttu-id="73813-201">响应</span><span class="sxs-lookup"><span data-stu-id="73813-201">Response</span></span>
<span data-ttu-id="73813-202">如果成功，此方法在响应`201 Created`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73813-202">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73813-203">示例</span><span class="sxs-lookup"><span data-stu-id="73813-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="73813-204">请求</span><span class="sxs-lookup"><span data-stu-id="73813-204">Request</span></span>
<span data-ttu-id="73813-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73813-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="73813-206">响应</span><span class="sxs-lookup"><span data-stu-id="73813-206">Response</span></span>
<span data-ttu-id="73813-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73813-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```




