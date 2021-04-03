---
title: 创建本地化的组织BrandingProperties
description: 为特定区域设置创建组织品牌。
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3d49f5fe2589acf2d668a25240a5862197390b87
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582709"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="be6ca-103">创建本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="be6ca-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be6ca-104">为特定 [区域设置创建 organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be6ca-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="be6ca-105">权限</span><span class="sxs-lookup"><span data-stu-id="be6ca-105">Permissions</span></span>

<span data-ttu-id="be6ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be6ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be6ca-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="be6ca-108">Permission type</span></span>                        | <span data-ttu-id="be6ca-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be6ca-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be6ca-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be6ca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="be6ca-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be6ca-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="be6ca-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be6ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be6ca-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="be6ca-113">Not supported.</span></span> |
| <span data-ttu-id="be6ca-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="be6ca-114">Application</span></span>                            | <span data-ttu-id="be6ca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be6ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be6ca-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be6ca-116">HTTP request</span></span>

<span data-ttu-id="be6ca-117">POST to branding/localizations to create a new localization.</span><span class="sxs-lookup"><span data-stu-id="be6ca-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="be6ca-118">正文中指定的 id 是本地化区域设置。</span><span class="sxs-lookup"><span data-stu-id="be6ca-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="be6ca-119">如果未指定 id，则 Content-Language 标头的值（如果已指定）将用作 id。如果未指定 id 和 Content-Language 标头，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="be6ca-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be6ca-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be6ca-120">Optional query parameters</span></span>

<span data-ttu-id="be6ca-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be6ca-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be6ca-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="be6ca-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="be6ca-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="be6ca-123">Request headers</span></span>

| <span data-ttu-id="be6ca-124">名称</span><span class="sxs-lookup"><span data-stu-id="be6ca-124">Name</span></span>      |<span data-ttu-id="be6ca-125">说明</span><span class="sxs-lookup"><span data-stu-id="be6ca-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be6ca-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="be6ca-126">Authorization</span></span> | <span data-ttu-id="be6ca-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be6ca-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be6ca-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be6ca-129">Content-Type</span></span>  | <span data-ttu-id="be6ca-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="be6ca-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="be6ca-132">Content-Language</span><span class="sxs-lookup"><span data-stu-id="be6ca-132">Content-Language</span></span>  | <span data-ttu-id="be6ca-133">区域设置。</span><span class="sxs-lookup"><span data-stu-id="be6ca-133">Locale.</span></span> <span data-ttu-id="be6ca-134">可选。</span><span class="sxs-lookup"><span data-stu-id="be6ca-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be6ca-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="be6ca-135">Request body</span></span>

