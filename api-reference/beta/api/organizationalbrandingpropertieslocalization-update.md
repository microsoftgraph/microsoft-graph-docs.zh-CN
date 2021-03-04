---
title: 更新本地化的 organizationalbrandingproperties
description: 为特定本地化更新 organizationalbrandingproperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 42f55715cdb43abec4da9142953c6ccb74722bd2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434032"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="024c9-103">更新本地化的 organizationalbrandingproperties</span><span class="sxs-lookup"><span data-stu-id="024c9-103">Update Localized organizationalbrandingproperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="024c9-104">为特定本地化更新 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="024c9-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="024c9-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="024c9-105">Permissions</span></span>

<span data-ttu-id="024c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="024c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="024c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="024c9-108">Permission type</span></span>                        | <span data-ttu-id="024c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="024c9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="024c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="024c9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="024c9-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="024c9-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="024c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="024c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="024c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="024c9-113">Not supported.</span></span> |
| <span data-ttu-id="024c9-114">Application</span><span class="sxs-lookup"><span data-stu-id="024c9-114">Application</span></span>                            | <span data-ttu-id="024c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="024c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="024c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="024c9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}
PUT /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="024c9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="024c9-117">Request headers</span></span>

| <span data-ttu-id="024c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="024c9-118">Name</span></span>       | <span data-ttu-id="024c9-119">说明</span><span class="sxs-lookup"><span data-stu-id="024c9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="024c9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="024c9-120">Authorization</span></span> | <span data-ttu-id="024c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="024c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="024c9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="024c9-123">Content-Type</span></span>  | <span data-ttu-id="024c9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="024c9-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="024c9-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="024c9-126">Content-Language</span></span>  | <span data-ttu-id="024c9-127">区域设置。</span><span class="sxs-lookup"><span data-stu-id="024c9-127">Locale.</span></span> <span data-ttu-id="024c9-128">可选。</span><span class="sxs-lookup"><span data-stu-id="024c9-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="024c9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="024c9-129">Request body</span></span>

<span data-ttu-id="024c9-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="024c9-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="024c9-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="024c9-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="024c9-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="024c9-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="024c9-133">属性</span><span class="sxs-lookup"><span data-stu-id="024c9-133">Property</span></span>     | <span data-ttu-id="024c9-134">类型</span><span class="sxs-lookup"><span data-stu-id="024c9-134">Type</span></span>        | <span data-ttu-id="024c9-135">说明</span><span class="sxs-lookup"><span data-stu-id="024c9-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="024c9-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="024c9-136">backgroundColor</span></span>|<span data-ttu-id="024c9-137">String</span><span class="sxs-lookup"><span data-stu-id="024c9-137">String</span></span>|<span data-ttu-id="024c9-138">将出现在低带宽连接中的背景图像的颜色。</span><span class="sxs-lookup"><span data-stu-id="024c9-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="024c9-139">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="024c9-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="024c9-140">以十六进制值指定 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="024c9-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="024c9-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="024c9-141">backgroundImage</span></span>|<span data-ttu-id="024c9-142">Stream</span><span class="sxs-lookup"><span data-stu-id="024c9-142">Stream</span></span>|<span data-ttu-id="024c9-143">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="024c9-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="024c9-144">.png 或 .jpg 不大于 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="024c9-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="024c9-145">较小的图像将降低带宽要求，使页面加载性能提高。</span><span class="sxs-lookup"><span data-stu-id="024c9-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="024c9-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="024c9-146">bannerLogo</span></span>|<span data-ttu-id="024c9-147">Stream</span><span class="sxs-lookup"><span data-stu-id="024c9-147">Stream</span></span>|<span data-ttu-id="024c9-148">显示在登录页面上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="024c9-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="024c9-149">.png 或 .jpg 不大于 36x245px。</span><span class="sxs-lookup"><span data-stu-id="024c9-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="024c9-150">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="024c9-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="024c9-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="024c9-151">signInPageText</span></span>|<span data-ttu-id="024c9-152">String</span><span class="sxs-lookup"><span data-stu-id="024c9-152">String</span></span>|<span data-ttu-id="024c9-153">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="024c9-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="024c9-154">可以使用此信息将其他信息（如电话号码）传达给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="024c9-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="024c9-155">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="024c9-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="024c9-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="024c9-156">squareLogo</span></span>|<span data-ttu-id="024c9-157">Stream</span><span class="sxs-lookup"><span data-stu-id="024c9-157">Stream</span></span>|<span data-ttu-id="024c9-158">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="024c9-158">Square version of your company logo.</span></span> <span data-ttu-id="024c9-159">这将显示在 Windows 10 现 (OOBE) 和启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="024c9-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="024c9-160">.png 或 .jpg 大小不超过 240x240px，大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="024c9-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="024c9-161">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="024c9-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="024c9-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="024c9-162">usernameHintText</span></span>|<span data-ttu-id="024c9-163">String</span><span class="sxs-lookup"><span data-stu-id="024c9-163">String</span></span>|<span data-ttu-id="024c9-164">在登录屏幕上的用户名文本框中作为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="024c9-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="024c9-165">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="024c9-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="024c9-166">id</span><span class="sxs-lookup"><span data-stu-id="024c9-166">id</span></span>|<span data-ttu-id="024c9-167">String</span><span class="sxs-lookup"><span data-stu-id="024c9-167">String</span></span>|<span data-ttu-id="024c9-168">要更新其品牌设置区域设置</span><span class="sxs-lookup"><span data-stu-id="024c9-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="024c9-169">响应</span><span class="sxs-lookup"><span data-stu-id="024c9-169">Response</span></span>

