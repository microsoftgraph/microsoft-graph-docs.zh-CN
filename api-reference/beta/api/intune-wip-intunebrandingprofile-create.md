---
title: 创建 intuneBrandingProfile
description: 创建新的 intuneBrandingProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e92ad91bd5d981e987fb6d5abfd32494f6ce54de
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805514"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="65866-103">创建 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="65866-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="65866-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65866-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65866-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65866-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65866-106">创建新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65866-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65866-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="65866-107">Prerequisites</span></span>
<span data-ttu-id="65866-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65866-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="65866-110">Permission type</span></span>|<span data-ttu-id="65866-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65866-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65866-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65866-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65866-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65866-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65866-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65866-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65866-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65866-115">Not supported.</span></span>|
|<span data-ttu-id="65866-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65866-116">Application</span></span>|<span data-ttu-id="65866-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="65866-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65866-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65866-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="65866-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65866-119">Request headers</span></span>
|<span data-ttu-id="65866-120">标头</span><span class="sxs-lookup"><span data-stu-id="65866-120">Header</span></span>|<span data-ttu-id="65866-121">值</span><span class="sxs-lookup"><span data-stu-id="65866-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65866-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65866-122">Authorization</span></span>|<span data-ttu-id="65866-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65866-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65866-124">接受</span><span class="sxs-lookup"><span data-stu-id="65866-124">Accept</span></span>|<span data-ttu-id="65866-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65866-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65866-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65866-126">Request body</span></span>
<span data-ttu-id="65866-127">在请求正文中, 提供 intuneBrandingProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65866-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="65866-128">下表显示创建 intuneBrandingProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65866-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="65866-129">属性</span><span class="sxs-lookup"><span data-stu-id="65866-129">Property</span></span>|<span data-ttu-id="65866-130">类型</span><span class="sxs-lookup"><span data-stu-id="65866-130">Type</span></span>|<span data-ttu-id="65866-131">说明</span><span class="sxs-lookup"><span data-stu-id="65866-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65866-132">id</span><span class="sxs-lookup"><span data-stu-id="65866-132">id</span></span>|<span data-ttu-id="65866-133">String</span><span class="sxs-lookup"><span data-stu-id="65866-133">String</span></span>|<span data-ttu-id="65866-134">配置文件键</span><span class="sxs-lookup"><span data-stu-id="65866-134">Profile Key</span></span>|
|<span data-ttu-id="65866-135">profileName</span><span class="sxs-lookup"><span data-stu-id="65866-135">profileName</span></span>|<span data-ttu-id="65866-136">String</span><span class="sxs-lookup"><span data-stu-id="65866-136">String</span></span>|<span data-ttu-id="65866-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="65866-137">Name of the profile</span></span>|
|<span data-ttu-id="65866-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="65866-138">profileDescription</span></span>|<span data-ttu-id="65866-139">String</span><span class="sxs-lookup"><span data-stu-id="65866-139">String</span></span>|<span data-ttu-id="65866-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="65866-140">Description of the profile</span></span>|
|<span data-ttu-id="65866-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="65866-141">isDefaultProfile</span></span>|<span data-ttu-id="65866-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="65866-142">Boolean</span></span>|<span data-ttu-id="65866-143">显示配置文件是否用于默认设置。</span><span class="sxs-lookup"><span data-stu-id="65866-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="65866-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65866-144">createdDateTime</span></span>|<span data-ttu-id="65866-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65866-145">DateTimeOffset</span></span>|<span data-ttu-id="65866-146">创建 BrandingProfile 时。</span><span class="sxs-lookup"><span data-stu-id="65866-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="65866-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65866-147">lastModifiedDateTime</span></span>|<span data-ttu-id="65866-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65866-148">DateTimeOffset</span></span>|<span data-ttu-id="65866-149">上次修改 BrandingProfile 的时间。</span><span class="sxs-lookup"><span data-stu-id="65866-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="65866-150">displayName</span><span class="sxs-lookup"><span data-stu-id="65866-150">displayName</span></span>|<span data-ttu-id="65866-151">字符串</span><span class="sxs-lookup"><span data-stu-id="65866-151">String</span></span>|<span data-ttu-id="65866-152">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="65866-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="65866-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="65866-153">contactITName</span></span>|<span data-ttu-id="65866-154">String</span><span class="sxs-lookup"><span data-stu-id="65866-154">String</span></span>|<span data-ttu-id="65866-155">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="65866-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="65866-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="65866-156">contactITPhoneNumber</span></span>|<span data-ttu-id="65866-157">String</span><span class="sxs-lookup"><span data-stu-id="65866-157">String</span></span>|<span data-ttu-id="65866-158">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="65866-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="65866-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="65866-159">contactITEmailAddress</span></span>|<span data-ttu-id="65866-160">String</span><span class="sxs-lookup"><span data-stu-id="65866-160">String</span></span>|<span data-ttu-id="65866-161">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="65866-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="65866-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="65866-162">contactITNotes</span></span>|<span data-ttu-id="65866-163">String</span><span class="sxs-lookup"><span data-stu-id="65866-163">String</span></span>|<span data-ttu-id="65866-164">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="65866-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="65866-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="65866-165">privacyUrl</span></span>|<span data-ttu-id="65866-166">String</span><span class="sxs-lookup"><span data-stu-id="65866-166">String</span></span>|<span data-ttu-id="65866-167">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="65866-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="65866-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="65866-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="65866-169">String</span><span class="sxs-lookup"><span data-stu-id="65866-169">String</span></span>|<span data-ttu-id="65866-170">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="65866-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="65866-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="65866-171">onlineSupportSiteName</span></span>|<span data-ttu-id="65866-172">String</span><span class="sxs-lookup"><span data-stu-id="65866-172">String</span></span>|<span data-ttu-id="65866-173">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="65866-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="65866-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="65866-174">themeColor</span></span>|[<span data-ttu-id="65866-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="65866-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="65866-176">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="65866-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="65866-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="65866-177">showLogo</span></span>|<span data-ttu-id="65866-178">布尔值</span><span class="sxs-lookup"><span data-stu-id="65866-178">Boolean</span></span>|<span data-ttu-id="65866-179">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="65866-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="65866-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="65866-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="65866-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="65866-181">Boolean</span></span>|<span data-ttu-id="65866-182">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="65866-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="65866-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="65866-183">themeColorLogo</span></span>|[<span data-ttu-id="65866-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="65866-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="65866-185">在主题颜色背景上的公司门户应用程序中显示的徽标图像。</span><span class="sxs-lookup"><span data-stu-id="65866-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="65866-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="65866-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="65866-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="65866-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="65866-188">在 "浅色背景" 的公司门户应用程序中显示的徽标图像。</span><span class="sxs-lookup"><span data-stu-id="65866-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="65866-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="65866-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="65866-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="65866-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="65866-191">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="65866-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="65866-192">响应</span><span class="sxs-lookup"><span data-stu-id="65866-192">Response</span></span>
<span data-ttu-id="65866-193">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65866-193">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65866-194">示例</span><span class="sxs-lookup"><span data-stu-id="65866-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="65866-195">请求</span><span class="sxs-lookup"><span data-stu-id="65866-195">Request</span></span>
<span data-ttu-id="65866-196">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65866-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1205

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
  }
}
```

### <a name="response"></a><span data-ttu-id="65866-197">响应</span><span class="sxs-lookup"><span data-stu-id="65866-197">Response</span></span>
<span data-ttu-id="65866-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65866-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

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
  }
}
```





