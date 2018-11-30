---
title: 更新 intuneBrandingProfile
description: 更新 intuneBrandingProfile 对象的属性。
ms.openlocfilehash: 094de592e0e8d80472f1b0c6ed3d751ac79ba863
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048791"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="0f03e-103">更新 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="0f03e-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="0f03e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0f03e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f03e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f03e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f03e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0f03e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f03e-107">更新[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0f03e-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f03e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f03e-108">Prerequisites</span></span>
<span data-ttu-id="0f03e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0f03e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f03e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f03e-111">Permission type</span></span>|<span data-ttu-id="0f03e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f03e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f03e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f03e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f03e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f03e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f03e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f03e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f03e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f03e-116">Not supported.</span></span>|
|<span data-ttu-id="0f03e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f03e-117">Application</span></span>|<span data-ttu-id="0f03e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f03e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f03e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f03e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0f03e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f03e-120">Request headers</span></span>
|<span data-ttu-id="0f03e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0f03e-121">Header</span></span>|<span data-ttu-id="0f03e-122">值</span><span class="sxs-lookup"><span data-stu-id="0f03e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f03e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f03e-123">Authorization</span></span>|<span data-ttu-id="0f03e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f03e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f03e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f03e-125">Accept</span></span>|<span data-ttu-id="0f03e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f03e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f03e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f03e-127">Request body</span></span>
<span data-ttu-id="0f03e-128">在请求正文中，提供[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f03e-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="0f03e-129">下表显示时创建[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f03e-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="0f03e-130">属性</span><span class="sxs-lookup"><span data-stu-id="0f03e-130">Property</span></span>|<span data-ttu-id="0f03e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0f03e-131">Type</span></span>|<span data-ttu-id="0f03e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0f03e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f03e-133">id</span><span class="sxs-lookup"><span data-stu-id="0f03e-133">id</span></span>|<span data-ttu-id="0f03e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0f03e-134">String</span></span>|<span data-ttu-id="0f03e-135">配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="0f03e-135">Profile Key</span></span>|
|<span data-ttu-id="0f03e-136">profileName</span><span class="sxs-lookup"><span data-stu-id="0f03e-136">profileName</span></span>|<span data-ttu-id="0f03e-137">字符串</span><span class="sxs-lookup"><span data-stu-id="0f03e-137">String</span></span>|<span data-ttu-id="0f03e-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="0f03e-138">Name of the profile</span></span>|
|<span data-ttu-id="0f03e-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="0f03e-139">profileDescription</span></span>|<span data-ttu-id="0f03e-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0f03e-140">String</span></span>|<span data-ttu-id="0f03e-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="0f03e-141">Description of the profile</span></span>|
|<span data-ttu-id="0f03e-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="0f03e-142">isDefaultProfile</span></span>|<span data-ttu-id="0f03e-143">布尔</span><span class="sxs-lookup"><span data-stu-id="0f03e-143">Boolean</span></span>|<span data-ttu-id="0f03e-144">如果在配置文件使用的默认，呈现。</span><span class="sxs-lookup"><span data-stu-id="0f03e-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="0f03e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f03e-145">createdDateTime</span></span>|<span data-ttu-id="0f03e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f03e-146">DateTimeOffset</span></span>|<span data-ttu-id="0f03e-147">创建 BrandingProfile 时。</span><span class="sxs-lookup"><span data-stu-id="0f03e-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="0f03e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f03e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0f03e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f03e-149">DateTimeOffset</span></span>|<span data-ttu-id="0f03e-150">当 BrandingProfile 上次修改。</span><span class="sxs-lookup"><span data-stu-id="0f03e-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="0f03e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="0f03e-151">displayName</span></span>|<span data-ttu-id="0f03e-152">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-152">String</span></span>|<span data-ttu-id="0f03e-153">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="0f03e-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="0f03e-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="0f03e-154">contactITName</span></span>|<span data-ttu-id="0f03e-155">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-155">String</span></span>|<span data-ttu-id="0f03e-156">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="0f03e-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0f03e-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0f03e-157">contactITPhoneNumber</span></span>|<span data-ttu-id="0f03e-158">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-158">String</span></span>|<span data-ttu-id="0f03e-159">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="0f03e-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0f03e-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0f03e-160">contactITEmailAddress</span></span>|<span data-ttu-id="0f03e-161">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-161">String</span></span>|<span data-ttu-id="0f03e-162">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0f03e-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0f03e-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="0f03e-163">contactITNotes</span></span>|<span data-ttu-id="0f03e-164">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-164">String</span></span>|<span data-ttu-id="0f03e-165">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="0f03e-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0f03e-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="0f03e-166">privacyUrl</span></span>|<span data-ttu-id="0f03e-167">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-167">String</span></span>|<span data-ttu-id="0f03e-168">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="0f03e-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="0f03e-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="0f03e-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="0f03e-170">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-170">String</span></span>|<span data-ttu-id="0f03e-171">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="0f03e-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="0f03e-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="0f03e-172">onlineSupportSiteName</span></span>|<span data-ttu-id="0f03e-173">String</span><span class="sxs-lookup"><span data-stu-id="0f03e-173">String</span></span>|<span data-ttu-id="0f03e-174">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="0f03e-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="0f03e-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="0f03e-175">themeColor</span></span>|[<span data-ttu-id="0f03e-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="0f03e-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="0f03e-177">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="0f03e-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="0f03e-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="0f03e-178">showLogo</span></span>|<span data-ttu-id="0f03e-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="0f03e-179">Boolean</span></span>|<span data-ttu-id="0f03e-180">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0f03e-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="0f03e-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="0f03e-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="0f03e-182">布尔值</span><span class="sxs-lookup"><span data-stu-id="0f03e-182">Boolean</span></span>|<span data-ttu-id="0f03e-183">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0f03e-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="0f03e-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="0f03e-184">themeColorLogo</span></span>|[<span data-ttu-id="0f03e-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f03e-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f03e-186">主题颜色背景上的公司门户应用程序中显示的徽标图像。</span><span class="sxs-lookup"><span data-stu-id="0f03e-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="0f03e-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="0f03e-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="0f03e-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f03e-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f03e-189">浅色背景上的公司门户应用程序中显示的徽标图像。</span><span class="sxs-lookup"><span data-stu-id="0f03e-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="0f03e-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="0f03e-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="0f03e-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f03e-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f03e-192">自定义登录页的公司门户应用程序中显示的图像</span><span class="sxs-lookup"><span data-stu-id="0f03e-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="0f03e-193">响应</span><span class="sxs-lookup"><span data-stu-id="0f03e-193">Response</span></span>
<span data-ttu-id="0f03e-194">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f03e-194">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f03e-195">示例</span><span class="sxs-lookup"><span data-stu-id="0f03e-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f03e-196">请求</span><span class="sxs-lookup"><span data-stu-id="0f03e-196">Request</span></span>
<span data-ttu-id="0f03e-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f03e-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1209

{
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
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

### <a name="response"></a><span data-ttu-id="0f03e-198">响应</span><span class="sxs-lookup"><span data-stu-id="0f03e-198">Response</span></span>
<span data-ttu-id="0f03e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f03e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





