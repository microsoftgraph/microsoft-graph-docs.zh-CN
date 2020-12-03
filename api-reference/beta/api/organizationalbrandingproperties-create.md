---
title: 创建 organizationalBrandingProperties
description: 创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adf9a1e6b3f0bb01cbe028b27822b139d736d42e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524615"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="27d03-103">创建 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="27d03-103">Create organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d03-104">创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27d03-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="27d03-105">这将同时创建默认品牌打造和本地化品牌（可选）。</span><span class="sxs-lookup"><span data-stu-id="27d03-105">This creates the default branding and optionally a localized branding at the same time.</span></span> <span data-ttu-id="27d03-106">当本地化品牌集未配置为使用用户的浏览器语言时，将加载默认品牌。</span><span class="sxs-lookup"><span data-stu-id="27d03-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="27d03-107">权限</span><span class="sxs-lookup"><span data-stu-id="27d03-107">Permissions</span></span>

<span data-ttu-id="27d03-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27d03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27d03-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27d03-110">Permission type</span></span>                        | <span data-ttu-id="27d03-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27d03-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27d03-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27d03-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="27d03-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d03-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="27d03-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27d03-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27d03-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27d03-115">Not supported.</span></span> |
| <span data-ttu-id="27d03-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="27d03-116">Application</span></span>                            | <span data-ttu-id="27d03-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="27d03-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27d03-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27d03-118">HTTP request</span></span>

<span data-ttu-id="27d03-119">如果尚不存在使用 PUT 或 PATCH 的组织，则会为组织创建一个品牌。</span><span class="sxs-lookup"><span data-stu-id="27d03-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="27d03-120">如果已配置品牌，则 PUT 将覆盖所有现有值，而不管请求正文中的内容如何。</span><span class="sxs-lookup"><span data-stu-id="27d03-120">If branding is already configured, PUT will overwrite all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="27d03-121">修补程序将仅 overite 请求正文中包含的值，并将不包含的值保持不变。</span><span class="sxs-lookup"><span data-stu-id="27d03-121">PATCH will only overite the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="27d03-122">对/branding singleton 的 PUT/PATCH 忽略 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="27d03-122">The **id** property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="27d03-123">如果未指定内容语言，则会创建默认品牌，它对应于的 **id** `und` 。</span><span class="sxs-lookup"><span data-stu-id="27d03-123">If Content-Language is not specified, the default branding is created, which corresponds to an **id** of `und`.</span></span> <span data-ttu-id="27d03-124">如果指定了 Content 语言，则会为该区域设置创建品牌。</span><span class="sxs-lookup"><span data-stu-id="27d03-124">If Content-Language is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27d03-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="27d03-125">Optional query parameters</span></span>

<span data-ttu-id="27d03-126">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="27d03-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="27d03-127">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="27d03-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="27d03-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="27d03-128">Request headers</span></span>

| <span data-ttu-id="27d03-129">名称</span><span class="sxs-lookup"><span data-stu-id="27d03-129">Name</span></span>      |<span data-ttu-id="27d03-130">说明</span><span class="sxs-lookup"><span data-stu-id="27d03-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27d03-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="27d03-131">Authorization</span></span> | <span data-ttu-id="27d03-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27d03-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27d03-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27d03-134">Content-Type</span></span>  | <span data-ttu-id="27d03-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="27d03-p107">application/json. Required.</span></span>  |
| <span data-ttu-id="27d03-137">Content-Language</span><span class="sxs-lookup"><span data-stu-id="27d03-137">Content-Language</span></span>  | <span data-ttu-id="27d03-138">位置.</span><span class="sxs-lookup"><span data-stu-id="27d03-138">Locale.</span></span> <span data-ttu-id="27d03-139">可选。</span><span class="sxs-lookup"><span data-stu-id="27d03-139">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27d03-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="27d03-140">Request body</span></span>

