---
title: 创建本地化的 organizationalBrandingProperties
description: 为特定区域设置创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80849083686bab10626756197880ddfeade06c8b
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031908"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="c97c0-103">创建本地化的 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="c97c0-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c97c0-104">为特定区域设置创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c97c0-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="c97c0-105">权限</span><span class="sxs-lookup"><span data-stu-id="c97c0-105">Permissions</span></span>

<span data-ttu-id="c97c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c97c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c97c0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c97c0-108">Permission type</span></span>                        | <span data-ttu-id="c97c0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c97c0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c97c0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c97c0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c97c0-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c97c0-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="c97c0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c97c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c97c0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c97c0-113">Not supported.</span></span> |
| <span data-ttu-id="c97c0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c97c0-114">Application</span></span>                            | <span data-ttu-id="c97c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c97c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c97c0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c97c0-116">HTTP request</span></span>

<span data-ttu-id="c97c0-117">发布到品牌/localizations 以创建新的本地化。</span><span class="sxs-lookup"><span data-stu-id="c97c0-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="c97c0-118">正文中指定的 id 是本地化的区域设置。</span><span class="sxs-lookup"><span data-stu-id="c97c0-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="c97c0-119">如果未指定 id，则内容语言标头的值（如果指定）将用作 id。如果没有指定 id，也未指定内容语言标头，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="c97c0-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c97c0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c97c0-120">Optional query parameters</span></span>

<span data-ttu-id="c97c0-p103">此方法支持使用某些 OData 查询参数来帮助自定义响应。有关常规信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c97c0-p103">This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c97c0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c97c0-123">Request headers</span></span>

| <span data-ttu-id="c97c0-124">名称</span><span class="sxs-lookup"><span data-stu-id="c97c0-124">Name</span></span>      |<span data-ttu-id="c97c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="c97c0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c97c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c97c0-126">Authorization</span></span> | <span data-ttu-id="c97c0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c97c0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c97c0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c97c0-129">Content-Type</span></span>  | <span data-ttu-id="c97c0-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c97c0-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="c97c0-132">Content-Language</span><span class="sxs-lookup"><span data-stu-id="c97c0-132">Content-Language</span></span>  | <span data-ttu-id="c97c0-133">位置.</span><span class="sxs-lookup"><span data-stu-id="c97c0-133">Locale.</span></span> <span data-ttu-id="c97c0-134">可选。</span><span class="sxs-lookup"><span data-stu-id="c97c0-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c97c0-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="c97c0-135">Request body</span></span>

<span data-ttu-id="c97c0-136">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c97c0-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c97c0-137">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c97c0-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c97c0-138">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c97c0-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c97c0-139">属性</span><span class="sxs-lookup"><span data-stu-id="c97c0-139">Property</span></span>     | <span data-ttu-id="c97c0-140">类型</span><span class="sxs-lookup"><span data-stu-id="c97c0-140">Type</span></span>        | <span data-ttu-id="c97c0-141">Description</span><span class="sxs-lookup"><span data-stu-id="c97c0-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c97c0-142">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="c97c0-142">backgroundColor</span></span>|<span data-ttu-id="c97c0-143">String</span><span class="sxs-lookup"><span data-stu-id="c97c0-143">String</span></span>|<span data-ttu-id="c97c0-144">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="c97c0-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="c97c0-145">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="c97c0-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="c97c0-146">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="c97c0-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="c97c0-147">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="c97c0-147">backgroundImage</span></span>|<span data-ttu-id="c97c0-148">Stream</span><span class="sxs-lookup"><span data-stu-id="c97c0-148">Stream</span></span>|<span data-ttu-id="c97c0-149">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="c97c0-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="c97c0-150">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="c97c0-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="c97c0-151">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="c97c0-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="c97c0-152">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="c97c0-152">bannerLogo</span></span>|<span data-ttu-id="c97c0-153">Stream</span><span class="sxs-lookup"><span data-stu-id="c97c0-153">Stream</span></span>|<span data-ttu-id="c97c0-154">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="c97c0-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="c97c0-155">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="c97c0-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="c97c0-156">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="c97c0-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="c97c0-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="c97c0-157">signInPageText</span></span>|<span data-ttu-id="c97c0-158">String</span><span class="sxs-lookup"><span data-stu-id="c97c0-158">String</span></span>|<span data-ttu-id="c97c0-159">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="c97c0-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="c97c0-160">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="c97c0-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="c97c0-161">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="c97c0-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="c97c0-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="c97c0-162">squareLogo</span></span>|<span data-ttu-id="c97c0-163">Stream</span><span class="sxs-lookup"><span data-stu-id="c97c0-163">Stream</span></span>|<span data-ttu-id="c97c0-164">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="c97c0-164">Square version of your company logo.</span></span> <span data-ttu-id="c97c0-165">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="c97c0-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="c97c0-166">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="c97c0-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="c97c0-167">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="c97c0-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="c97c0-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="c97c0-168">usernameHintText</span></span>|<span data-ttu-id="c97c0-169">String</span><span class="sxs-lookup"><span data-stu-id="c97c0-169">String</span></span>|<span data-ttu-id="c97c0-170">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="c97c0-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="c97c0-171">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="c97c0-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="c97c0-172">id</span><span class="sxs-lookup"><span data-stu-id="c97c0-172">id</span></span>|<span data-ttu-id="c97c0-173">String</span><span class="sxs-lookup"><span data-stu-id="c97c0-173">String</span></span>|<span data-ttu-id="c97c0-174">创建品牌的区域设置</span><span class="sxs-lookup"><span data-stu-id="c97c0-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="c97c0-175">响应</span><span class="sxs-lookup"><span data-stu-id="c97c0-175">Response</span></span>

<span data-ttu-id="c97c0-176">如果成功，此方法 `201 CREATED` 在响应正文中返回响应代码和创建的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c97c0-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c97c0-177">示例</span><span class="sxs-lookup"><span data-stu-id="c97c0-177">Examples</span></span>

<span data-ttu-id="c97c0-178">下面的示例创建了法语 (fr) 的品牌打造本地化。</span><span class="sxs-lookup"><span data-stu-id="c97c0-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="c97c0-179">请求</span><span class="sxs-lookup"><span data-stu-id="c97c0-179">Request</span></span>

<span data-ttu-id="c97c0-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c97c0-180">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```

### <a name="response"></a><span data-ttu-id="c97c0-181">响应</span><span class="sxs-lookup"><span data-stu-id="c97c0-181">Response</span></span>

<span data-ttu-id="c97c0-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c97c0-182">The following is an example of the response.</span></span>

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
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
<span data-ttu-id="c97c0-183">**MediaEditLink** 指定本地化的媒体的写入位置。</span><span class="sxs-lookup"><span data-stu-id="c97c0-183">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="c97c0-184">MediaReadLink 为 null，因为没有为本地化设置媒体。</span><span class="sxs-lookup"><span data-stu-id="c97c0-184">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
