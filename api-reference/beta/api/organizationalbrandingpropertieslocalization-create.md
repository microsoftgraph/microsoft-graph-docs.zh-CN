---
title: 创建本地化的 organizationalBrandingProperties
description: 为特定区域设置创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7e3108da9ed5251b9f041dc710c16bff674c8a01
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447816"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="46f3d-103">创建本地化的 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="46f3d-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46f3d-104">为特定区域设置创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46f3d-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="46f3d-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="46f3d-105">Permissions</span></span>

<span data-ttu-id="46f3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46f3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46f3d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="46f3d-108">Permission type</span></span>                        | <span data-ttu-id="46f3d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46f3d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46f3d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46f3d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="46f3d-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f3d-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="46f3d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46f3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46f3d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="46f3d-113">Not supported.</span></span> |
| <span data-ttu-id="46f3d-114">Application</span><span class="sxs-lookup"><span data-stu-id="46f3d-114">Application</span></span>                            | <span data-ttu-id="46f3d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46f3d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46f3d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46f3d-116">HTTP request</span></span>

<span data-ttu-id="46f3d-117">POST 到品牌打造/本地化以创建新的本地化。</span><span class="sxs-lookup"><span data-stu-id="46f3d-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="46f3d-118">正文中指定的 ID 是本地化区域设置。</span><span class="sxs-lookup"><span data-stu-id="46f3d-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="46f3d-119">如果未指定 id，则 Content-Language 标头的值（如果已指定）用作 ID。如果未指定 ID 和 Content-Language 标头，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="46f3d-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46f3d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46f3d-120">Optional query parameters</span></span>

<span data-ttu-id="46f3d-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46f3d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="46f3d-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="46f3d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46f3d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="46f3d-123">Request headers</span></span>

| <span data-ttu-id="46f3d-124">名称</span><span class="sxs-lookup"><span data-stu-id="46f3d-124">Name</span></span>      |<span data-ttu-id="46f3d-125">说明</span><span class="sxs-lookup"><span data-stu-id="46f3d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46f3d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="46f3d-126">Authorization</span></span> | <span data-ttu-id="46f3d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46f3d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46f3d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46f3d-129">Content-Type</span></span>  | <span data-ttu-id="46f3d-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="46f3d-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="46f3d-132">Content-Language</span><span class="sxs-lookup"><span data-stu-id="46f3d-132">Content-Language</span></span>  | <span data-ttu-id="46f3d-133">区域设置。</span><span class="sxs-lookup"><span data-stu-id="46f3d-133">Locale.</span></span> <span data-ttu-id="46f3d-134">可选。</span><span class="sxs-lookup"><span data-stu-id="46f3d-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46f3d-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="46f3d-135">Request body</span></span>