<span data-ttu-id="024c9-170">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="024c9-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="024c9-171">示例</span><span class="sxs-lookup"><span data-stu-id="024c9-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="024c9-172">示例 1：使用 PUT 设置 fr 本地化的 **bannerLogo**</span><span class="sxs-lookup"><span data-stu-id="024c9-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="024c9-173">以下请求更新 fr 本地化的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="024c9-173">The following request updates the banner logo for the fr localization.</span></span> <span data-ttu-id="024c9-174">使用 PUT 时，如果 fr 本地化不存在，则返回"未找到 404"。</span><span class="sxs-lookup"><span data-stu-id="024c9-174">Using PUT, if the fr localization does not exist, "404 not found" is returned.</span></span> <span data-ttu-id="024c9-175">如果有效负载包含 id 属性或 Content-Language 标头，并且它们与 URL 中的 ID 不匹配，则返回错误请求。</span><span class="sxs-lookup"><span data-stu-id="024c9-175">If the payload contains an id property or Content-Language header, and they don't match id in URL, a Bad Request is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="024c9-176">请求</span><span class="sxs-lookup"><span data-stu-id="024c9-176">Request</span></span>

<span data-ttu-id="024c9-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="024c9-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="024c9-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="024c9-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="024c9-179">C#</span><span class="sxs-lookup"><span data-stu-id="024c9-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="024c9-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="024c9-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="024c9-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="024c9-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="024c9-182">Java</span><span class="sxs-lookup"><span data-stu-id="024c9-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="024c9-183">响应</span><span class="sxs-lookup"><span data-stu-id="024c9-183">Response</span></span>

<span data-ttu-id="024c9-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="024c9-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="024c9-185">示例 2：使用 PATCH 更新 fr 本地化的 **bannerLogo**</span><span class="sxs-lookup"><span data-stu-id="024c9-185">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="024c9-186">以下请求更新 fr 本地化的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="024c9-186">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="024c9-187">使用 PATCH，如果指定的本地化不存在，则创建它，并写入属性。</span><span class="sxs-lookup"><span data-stu-id="024c9-187">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="024c9-188">请求</span><span class="sxs-lookup"><span data-stu-id="024c9-188">Request</span></span>

<span data-ttu-id="024c9-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="024c9-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="024c9-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="024c9-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="024c9-191">C#</span><span class="sxs-lookup"><span data-stu-id="024c9-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="024c9-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="024c9-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="024c9-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="024c9-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="024c9-194">Java</span><span class="sxs-lookup"><span data-stu-id="024c9-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="024c9-195">响应</span><span class="sxs-lookup"><span data-stu-id="024c9-195">Response</span></span>
<span data-ttu-id="024c9-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="024c9-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="024c9-197">示例 3：使用空字符串替代默认品牌值</span><span class="sxs-lookup"><span data-stu-id="024c9-197">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="024c9-198">如果本地化中的属性值为 null，则该值将继承自默认品牌。</span><span class="sxs-lookup"><span data-stu-id="024c9-198">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="024c9-199">若要防止这种情况发生，请设置一个空字符串或字符串，其中仅包含本地化品牌中的空白。</span><span class="sxs-lookup"><span data-stu-id="024c9-199">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="024c9-200">请求</span><span class="sxs-lookup"><span data-stu-id="024c9-200">Request</span></span>

<span data-ttu-id="024c9-201">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="024c9-201">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="024c9-202">响应</span><span class="sxs-lookup"><span data-stu-id="024c9-202">Response</span></span>

<span data-ttu-id="024c9-203">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="024c9-203">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="024c9-204">在此请求后，fr 本地化的 usernameHintText 将为空，而不是从默认品牌继承值。</span><span class="sxs-lookup"><span data-stu-id="024c9-204">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="024c9-205">示例 4：将法语本地化替换为 PUT</span><span class="sxs-lookup"><span data-stu-id="024c9-205">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="024c9-206">若要使用 PUT 更新本地化，应在正文中添加所有属性以及需要更新的属性，因为 PUT 将现有对象替换为新对象。</span><span class="sxs-lookup"><span data-stu-id="024c9-206">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="024c9-207">其他不在 PUT 的有效负载正文中的属性将设置为 NULL。</span><span class="sxs-lookup"><span data-stu-id="024c9-207">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="024c9-208">下面的示例中，仅保留 backgroundColor 属性，并更新 signInPageText，而其他属性设置为 null。</span><span class="sxs-lookup"><span data-stu-id="024c9-208">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="024c9-209">如果指定的本地化不存在，PUT to the URL 指定本地化将创建它。</span><span class="sxs-lookup"><span data-stu-id="024c9-209">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="024c9-210">如果有效负载包含 id 属性或 Content-Language 标头，并且它们与 URL 中的 ID 不匹配，我们将引发错误请求。</span><span class="sxs-lookup"><span data-stu-id="024c9-210">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="024c9-211">请求</span><span class="sxs-lookup"><span data-stu-id="024c9-211">Request</span></span>

<span data-ttu-id="024c9-212">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="024c9-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="024c9-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="024c9-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="024c9-214">C#</span><span class="sxs-lookup"><span data-stu-id="024c9-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="024c9-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="024c9-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="024c9-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="024c9-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="024c9-217">Java</span><span class="sxs-lookup"><span data-stu-id="024c9-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="024c9-218">响应</span><span class="sxs-lookup"><span data-stu-id="024c9-218">Response</span></span>
<span data-ttu-id="024c9-219">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="024c9-219">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