<span data-ttu-id="be6ca-136">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="be6ca-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="be6ca-137">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="be6ca-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="be6ca-138">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="be6ca-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="be6ca-139">属性</span><span class="sxs-lookup"><span data-stu-id="be6ca-139">Property</span></span>     | <span data-ttu-id="be6ca-140">类型</span><span class="sxs-lookup"><span data-stu-id="be6ca-140">Type</span></span>        | <span data-ttu-id="be6ca-141">说明</span><span class="sxs-lookup"><span data-stu-id="be6ca-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="be6ca-142">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="be6ca-142">backgroundColor</span></span>|<span data-ttu-id="be6ca-143">字符串</span><span class="sxs-lookup"><span data-stu-id="be6ca-143">String</span></span>|<span data-ttu-id="be6ca-144">将出现在低带宽连接中的背景图像上的颜色。</span><span class="sxs-lookup"><span data-stu-id="be6ca-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="be6ca-145">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="be6ca-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="be6ca-146">以十六进制表示 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="be6ca-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="be6ca-147">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="be6ca-147">backgroundImage</span></span>|<span data-ttu-id="be6ca-148">Stream</span><span class="sxs-lookup"><span data-stu-id="be6ca-148">Stream</span></span>|<span data-ttu-id="be6ca-149">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="be6ca-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="be6ca-150">.png 或 .jpg 不大于 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="be6ca-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="be6ca-151">较小的图像将降低带宽要求，提高页面加载性能。</span><span class="sxs-lookup"><span data-stu-id="be6ca-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="be6ca-152">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="be6ca-152">bannerLogo</span></span>|<span data-ttu-id="be6ca-153">Stream</span><span class="sxs-lookup"><span data-stu-id="be6ca-153">Stream</span></span>|<span data-ttu-id="be6ca-154">显示在登录页上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="be6ca-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="be6ca-155">.png 或 .jpg 不超过 36x245px。</span><span class="sxs-lookup"><span data-stu-id="be6ca-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="be6ca-156">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="be6ca-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="be6ca-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="be6ca-157">signInPageText</span></span>|<span data-ttu-id="be6ca-158">字符串</span><span class="sxs-lookup"><span data-stu-id="be6ca-158">String</span></span>|<span data-ttu-id="be6ca-159">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="be6ca-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="be6ca-160">您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="be6ca-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="be6ca-161">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="be6ca-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="be6ca-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="be6ca-162">squareLogo</span></span>|<span data-ttu-id="be6ca-163">Stream</span><span class="sxs-lookup"><span data-stu-id="be6ca-163">Stream</span></span>|<span data-ttu-id="be6ca-164">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="be6ca-164">Square version of your company logo.</span></span> <span data-ttu-id="be6ca-165">这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="be6ca-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="be6ca-166">.png 或 .jpg 不超过 240x240px 且大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="be6ca-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="be6ca-167">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="be6ca-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="be6ca-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="be6ca-168">usernameHintText</span></span>|<span data-ttu-id="be6ca-169">字符串</span><span class="sxs-lookup"><span data-stu-id="be6ca-169">String</span></span>|<span data-ttu-id="be6ca-170">字符串，在登录屏幕的用户名文本框中作为提示显示。</span><span class="sxs-lookup"><span data-stu-id="be6ca-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="be6ca-171">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="be6ca-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="be6ca-172">id</span><span class="sxs-lookup"><span data-stu-id="be6ca-172">id</span></span>|<span data-ttu-id="be6ca-173">字符串</span><span class="sxs-lookup"><span data-stu-id="be6ca-173">String</span></span>|<span data-ttu-id="be6ca-174">要创建品牌打造区域设置</span><span class="sxs-lookup"><span data-stu-id="be6ca-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="be6ca-175">响应</span><span class="sxs-lookup"><span data-stu-id="be6ca-175">Response</span></span>

<span data-ttu-id="be6ca-176">如果成功，此方法在响应正文中返回 响应代码和创建的 `201 CREATED` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be6ca-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be6ca-177">示例</span><span class="sxs-lookup"><span data-stu-id="be6ca-177">Examples</span></span>

<span data-ttu-id="be6ca-178">以下示例为法语版本创建品牌本地化 (fr) 。</span><span class="sxs-lookup"><span data-stu-id="be6ca-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="be6ca-179">请求</span><span class="sxs-lookup"><span data-stu-id="be6ca-179">Request</span></span>

<span data-ttu-id="be6ca-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be6ca-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be6ca-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="be6ca-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_7"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="be6ca-182">C#</span><span class="sxs-lookup"><span data-stu-id="be6ca-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be6ca-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be6ca-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be6ca-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be6ca-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be6ca-185">Java</span><span class="sxs-lookup"><span data-stu-id="be6ca-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be6ca-186">响应</span><span class="sxs-lookup"><span data-stu-id="be6ca-186">Response</span></span>

<span data-ttu-id="be6ca-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be6ca-187">The following is an example of the response.</span></span>

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
<span data-ttu-id="be6ca-188">**mediaEditLink** 指定本地化媒体的写入位置。</span><span class="sxs-lookup"><span data-stu-id="be6ca-188">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="be6ca-189">mediaReadLink 为 null，因为尚未为本地化设置媒体。</span><span class="sxs-lookup"><span data-stu-id="be6ca-189">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
