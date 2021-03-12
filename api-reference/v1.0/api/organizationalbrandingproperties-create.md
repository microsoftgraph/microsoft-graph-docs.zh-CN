---
title: 创建 organizationalBrandingProperties
description: 创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6f5e16a87f78be5e0664af624d058fff64f70bba
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722544"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="29b34-103">创建 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="29b34-103">Create organizationalBrandingProperties</span></span>

<span data-ttu-id="29b34-104">创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29b34-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="29b34-105">这将创建默认品牌和（可选）本地化品牌。</span><span class="sxs-lookup"><span data-stu-id="29b34-105">This creates the default branding and optionally a localized branding.</span></span> <span data-ttu-id="29b34-106">未为用户的浏览器语言配置本地化品牌打造集时，将加载默认品牌。</span><span class="sxs-lookup"><span data-stu-id="29b34-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="29b34-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="29b34-107">Permissions</span></span>

<span data-ttu-id="29b34-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29b34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29b34-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="29b34-110">Permission type</span></span>                        | <span data-ttu-id="29b34-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29b34-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29b34-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29b34-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="29b34-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b34-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="29b34-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29b34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29b34-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="29b34-115">Not supported.</span></span> |
| <span data-ttu-id="29b34-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="29b34-116">Application</span></span>                            | <span data-ttu-id="29b34-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="29b34-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29b34-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29b34-118">HTTP request</span></span>

<span data-ttu-id="29b34-119">使用 PUT 或 PATCH 为组织创建品牌（如果不存在）。</span><span class="sxs-lookup"><span data-stu-id="29b34-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="29b34-120">如果已配置品牌，PUT 将覆盖所有现有值，无论请求正文中有什么内容。</span><span class="sxs-lookup"><span data-stu-id="29b34-120">If branding is already configured, PUT overwrites all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="29b34-121">PATCH 仅覆盖请求正文中包含的值，保留未包含的值不变。</span><span class="sxs-lookup"><span data-stu-id="29b34-121">PATCH only overwrites the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="29b34-122">属性 `id` 在 PUT/PATCH 上忽略为 /branding singleton。</span><span class="sxs-lookup"><span data-stu-id="29b34-122">The `id` property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="29b34-123">如果 **未指定 Content-Language，** 则创建与 对应的默认 `id` 品牌 `und` 。</span><span class="sxs-lookup"><span data-stu-id="29b34-123">If **Content-Language** is not specified, the default branding is created, which corresponds to an `id` of `und`.</span></span> <span data-ttu-id="29b34-124">如果 **指定了 Content-Language，** 则针对该区域设置创建品牌。</span><span class="sxs-lookup"><span data-stu-id="29b34-124">If **Content-Language** is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="29b34-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="29b34-125">Request headers</span></span>

| <span data-ttu-id="29b34-126">名称</span><span class="sxs-lookup"><span data-stu-id="29b34-126">Name</span></span>      |<span data-ttu-id="29b34-127">说明</span><span class="sxs-lookup"><span data-stu-id="29b34-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29b34-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="29b34-128">Authorization</span></span> | <span data-ttu-id="29b34-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29b34-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29b34-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29b34-131">Content-Type</span></span>  | <span data-ttu-id="29b34-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="29b34-p106">application/json. Required.</span></span>  |
| <span data-ttu-id="29b34-134">Content-Language</span><span class="sxs-lookup"><span data-stu-id="29b34-134">Content-Language</span></span>  | <span data-ttu-id="29b34-135">区域设置。</span><span class="sxs-lookup"><span data-stu-id="29b34-135">Locale.</span></span> <span data-ttu-id="29b34-136">可选。</span><span class="sxs-lookup"><span data-stu-id="29b34-136">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29b34-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="29b34-137">Request body</span></span>

<span data-ttu-id="29b34-138">在请求正文中，包括 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29b34-138">In the request body, include a JSON representation of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="29b34-139">下表列出了所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29b34-139">The following table lists the required properties.</span></span>

