---
title: 更新本地化的 organizationalbrandingproperties
description: 为特定本地化更新 organizationalbrandingproperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 78e6ae581b1a4c0cbfd5fbff2f3814532c7491bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49523947"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="2c8ad-103">更新本地化的 organizationalbrandingproperties</span><span class="sxs-lookup"><span data-stu-id="2c8ad-103">Update Localized organizationalbrandingproperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c8ad-104">为特定本地化更新 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c8ad-105">权限</span><span class="sxs-lookup"><span data-stu-id="2c8ad-105">Permissions</span></span>

<span data-ttu-id="2c8ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c8ad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c8ad-108">Permission type</span></span>                        | <span data-ttu-id="2c8ad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c8ad-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c8ad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c8ad-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c8ad-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c8ad-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="2c8ad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c8ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c8ad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-113">Not supported.</span></span> |
| <span data-ttu-id="2c8ad-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c8ad-114">Application</span></span>                            | <span data-ttu-id="2c8ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c8ad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c8ad-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="2c8ad-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c8ad-117">Request headers</span></span>

| <span data-ttu-id="2c8ad-118">名称</span><span class="sxs-lookup"><span data-stu-id="2c8ad-118">Name</span></span>       | <span data-ttu-id="2c8ad-119">说明</span><span class="sxs-lookup"><span data-stu-id="2c8ad-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2c8ad-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c8ad-120">Authorization</span></span> | <span data-ttu-id="2c8ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c8ad-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c8ad-123">Content-Type</span></span>  | <span data-ttu-id="2c8ad-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="2c8ad-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="2c8ad-126">Content-Language</span></span>  | <span data-ttu-id="2c8ad-127">位置.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-127">Locale.</span></span> <span data-ttu-id="2c8ad-128">可选。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c8ad-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c8ad-129">Request body</span></span>

<span data-ttu-id="2c8ad-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2c8ad-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2c8ad-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2c8ad-133">属性</span><span class="sxs-lookup"><span data-stu-id="2c8ad-133">Property</span></span>     | <span data-ttu-id="2c8ad-134">类型</span><span class="sxs-lookup"><span data-stu-id="2c8ad-134">Type</span></span>        | <span data-ttu-id="2c8ad-135">说明</span><span class="sxs-lookup"><span data-stu-id="2c8ad-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c8ad-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="2c8ad-136">backgroundColor</span></span>|<span data-ttu-id="2c8ad-137">String</span><span class="sxs-lookup"><span data-stu-id="2c8ad-137">String</span></span>|<span data-ttu-id="2c8ad-138">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="2c8ad-139">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="2c8ad-140">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="2c8ad-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="2c8ad-141">backgroundImage</span></span>|<span data-ttu-id="2c8ad-142">Stream</span><span class="sxs-lookup"><span data-stu-id="2c8ad-142">Stream</span></span>|<span data-ttu-id="2c8ad-143">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="2c8ad-144">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="2c8ad-145">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="2c8ad-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="2c8ad-146">bannerLogo</span></span>|<span data-ttu-id="2c8ad-147">Stream</span><span class="sxs-lookup"><span data-stu-id="2c8ad-147">Stream</span></span>|<span data-ttu-id="2c8ad-148">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="2c8ad-149">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="2c8ad-150">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="2c8ad-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="2c8ad-151">signInPageText</span></span>|<span data-ttu-id="2c8ad-152">String</span><span class="sxs-lookup"><span data-stu-id="2c8ad-152">String</span></span>|<span data-ttu-id="2c8ad-153">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="2c8ad-154">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="2c8ad-155">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="2c8ad-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="2c8ad-156">squareLogo</span></span>|<span data-ttu-id="2c8ad-157">Stream</span><span class="sxs-lookup"><span data-stu-id="2c8ad-157">Stream</span></span>|<span data-ttu-id="2c8ad-158">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-158">Square version of your company logo.</span></span> <span data-ttu-id="2c8ad-159">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="2c8ad-160">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="2c8ad-161">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="2c8ad-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="2c8ad-162">usernameHintText</span></span>|<span data-ttu-id="2c8ad-163">String</span><span class="sxs-lookup"><span data-stu-id="2c8ad-163">String</span></span>|<span data-ttu-id="2c8ad-164">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="2c8ad-165">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="2c8ad-166">id</span><span class="sxs-lookup"><span data-stu-id="2c8ad-166">id</span></span>|<span data-ttu-id="2c8ad-167">String</span><span class="sxs-lookup"><span data-stu-id="2c8ad-167">String</span></span>|<span data-ttu-id="2c8ad-168">更新品牌的区域设置</span><span class="sxs-lookup"><span data-stu-id="2c8ad-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="2c8ad-169">响应</span><span class="sxs-lookup"><span data-stu-id="2c8ad-169">Response</span></span>