<span data-ttu-id="46f3d-136">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="46f3d-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="46f3d-137">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="46f3d-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="46f3d-138">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="46f3d-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46f3d-139">属性</span><span class="sxs-lookup"><span data-stu-id="46f3d-139">Property</span></span>     | <span data-ttu-id="46f3d-140">类型</span><span class="sxs-lookup"><span data-stu-id="46f3d-140">Type</span></span>        | <span data-ttu-id="46f3d-141">说明</span><span class="sxs-lookup"><span data-stu-id="46f3d-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46f3d-142">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="46f3d-142">backgroundColor</span></span>|<span data-ttu-id="46f3d-143">String</span><span class="sxs-lookup"><span data-stu-id="46f3d-143">String</span></span>|<span data-ttu-id="46f3d-144">将出现在低带宽连接中的背景图像的颜色。</span><span class="sxs-lookup"><span data-stu-id="46f3d-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="46f3d-145">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="46f3d-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="46f3d-146">以十六进制值指定 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="46f3d-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="46f3d-147">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="46f3d-147">backgroundImage</span></span>|<span data-ttu-id="46f3d-148">Stream</span><span class="sxs-lookup"><span data-stu-id="46f3d-148">Stream</span></span>|<span data-ttu-id="46f3d-149">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="46f3d-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="46f3d-150">.png 或 .jpg 不大于 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="46f3d-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="46f3d-151">较小的图像将降低带宽要求，使页面加载性能提高。</span><span class="sxs-lookup"><span data-stu-id="46f3d-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="46f3d-152">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="46f3d-152">bannerLogo</span></span>|<span data-ttu-id="46f3d-153">Stream</span><span class="sxs-lookup"><span data-stu-id="46f3d-153">Stream</span></span>|<span data-ttu-id="46f3d-154">显示在登录页面上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="46f3d-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="46f3d-155">.png 或 .jpg 不大于 36x245px。</span><span class="sxs-lookup"><span data-stu-id="46f3d-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="46f3d-156">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="46f3d-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="46f3d-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="46f3d-157">signInPageText</span></span>|<span data-ttu-id="46f3d-158">String</span><span class="sxs-lookup"><span data-stu-id="46f3d-158">String</span></span>|<span data-ttu-id="46f3d-159">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="46f3d-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="46f3d-160">可以使用此信息向技术支持或法律声明传达其他信息，例如电话号码。</span><span class="sxs-lookup"><span data-stu-id="46f3d-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="46f3d-161">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="46f3d-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="46f3d-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="46f3d-162">squareLogo</span></span>|<span data-ttu-id="46f3d-163">Stream</span><span class="sxs-lookup"><span data-stu-id="46f3d-163">Stream</span></span>|<span data-ttu-id="46f3d-164">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="46f3d-164">Square version of your company logo.</span></span> <span data-ttu-id="46f3d-165">这将显示在 Windows 10 现 (OOBE) 和启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="46f3d-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="46f3d-166">.png 或 .jpg 大小不超过 240x240px，大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="46f3d-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="46f3d-167">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="46f3d-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="46f3d-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="46f3d-168">usernameHintText</span></span>|<span data-ttu-id="46f3d-169">String</span><span class="sxs-lookup"><span data-stu-id="46f3d-169">String</span></span>|<span data-ttu-id="46f3d-170">在登录屏幕上的用户名文本框中作为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="46f3d-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="46f3d-171">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="46f3d-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="46f3d-172">id</span><span class="sxs-lookup"><span data-stu-id="46f3d-172">id</span></span>|<span data-ttu-id="46f3d-173">String</span><span class="sxs-lookup"><span data-stu-id="46f3d-173">String</span></span>|<span data-ttu-id="46f3d-174">创建品牌打造区域设置</span><span class="sxs-lookup"><span data-stu-id="46f3d-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="46f3d-175">响应</span><span class="sxs-lookup"><span data-stu-id="46f3d-175">Response</span></span>

<span data-ttu-id="46f3d-176">如果成功，此方法在响应正文中返回响应代码和已创建的 `201 CREATED` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46f3d-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46f3d-177">示例</span><span class="sxs-lookup"><span data-stu-id="46f3d-177">Examples</span></span>

<span data-ttu-id="46f3d-178">以下示例为法语版本创建一个品牌本地化 (fr) 。</span><span class="sxs-lookup"><span data-stu-id="46f3d-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="46f3d-179">请求</span><span class="sxs-lookup"><span data-stu-id="46f3d-179">Request</span></span>

<span data-ttu-id="46f3d-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="46f3d-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46f3d-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="46f3d-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="46f3d-182">C#</span><span class="sxs-lookup"><span data-stu-id="46f3d-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46f3d-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46f3d-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46f3d-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46f3d-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46f3d-185">Java</span><span class="sxs-lookup"><span data-stu-id="46f3d-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46f3d-186">响应</span><span class="sxs-lookup"><span data-stu-id="46f3d-186">Response</span></span>

<span data-ttu-id="46f3d-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="46f3d-187">The following is an example of the response.</span></span>

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
<span data-ttu-id="46f3d-188">**mediaEditLink** 指定本地化媒体的写入位置。</span><span class="sxs-lookup"><span data-stu-id="46f3d-188">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="46f3d-189">mediaReadLink 为 null，因为尚未为本地化设置媒体。</span><span class="sxs-lookup"><span data-stu-id="46f3d-189">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