| <span data-ttu-id="27d03-141">属性</span><span class="sxs-lookup"><span data-stu-id="27d03-141">Property</span></span>     | <span data-ttu-id="27d03-142">类型</span><span class="sxs-lookup"><span data-stu-id="27d03-142">Type</span></span>        | <span data-ttu-id="27d03-143">说明</span><span class="sxs-lookup"><span data-stu-id="27d03-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27d03-144">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="27d03-144">backgroundColor</span></span>|<span data-ttu-id="27d03-145">String</span><span class="sxs-lookup"><span data-stu-id="27d03-145">String</span></span>|<span data-ttu-id="27d03-146">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="27d03-146">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="27d03-147">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="27d03-147">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="27d03-148">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="27d03-148">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="27d03-149">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="27d03-149">backgroundImage</span></span>|<span data-ttu-id="27d03-150">Stream</span><span class="sxs-lookup"><span data-stu-id="27d03-150">Stream</span></span>|<span data-ttu-id="27d03-151">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="27d03-151">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="27d03-152">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="27d03-152">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="27d03-153">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="27d03-153">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="27d03-154">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="27d03-154">bannerLogo</span></span>|<span data-ttu-id="27d03-155">Stream</span><span class="sxs-lookup"><span data-stu-id="27d03-155">Stream</span></span>|<span data-ttu-id="27d03-156">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="27d03-156">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="27d03-157">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="27d03-157">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="27d03-158">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="27d03-158">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="27d03-159">signInPageText</span><span class="sxs-lookup"><span data-stu-id="27d03-159">signInPageText</span></span>|<span data-ttu-id="27d03-160">String</span><span class="sxs-lookup"><span data-stu-id="27d03-160">String</span></span>|<span data-ttu-id="27d03-161">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="27d03-161">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="27d03-162">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="27d03-162">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="27d03-163">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="27d03-163">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="27d03-164">squareLogo</span><span class="sxs-lookup"><span data-stu-id="27d03-164">squareLogo</span></span>|<span data-ttu-id="27d03-165">Stream</span><span class="sxs-lookup"><span data-stu-id="27d03-165">Stream</span></span>|<span data-ttu-id="27d03-166">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="27d03-166">Square version of your company logo.</span></span> <span data-ttu-id="27d03-167">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="27d03-167">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="27d03-168">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="27d03-168">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="27d03-169">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="27d03-169">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="27d03-170">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="27d03-170">usernameHintText</span></span>|<span data-ttu-id="27d03-171">String</span><span class="sxs-lookup"><span data-stu-id="27d03-171">String</span></span>|<span data-ttu-id="27d03-172">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="27d03-172">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="27d03-173">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="27d03-173">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="27d03-174">响应</span><span class="sxs-lookup"><span data-stu-id="27d03-174">Response</span></span>

<span data-ttu-id="27d03-175">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和创建的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27d03-175">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27d03-176">示例</span><span class="sxs-lookup"><span data-stu-id="27d03-176">Examples</span></span>

<span data-ttu-id="27d03-177">下面的示例为 en-us 创建了默认的品牌打造和本地化。</span><span class="sxs-lookup"><span data-stu-id="27d03-177">The following example creates default branding and localization for en-US.</span></span>

### <a name="request"></a><span data-ttu-id="27d03-178">请求</span><span class="sxs-lookup"><span data-stu-id="27d03-178">Request</span></span>

<span data-ttu-id="27d03-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="27d03-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27d03-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d03-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```
# <a name="c"></a>[<span data-ttu-id="27d03-181">C#</span><span class="sxs-lookup"><span data-stu-id="27d03-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27d03-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d03-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27d03-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27d03-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27d03-184">Java</span><span class="sxs-lookup"><span data-stu-id="27d03-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27d03-185">响应</span><span class="sxs-lookup"><span data-stu-id="27d03-185">Response</span></span>

<span data-ttu-id="27d03-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="27d03-186">The following is an example of the response.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

<span data-ttu-id="27d03-187">在这种情况下，将设置默认品牌化对象。</span><span class="sxs-lookup"><span data-stu-id="27d03-187">In this case, the default branding object is set.</span></span> <span data-ttu-id="27d03-188">由于标头中的内容语言，即使在响应中未返回 en-us 品牌设置，也会对 en-us 的本地化品牌进行设置。</span><span class="sxs-lookup"><span data-stu-id="27d03-188">Localized branding for en-US is also set due to the Content-Language in the header, even though the en-US branding set is not returned in the response.</span></span> <span data-ttu-id="27d03-189">请注意，请求中的内容语言是可选的，如果不存在，将仅设置默认品牌。</span><span class="sxs-lookup"><span data-stu-id="27d03-189">Note that Content-Language in the request is optional, and if not present, will only set default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