<span data-ttu-id="2c8ad-170">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2c8ad-171">示例</span><span class="sxs-lookup"><span data-stu-id="2c8ad-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="2c8ad-172">示例1：使用 PUT 设置用于 fr 本地化的 **bannerLogo**</span><span class="sxs-lookup"><span data-stu-id="2c8ad-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="2c8ad-173">以下请求更新了 fr 本地化的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-173">The following request updates the banner logo for the fr localization.</span></span> <span data-ttu-id="2c8ad-174">使用 PUT，如果不存在 fr 本地化，则返回 "找不到 404"。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-174">Using PUT, if the fr localization does not exist, "404 not found" is returned.</span></span> <span data-ttu-id="2c8ad-175">如果有效负载包含 id 属性或内容语言标头，并且它们与 URL 中的 id 不匹配，则返回一个错误的请求。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-175">If the payload contains an id property or Content-Language header, and they don't match id in URL, a Bad Request is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="2c8ad-176">请求</span><span class="sxs-lookup"><span data-stu-id="2c8ad-176">Request</span></span>

<span data-ttu-id="2c8ad-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c8ad-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8ad-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="2c8ad-179">C#</span><span class="sxs-lookup"><span data-stu-id="2c8ad-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c8ad-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c8ad-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c8ad-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c8ad-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c8ad-182">Java</span><span class="sxs-lookup"><span data-stu-id="2c8ad-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c8ad-183">响应</span><span class="sxs-lookup"><span data-stu-id="2c8ad-183">Response</span></span>

<span data-ttu-id="2c8ad-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="2c8ad-185">示例2：使用修补程序更新适用于 fr 本地化的 **bannerLogo**</span><span class="sxs-lookup"><span data-stu-id="2c8ad-185">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="2c8ad-186">以下请求更新了 fr 本地化的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-186">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="2c8ad-187">使用修补程序时，如果指定的本地化尚不存在，则会创建它并向其写入属性。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-187">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="2c8ad-188">请求</span><span class="sxs-lookup"><span data-stu-id="2c8ad-188">Request</span></span>

<span data-ttu-id="2c8ad-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c8ad-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8ad-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c8ad-191">C#</span><span class="sxs-lookup"><span data-stu-id="2c8ad-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c8ad-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c8ad-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c8ad-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c8ad-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c8ad-194">Java</span><span class="sxs-lookup"><span data-stu-id="2c8ad-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c8ad-195">响应</span><span class="sxs-lookup"><span data-stu-id="2c8ad-195">Response</span></span>
<span data-ttu-id="2c8ad-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="2c8ad-197">示例3：使用空字符串替代默认品牌值</span><span class="sxs-lookup"><span data-stu-id="2c8ad-197">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="2c8ad-198">如果本地化中的属性值为 null，则将从默认品牌打造继承值。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-198">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="2c8ad-199">若要避免这种情况发生，请在本地化的品牌中设置一个仅包含空格的空字符串或字符串。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-199">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="2c8ad-200">请求</span><span class="sxs-lookup"><span data-stu-id="2c8ad-200">Request</span></span>

<span data-ttu-id="2c8ad-201">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-201">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="2c8ad-202">响应</span><span class="sxs-lookup"><span data-stu-id="2c8ad-202">Response</span></span>

<span data-ttu-id="2c8ad-203">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-203">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="2c8ad-204">按照此请求，usernameHintText 的 fr 本地化将为空，而不是从默认品牌打造继承值。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-204">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="2c8ad-205">示例4：将法语本地化替换为 PUT</span><span class="sxs-lookup"><span data-stu-id="2c8ad-205">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="2c8ad-206">若要使用 PUT 对本地化进行更新，我们应在 body 中添加所有属性以及需要更新的属性，将现有对象替换为新对象。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-206">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="2c8ad-207">不在 PUT 的有效负载正文中的其他属性将设置为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-207">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="2c8ad-208">在下面的示例中，仅保留 backgroundColor 属性并更新 signInPageText，而将其他设置为 null。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-208">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="2c8ad-209">如果指定的本地化尚不存在，则放置到指定本地化创建该的 URL。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-209">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="2c8ad-210">如果有效负载包含 id 属性或内容语言标头，并且它们与 URL 中的 id 不匹配，则会引发错误的请求。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-210">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="2c8ad-211">请求</span><span class="sxs-lookup"><span data-stu-id="2c8ad-211">Request</span></span>

<span data-ttu-id="2c8ad-212">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c8ad-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8ad-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c8ad-214">C#</span><span class="sxs-lookup"><span data-stu-id="2c8ad-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c8ad-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c8ad-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c8ad-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c8ad-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c8ad-217">Java</span><span class="sxs-lookup"><span data-stu-id="2c8ad-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c8ad-218">响应</span><span class="sxs-lookup"><span data-stu-id="2c8ad-218">Response</span></span>
<span data-ttu-id="2c8ad-219">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c8ad-219">The following is an example of the response.</span></span>

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
