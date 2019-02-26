---
title: 更新 intuneBrandingProfile
description: 更新 intuneBrandingProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a66589e4be7d5cc175c792935e2f309c8f28e33
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162340"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="28387-103">更新 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="28387-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="28387-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28387-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28387-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28387-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28387-106">更新[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28387-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28387-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="28387-107">Prerequisites</span></span>
<span data-ttu-id="28387-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="28387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28387-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28387-110">Permission type</span></span>|<span data-ttu-id="28387-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="28387-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28387-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28387-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28387-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28387-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28387-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28387-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28387-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28387-115">Not supported.</span></span>|
|<span data-ttu-id="28387-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28387-116">Application</span></span>|<span data-ttu-id="28387-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="28387-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28387-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28387-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="28387-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28387-119">Request headers</span></span>
|<span data-ttu-id="28387-120">标头</span><span class="sxs-lookup"><span data-stu-id="28387-120">Header</span></span>|<span data-ttu-id="28387-121">值</span><span class="sxs-lookup"><span data-stu-id="28387-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28387-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28387-122">Authorization</span></span>|<span data-ttu-id="28387-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28387-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28387-124">Accept</span><span class="sxs-lookup"><span data-stu-id="28387-124">Accept</span></span>|<span data-ttu-id="28387-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28387-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28387-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28387-126">Request body</span></span>
<span data-ttu-id="28387-127">在请求正文中, 提供[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28387-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="28387-128">下表显示创建[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28387-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="28387-129">属性</span><span class="sxs-lookup"><span data-stu-id="28387-129">Property</span></span>|<span data-ttu-id="28387-130">类型</span><span class="sxs-lookup"><span data-stu-id="28387-130">Type</span></span>|<span data-ttu-id="28387-131">说明</span><span class="sxs-lookup"><span data-stu-id="28387-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28387-132">id</span><span class="sxs-lookup"><span data-stu-id="28387-132">id</span></span>|<span data-ttu-id="28387-133">字符串</span><span class="sxs-lookup"><span data-stu-id="28387-133">String</span></span>|<span data-ttu-id="28387-134">配置文件键</span><span class="sxs-lookup"><span data-stu-id="28387-134">Profile Key</span></span>|
|<span data-ttu-id="28387-135">profileName</span><span class="sxs-lookup"><span data-stu-id="28387-135">profileName</span></span>|<span data-ttu-id="28387-136">String</span><span class="sxs-lookup"><span data-stu-id="28387-136">String</span></span>|<span data-ttu-id="28387-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="28387-137">Name of the profile</span></span>|
|<span data-ttu-id="28387-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="28387-138">profileDescription</span></span>|<span data-ttu-id="28387-139">String</span><span class="sxs-lookup"><span data-stu-id="28387-139">String</span></span>|<span data-ttu-id="28387-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="28387-140">Description of the profile</span></span>|
|<span data-ttu-id="28387-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="28387-141">isDefaultProfile</span></span>|<span data-ttu-id="28387-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="28387-142">Boolean</span></span>|<span data-ttu-id="28387-143">显示配置文件是否用于默认设置。</span><span class="sxs-lookup"><span data-stu-id="28387-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="28387-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28387-144">createdDateTime</span></span>|<span data-ttu-id="28387-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28387-145">DateTimeOffset</span></span>|<span data-ttu-id="28387-146">创建 BrandingProfile 时。</span><span class="sxs-lookup"><span data-stu-id="28387-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="28387-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28387-147">lastModifiedDateTime</span></span>|<span data-ttu-id="28387-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28387-148">DateTimeOffset</span></span>|<span data-ttu-id="28387-149">上次修改 BrandingProfile 的时间。</span><span class="sxs-lookup"><span data-stu-id="28387-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="28387-150">displayName</span><span class="sxs-lookup"><span data-stu-id="28387-150">displayName</span></span>|<span data-ttu-id="28387-151">String</span><span class="sxs-lookup"><span data-stu-id="28387-151">String</span></span>|<span data-ttu-id="28387-152">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="28387-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="28387-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="28387-153">contactITName</span></span>|<span data-ttu-id="28387-154">String</span><span class="sxs-lookup"><span data-stu-id="28387-154">String</span></span>|<span data-ttu-id="28387-155">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="28387-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28387-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="28387-156">contactITPhoneNumber</span></span>|<span data-ttu-id="28387-157">String</span><span class="sxs-lookup"><span data-stu-id="28387-157">String</span></span>|<span data-ttu-id="28387-158">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="28387-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28387-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="28387-159">contactITEmailAddress</span></span>|<span data-ttu-id="28387-160">String</span><span class="sxs-lookup"><span data-stu-id="28387-160">String</span></span>|<span data-ttu-id="28387-161">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="28387-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28387-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="28387-162">contactITNotes</span></span>|<span data-ttu-id="28387-163">String</span><span class="sxs-lookup"><span data-stu-id="28387-163">String</span></span>|<span data-ttu-id="28387-164">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="28387-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28387-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="28387-165">privacyUrl</span></span>|<span data-ttu-id="28387-166">String</span><span class="sxs-lookup"><span data-stu-id="28387-166">String</span></span>|<span data-ttu-id="28387-167">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="28387-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="28387-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="28387-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="28387-169">String</span><span class="sxs-lookup"><span data-stu-id="28387-169">String</span></span>|<span data-ttu-id="28387-170">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="28387-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="28387-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="28387-171">onlineSupportSiteName</span></span>|<span data-ttu-id="28387-172">String</span><span class="sxs-lookup"><span data-stu-id="28387-172">String</span></span>|<span data-ttu-id="28387-173">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="28387-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="28387-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="28387-174">themeColor</span></span>|[<span data-ttu-id="28387-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="28387-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="28387-176">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="28387-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="28387-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="28387-177">showLogo</span></span>|<span data-ttu-id="28387-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="28387-178">Boolean</span></span>|<span data-ttu-id="28387-179">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="28387-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="28387-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="28387-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="28387-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="28387-181">Boolean</span></span>|<span data-ttu-id="28387-182">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="28387-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="28387-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="28387-183">themeColorLogo</span></span>|[<span data-ttu-id="28387-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28387-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28387-185">在主题颜色背景上的公司门户应用程序中显示的徽标图像。</span><span class="sxs-lookup"><span data-stu-id="28387-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="28387-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="28387-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="28387-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28387-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28387-188">在 "浅色背景" 的公司门户应用程序中显示的徽标图像。</span><span class="sxs-lookup"><span data-stu-id="28387-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="28387-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="28387-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="28387-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28387-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28387-191">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="28387-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="28387-192">响应</span><span class="sxs-lookup"><span data-stu-id="28387-192">Response</span></span>
<span data-ttu-id="28387-193">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28387-193">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28387-194">示例</span><span class="sxs-lookup"><span data-stu-id="28387-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="28387-195">请求</span><span class="sxs-lookup"><span data-stu-id="28387-195">Request</span></span>
<span data-ttu-id="28387-196">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28387-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
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

### <a name="response"></a><span data-ttu-id="28387-197">响应</span><span class="sxs-lookup"><span data-stu-id="28387-197">Response</span></span>
<span data-ttu-id="28387-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28387-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