| <span data-ttu-id="29b34-140">属性</span><span class="sxs-lookup"><span data-stu-id="29b34-140">Property</span></span>     | <span data-ttu-id="29b34-141">类型</span><span class="sxs-lookup"><span data-stu-id="29b34-141">Type</span></span>        | <span data-ttu-id="29b34-142">说明</span><span class="sxs-lookup"><span data-stu-id="29b34-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29b34-143">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="29b34-143">backgroundColor</span></span>|<span data-ttu-id="29b34-144">字符串</span><span class="sxs-lookup"><span data-stu-id="29b34-144">String</span></span>|<span data-ttu-id="29b34-145">在低带宽连接中显示用于背景图像的颜色。</span><span class="sxs-lookup"><span data-stu-id="29b34-145">Color that appears in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="29b34-146">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="29b34-146">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="29b34-147">以十六进制表示 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="29b34-147">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="29b34-148">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="29b34-148">backgroundImage</span></span>|<span data-ttu-id="29b34-149">Stream</span><span class="sxs-lookup"><span data-stu-id="29b34-149">Stream</span></span>|<span data-ttu-id="29b34-150">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="29b34-150">Image that appears as the background of the sign-in page.</span></span> <span data-ttu-id="29b34-151">图像是一个不大于 1920x1080 且小于 300kb 的 .png 或 .jpg。</span><span class="sxs-lookup"><span data-stu-id="29b34-151">The image is a .png or .jpg that is not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="29b34-152">较小的图像将降低带宽要求，提高页面加载性能。</span><span class="sxs-lookup"><span data-stu-id="29b34-152">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="29b34-153">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="29b34-153">bannerLogo</span></span>|<span data-ttu-id="29b34-154">Stream</span><span class="sxs-lookup"><span data-stu-id="29b34-154">Stream</span></span>|<span data-ttu-id="29b34-155">显示在登录页上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="29b34-155">A banner version of your company logo that appears on the sign-in page.</span></span> <span data-ttu-id="29b34-156">横幅是一个不超过 36x245px 的 .png 或 .jpg。</span><span class="sxs-lookup"><span data-stu-id="29b34-156">The banner is a .png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="29b34-157">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="29b34-157">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="29b34-158">signInPageText</span><span class="sxs-lookup"><span data-stu-id="29b34-158">signInPageText</span></span>|<span data-ttu-id="29b34-159">字符串</span><span class="sxs-lookup"><span data-stu-id="29b34-159">String</span></span>|<span data-ttu-id="29b34-160">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="29b34-160">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="29b34-161">您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="29b34-161">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="29b34-162">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="29b34-162">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="29b34-163">squareLogo</span><span class="sxs-lookup"><span data-stu-id="29b34-163">squareLogo</span></span>|<span data-ttu-id="29b34-164">Stream</span><span class="sxs-lookup"><span data-stu-id="29b34-164">Stream</span></span>|<span data-ttu-id="29b34-165">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="29b34-165">Square version of your company logo.</span></span> <span data-ttu-id="29b34-166">这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="29b34-166">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="29b34-167">徽标是大小不超过 240x240px 且不超过 10kb 的 .png 或 .jpg。</span><span class="sxs-lookup"><span data-stu-id="29b34-167">The logo is a .png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="29b34-168">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="29b34-168">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="29b34-169">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="29b34-169">usernameHintText</span></span>|<span data-ttu-id="29b34-170">字符串</span><span class="sxs-lookup"><span data-stu-id="29b34-170">String</span></span>|<span data-ttu-id="29b34-171">登录屏幕上用户名文本框中的提示。</span><span class="sxs-lookup"><span data-stu-id="29b34-171">The hint in the username textbox on the sign-in screen.</span></span> <span data-ttu-id="29b34-172">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="29b34-172">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="29b34-173">响应</span><span class="sxs-lookup"><span data-stu-id="29b34-173">Response</span></span>

<span data-ttu-id="29b34-174">如果成功，此方法在响应正文中返回 响应代码和创建的 `201 Created` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29b34-174">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29b34-175">示例</span><span class="sxs-lookup"><span data-stu-id="29b34-175">Examples</span></span>

<span data-ttu-id="29b34-176">下面的示例创建 **Content-Language** 为 的默认品牌和本地化 `en-US` 。</span><span class="sxs-lookup"><span data-stu-id="29b34-176">The following example creates default branding and localization where **Content-Language** is `en-US`.</span></span>

### <a name="request"></a><span data-ttu-id="29b34-177">请求</span><span class="sxs-lookup"><span data-stu-id="29b34-177">Request</span></span>

<span data-ttu-id="29b34-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="29b34-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```

### <a name="response"></a><span data-ttu-id="29b34-179">响应</span><span class="sxs-lookup"><span data-stu-id="29b34-179">Response</span></span>

<span data-ttu-id="29b34-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="29b34-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

<span data-ttu-id="29b34-181">在这种情况下，将设置默认品牌对象。</span><span class="sxs-lookup"><span data-stu-id="29b34-181">In this case, the default branding object is set.</span></span> <span data-ttu-id="29b34-182">本地化品牌也会由于 Content-Language 标头而设置，即使该响应中未返回 `en-US`  `en-US` 品牌设置。</span><span class="sxs-lookup"><span data-stu-id="29b34-182">Localized branding for `en-US` is also set due to the **Content-Language** header, even though the `en-US` branding set is not returned in the response.</span></span> <span data-ttu-id="29b34-183">请求 **中的 Content-Language** 标头是可选的，如果不存在，则仅设置默认品牌。</span><span class="sxs-lookup"><span data-stu-id="29b34-183">The **Content-Language** header in the request is optional, and if not present, only sets the default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
