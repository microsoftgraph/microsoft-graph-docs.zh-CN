---
title: 创建本地化的 organizationalBrandingProperties
description: 为特定区域设置创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c293085887eb0e8c2d49c4e01c567dbeea32699
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524419"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="558b5-103">创建本地化的 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="558b5-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="558b5-104">为特定区域设置创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="558b5-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="558b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="558b5-105">Permissions</span></span>

<span data-ttu-id="558b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="558b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="558b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="558b5-108">Permission type</span></span>                        | <span data-ttu-id="558b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="558b5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="558b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="558b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="558b5-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="558b5-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="558b5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="558b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="558b5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="558b5-113">Not supported.</span></span> |
| <span data-ttu-id="558b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="558b5-114">Application</span></span>                            | <span data-ttu-id="558b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="558b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="558b5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="558b5-116">HTTP request</span></span>

<span data-ttu-id="558b5-117">发布到品牌/localizations 以创建新的本地化。</span><span class="sxs-lookup"><span data-stu-id="558b5-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="558b5-118">正文中指定的 id 是本地化的区域设置。</span><span class="sxs-lookup"><span data-stu-id="558b5-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="558b5-119">如果未指定 id，则内容语言标头的值（如果指定）将用作 id。如果没有指定 id，也未指定内容语言标头，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="558b5-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="558b5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="558b5-120">Optional query parameters</span></span>

<span data-ttu-id="558b5-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="558b5-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="558b5-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="558b5-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="558b5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="558b5-123">Request headers</span></span>

| <span data-ttu-id="558b5-124">名称</span><span class="sxs-lookup"><span data-stu-id="558b5-124">Name</span></span>      |<span data-ttu-id="558b5-125">说明</span><span class="sxs-lookup"><span data-stu-id="558b5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="558b5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="558b5-126">Authorization</span></span> | <span data-ttu-id="558b5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="558b5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="558b5-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="558b5-129">Content-Type</span></span>  | <span data-ttu-id="558b5-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="558b5-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="558b5-132">Content-Language</span><span class="sxs-lookup"><span data-stu-id="558b5-132">Content-Language</span></span>  | <span data-ttu-id="558b5-133">位置.</span><span class="sxs-lookup"><span data-stu-id="558b5-133">Locale.</span></span> <span data-ttu-id="558b5-134">可选。</span><span class="sxs-lookup"><span data-stu-id="558b5-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="558b5-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="558b5-135">Request body</span></span>

<span data-ttu-id="558b5-136">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="558b5-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="558b5-137">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="558b5-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="558b5-138">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="558b5-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="558b5-139">属性</span><span class="sxs-lookup"><span data-stu-id="558b5-139">Property</span></span>     | <span data-ttu-id="558b5-140">类型</span><span class="sxs-lookup"><span data-stu-id="558b5-140">Type</span></span>        | <span data-ttu-id="558b5-141">说明</span><span class="sxs-lookup"><span data-stu-id="558b5-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="558b5-142">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="558b5-142">backgroundColor</span></span>|<span data-ttu-id="558b5-143">String</span><span class="sxs-lookup"><span data-stu-id="558b5-143">String</span></span>|<span data-ttu-id="558b5-144">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="558b5-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="558b5-145">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="558b5-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="558b5-146">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="558b5-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="558b5-147">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="558b5-147">backgroundImage</span></span>|<span data-ttu-id="558b5-148">Stream</span><span class="sxs-lookup"><span data-stu-id="558b5-148">Stream</span></span>|<span data-ttu-id="558b5-149">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="558b5-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="558b5-150">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="558b5-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="558b5-151">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="558b5-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="558b5-152">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="558b5-152">bannerLogo</span></span>|<span data-ttu-id="558b5-153">Stream</span><span class="sxs-lookup"><span data-stu-id="558b5-153">Stream</span></span>|<span data-ttu-id="558b5-154">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="558b5-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="558b5-155">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="558b5-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="558b5-156">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="558b5-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="558b5-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="558b5-157">signInPageText</span></span>|<span data-ttu-id="558b5-158">String</span><span class="sxs-lookup"><span data-stu-id="558b5-158">String</span></span>|<span data-ttu-id="558b5-159">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="558b5-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="558b5-160">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="558b5-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="558b5-161">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="558b5-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="558b5-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="558b5-162">squareLogo</span></span>|<span data-ttu-id="558b5-163">Stream</span><span class="sxs-lookup"><span data-stu-id="558b5-163">Stream</span></span>|<span data-ttu-id="558b5-164">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="558b5-164">Square version of your company logo.</span></span> <span data-ttu-id="558b5-165">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="558b5-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="558b5-166">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="558b5-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="558b5-167">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="558b5-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="558b5-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="558b5-168">usernameHintText</span></span>|<span data-ttu-id="558b5-169">String</span><span class="sxs-lookup"><span data-stu-id="558b5-169">String</span></span>|<span data-ttu-id="558b5-170">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="558b5-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="558b5-171">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="558b5-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="558b5-172">id</span><span class="sxs-lookup"><span data-stu-id="558b5-172">id</span></span>|<span data-ttu-id="558b5-173">String</span><span class="sxs-lookup"><span data-stu-id="558b5-173">String</span></span>|<span data-ttu-id="558b5-174">创建品牌的区域设置</span><span class="sxs-lookup"><span data-stu-id="558b5-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="558b5-175">响应</span><span class="sxs-lookup"><span data-stu-id="558b5-175">Response</span></span>

<span data-ttu-id="558b5-176">如果成功，此方法 `201 CREATED` 在响应正文中返回响应代码和创建的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="558b5-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="558b5-177">示例</span><span class="sxs-lookup"><span data-stu-id="558b5-177">Examples</span></span>

<span data-ttu-id="558b5-178">下面的示例创建了法语 (fr) 的品牌打造本地化。</span><span class="sxs-lookup"><span data-stu-id="558b5-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="558b5-179">请求</span><span class="sxs-lookup"><span data-stu-id="558b5-179">Request</span></span>

<span data-ttu-id="558b5-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="558b5-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="558b5-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="558b5-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="558b5-182">C#</span><span class="sxs-lookup"><span data-stu-id="558b5-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="558b5-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="558b5-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="558b5-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="558b5-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="558b5-185">Java</span><span class="sxs-lookup"><span data-stu-id="558b5-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="558b5-186">响应</span><span class="sxs-lookup"><span data-stu-id="558b5-186">Response</span></span>

<span data-ttu-id="558b5-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="558b5-187">The following is an example of the response.</span></span>

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
<span data-ttu-id="558b5-188">**MediaEditLink** 指定本地化的媒体的写入位置。</span><span class="sxs-lookup"><span data-stu-id="558b5-188">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="558b5-189">MediaReadLink 为 null，因为没有为本地化设置媒体。</span><span class="sxs-lookup"><span data-stu-id="558b5-189">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
