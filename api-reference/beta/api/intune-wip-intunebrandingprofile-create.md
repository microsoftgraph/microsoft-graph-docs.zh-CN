---
title: 创建 intuneBrandingProfile
description: 创建新的 intuneBrandingProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59b5a20819e2912e88c1091627b487b898c61979
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993332"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="84d54-103">创建 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="84d54-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="84d54-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84d54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84d54-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84d54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84d54-106">创建新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84d54-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84d54-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="84d54-107">Prerequisites</span></span>
<span data-ttu-id="84d54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84d54-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84d54-110">Permission type</span></span>|<span data-ttu-id="84d54-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84d54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84d54-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84d54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84d54-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84d54-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84d54-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84d54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84d54-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84d54-115">Not supported.</span></span>|
|<span data-ttu-id="84d54-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84d54-116">Application</span></span>|<span data-ttu-id="84d54-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="84d54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84d54-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84d54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="84d54-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84d54-119">Request headers</span></span>
|<span data-ttu-id="84d54-120">标头</span><span class="sxs-lookup"><span data-stu-id="84d54-120">Header</span></span>|<span data-ttu-id="84d54-121">值</span><span class="sxs-lookup"><span data-stu-id="84d54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84d54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84d54-122">Authorization</span></span>|<span data-ttu-id="84d54-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84d54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84d54-124">接受</span><span class="sxs-lookup"><span data-stu-id="84d54-124">Accept</span></span>|<span data-ttu-id="84d54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84d54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84d54-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="84d54-126">Request body</span></span>
<span data-ttu-id="84d54-127">在请求正文中, 提供 intuneBrandingProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84d54-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="84d54-128">下表显示创建 intuneBrandingProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84d54-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="84d54-129">属性</span><span class="sxs-lookup"><span data-stu-id="84d54-129">Property</span></span>|<span data-ttu-id="84d54-130">类型</span><span class="sxs-lookup"><span data-stu-id="84d54-130">Type</span></span>|<span data-ttu-id="84d54-131">说明</span><span class="sxs-lookup"><span data-stu-id="84d54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84d54-132">id</span><span class="sxs-lookup"><span data-stu-id="84d54-132">id</span></span>|<span data-ttu-id="84d54-133">String</span><span class="sxs-lookup"><span data-stu-id="84d54-133">String</span></span>|<span data-ttu-id="84d54-134">配置文件键</span><span class="sxs-lookup"><span data-stu-id="84d54-134">Profile Key</span></span>|
|<span data-ttu-id="84d54-135">profileName</span><span class="sxs-lookup"><span data-stu-id="84d54-135">profileName</span></span>|<span data-ttu-id="84d54-136">String</span><span class="sxs-lookup"><span data-stu-id="84d54-136">String</span></span>|<span data-ttu-id="84d54-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="84d54-137">Name of the profile</span></span>|
|<span data-ttu-id="84d54-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="84d54-138">profileDescription</span></span>|<span data-ttu-id="84d54-139">String</span><span class="sxs-lookup"><span data-stu-id="84d54-139">String</span></span>|<span data-ttu-id="84d54-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="84d54-140">Description of the profile</span></span>|
|<span data-ttu-id="84d54-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="84d54-141">isDefaultProfile</span></span>|<span data-ttu-id="84d54-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="84d54-142">Boolean</span></span>|<span data-ttu-id="84d54-143">一个 Boolean 类型的值, 该值表示是否将配置文件用作默认配置文件</span><span class="sxs-lookup"><span data-stu-id="84d54-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="84d54-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84d54-144">createdDateTime</span></span>|<span data-ttu-id="84d54-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84d54-145">DateTimeOffset</span></span>|<span data-ttu-id="84d54-146">创建 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="84d54-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="84d54-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84d54-147">lastModifiedDateTime</span></span>|<span data-ttu-id="84d54-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84d54-148">DateTimeOffset</span></span>|<span data-ttu-id="84d54-149">上次修改 BrandingProfile 的时间</span><span class="sxs-lookup"><span data-stu-id="84d54-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="84d54-150">displayName</span><span class="sxs-lookup"><span data-stu-id="84d54-150">displayName</span></span>|<span data-ttu-id="84d54-151">字符串</span><span class="sxs-lookup"><span data-stu-id="84d54-151">String</span></span>|<span data-ttu-id="84d54-152">向最终用户显示的公司/组织名称</span><span class="sxs-lookup"><span data-stu-id="84d54-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="84d54-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="84d54-153">contactITName</span></span>|<span data-ttu-id="84d54-154">String</span><span class="sxs-lookup"><span data-stu-id="84d54-154">String</span></span>|<span data-ttu-id="84d54-155">负责 IT 支持的人员/组织的名称</span><span class="sxs-lookup"><span data-stu-id="84d54-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="84d54-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="84d54-156">contactITPhoneNumber</span></span>|<span data-ttu-id="84d54-157">String</span><span class="sxs-lookup"><span data-stu-id="84d54-157">String</span></span>|<span data-ttu-id="84d54-158">负责 IT 支持的个人/组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="84d54-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="84d54-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="84d54-159">contactITEmailAddress</span></span>|<span data-ttu-id="84d54-160">String</span><span class="sxs-lookup"><span data-stu-id="84d54-160">String</span></span>|<span data-ttu-id="84d54-161">负责 IT 支持的个人/组织的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="84d54-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="84d54-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="84d54-162">contactITNotes</span></span>|<span data-ttu-id="84d54-163">String</span><span class="sxs-lookup"><span data-stu-id="84d54-163">String</span></span>|<span data-ttu-id="84d54-164">关于负责 IT 支持的人员/组织的文本注释</span><span class="sxs-lookup"><span data-stu-id="84d54-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="84d54-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="84d54-165">privacyUrl</span></span>|<span data-ttu-id="84d54-166">String</span><span class="sxs-lookup"><span data-stu-id="84d54-166">String</span></span>|<span data-ttu-id="84d54-167">指向公司/组织的隐私策略的 URL</span><span class="sxs-lookup"><span data-stu-id="84d54-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="84d54-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="84d54-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="84d54-169">String</span><span class="sxs-lookup"><span data-stu-id="84d54-169">String</span></span>|<span data-ttu-id="84d54-170">指向公司/组织的 IT 支持人员网站的 URL</span><span class="sxs-lookup"><span data-stu-id="84d54-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="84d54-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="84d54-171">onlineSupportSiteName</span></span>|<span data-ttu-id="84d54-172">String</span><span class="sxs-lookup"><span data-stu-id="84d54-172">String</span></span>|<span data-ttu-id="84d54-173">公司/组织的 IT 支持人员网站的显示名称</span><span class="sxs-lookup"><span data-stu-id="84d54-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="84d54-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="84d54-174">themeColor</span></span>|[<span data-ttu-id="84d54-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="84d54-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="84d54-176">公司门户应用程序和 web 门户中使用的主要主题颜色</span><span class="sxs-lookup"><span data-stu-id="84d54-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="84d54-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="84d54-177">showLogo</span></span>|<span data-ttu-id="84d54-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="84d54-178">Boolean</span></span>|<span data-ttu-id="84d54-179">Boolean 类型的值, 该值表示是否显示管理员提供的徽标图像</span><span class="sxs-lookup"><span data-stu-id="84d54-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="84d54-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="84d54-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="84d54-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="84d54-181">Boolean</span></span>|<span data-ttu-id="84d54-182">一个 Boolean 类型的值, 该值表示是否在徽标图像旁边显示管理员提供的显示名称</span><span class="sxs-lookup"><span data-stu-id="84d54-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="84d54-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="84d54-183">themeColorLogo</span></span>|[<span data-ttu-id="84d54-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84d54-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84d54-185">在公司门户应用程序中显示的徽标图像, 其徽标后面有主题颜色背景</span><span class="sxs-lookup"><span data-stu-id="84d54-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="84d54-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="84d54-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="84d54-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84d54-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84d54-188">在公司门户应用程序中显示的徽标图像, 徽标后面有浅背景</span><span class="sxs-lookup"><span data-stu-id="84d54-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="84d54-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="84d54-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="84d54-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84d54-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84d54-191">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="84d54-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="84d54-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="84d54-192">customPrivacyMessage</span></span>|<span data-ttu-id="84d54-193">String</span><span class="sxs-lookup"><span data-stu-id="84d54-193">String</span></span>|<span data-ttu-id="84d54-194">有关管理员在设备上有权访问的内容的文本注释</span><span class="sxs-lookup"><span data-stu-id="84d54-194">Text comments regarding what the admin has access to on the device</span></span>|



## <a name="response"></a><span data-ttu-id="84d54-195">响应</span><span class="sxs-lookup"><span data-stu-id="84d54-195">Response</span></span>
<span data-ttu-id="84d54-196">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84d54-196">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d54-197">示例</span><span class="sxs-lookup"><span data-stu-id="84d54-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="84d54-198">请求</span><span class="sxs-lookup"><span data-stu-id="84d54-198">Request</span></span>
<span data-ttu-id="84d54-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84d54-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1264

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```

### <a name="response"></a><span data-ttu-id="84d54-200">响应</span><span class="sxs-lookup"><span data-stu-id="84d54-200">Response</span></span>
<span data-ttu-id="84d54-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84d54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```





