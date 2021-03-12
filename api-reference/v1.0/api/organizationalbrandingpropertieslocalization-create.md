---
title: 创建本地化的组织BrandingProperties
description: 为特定区域设置创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8a52e0861f27fc1a21a87d23704d5163456a53ea
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722535"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="9a684-103">创建本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="9a684-103">Create localized organizationalBrandingProperties</span></span>

<span data-ttu-id="9a684-104">为特定 [区域设置创建 organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a684-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a684-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="9a684-105">Permissions</span></span>

<span data-ttu-id="9a684-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a684-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a684-108">Permission type</span></span>                        | <span data-ttu-id="9a684-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a684-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a684-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a684-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a684-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a684-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="9a684-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a684-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a684-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a684-113">Not supported.</span></span> |
| <span data-ttu-id="9a684-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a684-114">Application</span></span>                            | <span data-ttu-id="9a684-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a684-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a684-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a684-116">HTTP request</span></span>

<span data-ttu-id="9a684-117">POST to branding/localizations to create a new localization.</span><span class="sxs-lookup"><span data-stu-id="9a684-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="9a684-118">正文中指定的 id 是本地化区域设置。</span><span class="sxs-lookup"><span data-stu-id="9a684-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="9a684-119">如果未指定 id，则 Content-Language 标头的值（如果已指定）将用作 id。如果未指定 id 和 Content-Language 标头，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="9a684-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="request-headers"></a><span data-ttu-id="9a684-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a684-120">Request headers</span></span>

| <span data-ttu-id="9a684-121">名称</span><span class="sxs-lookup"><span data-stu-id="9a684-121">Name</span></span>      |<span data-ttu-id="9a684-122">说明</span><span class="sxs-lookup"><span data-stu-id="9a684-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a684-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a684-123">Authorization</span></span> | <span data-ttu-id="9a684-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a684-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a684-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a684-126">Content-Type</span></span>  | <span data-ttu-id="9a684-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9a684-p104">application/json. Required.</span></span>  |
| <span data-ttu-id="9a684-129">Content-Language</span><span class="sxs-lookup"><span data-stu-id="9a684-129">Content-Language</span></span>  | <span data-ttu-id="9a684-130">区域设置。</span><span class="sxs-lookup"><span data-stu-id="9a684-130">Locale.</span></span> <span data-ttu-id="9a684-131">可选。</span><span class="sxs-lookup"><span data-stu-id="9a684-131">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a684-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a684-132">Request body</span></span>

<span data-ttu-id="9a684-133">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9a684-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9a684-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9a684-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9a684-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9a684-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a684-136">属性</span><span class="sxs-lookup"><span data-stu-id="9a684-136">Property</span></span>     | <span data-ttu-id="9a684-137">类型</span><span class="sxs-lookup"><span data-stu-id="9a684-137">Type</span></span>        | <span data-ttu-id="9a684-138">说明</span><span class="sxs-lookup"><span data-stu-id="9a684-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a684-139">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="9a684-139">backgroundColor</span></span>|<span data-ttu-id="9a684-140">字符串</span><span class="sxs-lookup"><span data-stu-id="9a684-140">String</span></span>|<span data-ttu-id="9a684-141">将出现在低带宽连接中的背景图像上的颜色。</span><span class="sxs-lookup"><span data-stu-id="9a684-141">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="9a684-142">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="9a684-142">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="9a684-143">以十六进制表示 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="9a684-143">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="9a684-144">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="9a684-144">backgroundImage</span></span>|<span data-ttu-id="9a684-145">Stream</span><span class="sxs-lookup"><span data-stu-id="9a684-145">Stream</span></span>|<span data-ttu-id="9a684-146">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="9a684-146">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="9a684-147">.png 或 .jpg 不大于 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="9a684-147">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="9a684-148">较小的图像将降低带宽要求，提高页面加载性能。</span><span class="sxs-lookup"><span data-stu-id="9a684-148">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="9a684-149">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="9a684-149">bannerLogo</span></span>|<span data-ttu-id="9a684-150">Stream</span><span class="sxs-lookup"><span data-stu-id="9a684-150">Stream</span></span>|<span data-ttu-id="9a684-151">显示在登录页上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="9a684-151">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="9a684-152">.png 或 .jpg 不超过 36x245px。</span><span class="sxs-lookup"><span data-stu-id="9a684-152">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="9a684-153">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="9a684-153">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="9a684-154">signInPageText</span><span class="sxs-lookup"><span data-stu-id="9a684-154">signInPageText</span></span>|<span data-ttu-id="9a684-155">字符串</span><span class="sxs-lookup"><span data-stu-id="9a684-155">String</span></span>|<span data-ttu-id="9a684-156">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="9a684-156">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="9a684-157">您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="9a684-157">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="9a684-158">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="9a684-158">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="9a684-159">squareLogo</span><span class="sxs-lookup"><span data-stu-id="9a684-159">squareLogo</span></span>|<span data-ttu-id="9a684-160">Stream</span><span class="sxs-lookup"><span data-stu-id="9a684-160">Stream</span></span>|<span data-ttu-id="9a684-161">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="9a684-161">Square version of your company logo.</span></span> <span data-ttu-id="9a684-162">这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="9a684-162">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="9a684-163">.png 或 .jpg 不超过 240x240px 且大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="9a684-163">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="9a684-164">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="9a684-164">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="9a684-165">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="9a684-165">usernameHintText</span></span>|<span data-ttu-id="9a684-166">字符串</span><span class="sxs-lookup"><span data-stu-id="9a684-166">String</span></span>|<span data-ttu-id="9a684-167">字符串，在登录屏幕的用户名文本框中作为提示显示。</span><span class="sxs-lookup"><span data-stu-id="9a684-167">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="9a684-168">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="9a684-168">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="9a684-169">id</span><span class="sxs-lookup"><span data-stu-id="9a684-169">id</span></span>|<span data-ttu-id="9a684-170">字符串</span><span class="sxs-lookup"><span data-stu-id="9a684-170">String</span></span>|<span data-ttu-id="9a684-171">要创建品牌打造区域设置</span><span class="sxs-lookup"><span data-stu-id="9a684-171">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="9a684-172">响应</span><span class="sxs-lookup"><span data-stu-id="9a684-172">Response</span></span>

<span data-ttu-id="9a684-173">如果成功，此方法在响应正文中返回 响应代码和创建的 `201 Created` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a684-173">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a684-174">示例</span><span class="sxs-lookup"><span data-stu-id="9a684-174">Examples</span></span>

<span data-ttu-id="9a684-175">以下示例为法语版本创建品牌本地化 (fr) 。</span><span class="sxs-lookup"><span data-stu-id="9a684-175">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="9a684-176">请求</span><span class="sxs-lookup"><span data-stu-id="9a684-176">Request</span></span>

<span data-ttu-id="9a684-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a684-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```

### <a name="response"></a><span data-ttu-id="9a684-178">响应</span><span class="sxs-lookup"><span data-stu-id="9a684-178">Response</span></span>

<span data-ttu-id="9a684-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a684-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
<span data-ttu-id="9a684-180">**mediaEditLink** 指定本地化媒体的写入位置。</span><span class="sxs-lookup"><span data-stu-id="9a684-180">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="9a684-181">mediaReadLink 为 null，因为尚未为本地化设置媒体。</span><span class="sxs-lookup"><span data-stu-id="9a684-181">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
