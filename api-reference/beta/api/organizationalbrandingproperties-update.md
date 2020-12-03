---
title: 更新 organizationalBrandingProperties
description: 更新 organizationalBrandingProperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd8eb2976fc3e8309f804714babbd45474574455
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524461"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="c11bf-103">更新 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="c11bf-103">Update organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c11bf-104">更新 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c11bf-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c11bf-105">权限</span><span class="sxs-lookup"><span data-stu-id="c11bf-105">Permissions</span></span>

<span data-ttu-id="c11bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c11bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c11bf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c11bf-108">Permission type</span></span>                        | <span data-ttu-id="c11bf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c11bf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c11bf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c11bf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c11bf-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c11bf-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="c11bf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c11bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c11bf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c11bf-113">Not supported.</span></span> |
| <span data-ttu-id="c11bf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c11bf-114">Application</span></span>                            | <span data-ttu-id="c11bf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c11bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c11bf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c11bf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="c11bf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c11bf-117">Request headers</span></span>

| <span data-ttu-id="c11bf-118">名称</span><span class="sxs-lookup"><span data-stu-id="c11bf-118">Name</span></span>       | <span data-ttu-id="c11bf-119">说明</span><span class="sxs-lookup"><span data-stu-id="c11bf-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c11bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c11bf-120">Authorization</span></span> | <span data-ttu-id="c11bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c11bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c11bf-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c11bf-123">Content-Type</span></span>  | <span data-ttu-id="c11bf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c11bf-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="c11bf-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="c11bf-126">Content-Language</span></span>  | <span data-ttu-id="c11bf-127">位置.</span><span class="sxs-lookup"><span data-stu-id="c11bf-127">Locale.</span></span> <span data-ttu-id="c11bf-128">可选。</span><span class="sxs-lookup"><span data-stu-id="c11bf-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c11bf-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c11bf-129">Request body</span></span>

<span data-ttu-id="c11bf-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c11bf-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c11bf-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c11bf-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c11bf-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c11bf-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c11bf-133">属性</span><span class="sxs-lookup"><span data-stu-id="c11bf-133">Property</span></span>     | <span data-ttu-id="c11bf-134">类型</span><span class="sxs-lookup"><span data-stu-id="c11bf-134">Type</span></span>        | <span data-ttu-id="c11bf-135">说明</span><span class="sxs-lookup"><span data-stu-id="c11bf-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c11bf-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="c11bf-136">backgroundColor</span></span>|<span data-ttu-id="c11bf-137">String</span><span class="sxs-lookup"><span data-stu-id="c11bf-137">String</span></span>|<span data-ttu-id="c11bf-138">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="c11bf-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="c11bf-139">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="c11bf-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="c11bf-140">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="c11bf-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="c11bf-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="c11bf-141">backgroundImage</span></span>|<span data-ttu-id="c11bf-142">Stream</span><span class="sxs-lookup"><span data-stu-id="c11bf-142">Stream</span></span>|<span data-ttu-id="c11bf-143">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="c11bf-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="c11bf-144">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="c11bf-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="c11bf-145">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="c11bf-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="c11bf-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="c11bf-146">bannerLogo</span></span>|<span data-ttu-id="c11bf-147">Stream</span><span class="sxs-lookup"><span data-stu-id="c11bf-147">Stream</span></span>|<span data-ttu-id="c11bf-148">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="c11bf-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="c11bf-149">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="c11bf-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="c11bf-150">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="c11bf-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="c11bf-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="c11bf-151">signInPageText</span></span>|<span data-ttu-id="c11bf-152">String</span><span class="sxs-lookup"><span data-stu-id="c11bf-152">String</span></span>|<span data-ttu-id="c11bf-153">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="c11bf-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="c11bf-154">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="c11bf-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="c11bf-155">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="c11bf-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="c11bf-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="c11bf-156">squareLogo</span></span>|<span data-ttu-id="c11bf-157">Stream</span><span class="sxs-lookup"><span data-stu-id="c11bf-157">Stream</span></span>|<span data-ttu-id="c11bf-158">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="c11bf-158">Square version of your company logo.</span></span> <span data-ttu-id="c11bf-159">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="c11bf-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="c11bf-160">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="c11bf-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="c11bf-161">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="c11bf-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="c11bf-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="c11bf-162">usernameHintText</span></span>|<span data-ttu-id="c11bf-163">String</span><span class="sxs-lookup"><span data-stu-id="c11bf-163">String</span></span>|<span data-ttu-id="c11bf-164">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="c11bf-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="c11bf-165">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="c11bf-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="c11bf-166">**Id** 属性在传入时被忽略。</span><span class="sxs-lookup"><span data-stu-id="c11bf-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="c11bf-167">响应</span><span class="sxs-lookup"><span data-stu-id="c11bf-167">Response</span></span>

<span data-ttu-id="c11bf-168">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c11bf-168">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c11bf-169">示例</span><span class="sxs-lookup"><span data-stu-id="c11bf-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="c11bf-170">示例1：更新默认品牌</span><span class="sxs-lookup"><span data-stu-id="c11bf-170">Example 1: Update default branding</span></span>
<span data-ttu-id="c11bf-171">如果署名已存在，则修补程序将仅替换指定的属性，但未指定的属性保持不变。</span><span class="sxs-lookup"><span data-stu-id="c11bf-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="c11bf-172">请求</span><span class="sxs-lookup"><span data-stu-id="c11bf-172">Request</span></span>

<span data-ttu-id="c11bf-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c11bf-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c11bf-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="c11bf-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[<span data-ttu-id="c11bf-175">C#</span><span class="sxs-lookup"><span data-stu-id="c11bf-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c11bf-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c11bf-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c11bf-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c11bf-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c11bf-178">Java</span><span class="sxs-lookup"><span data-stu-id="c11bf-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c11bf-179">响应</span><span class="sxs-lookup"><span data-stu-id="c11bf-179">Response</span></span>
<span data-ttu-id="c11bf-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c11bf-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="c11bf-181">在这种情况下，将更新默认/branding 的值，但不会对任何本地化更改任何值。</span><span class="sxs-lookup"><span data-stu-id="c11bf-181">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="c11bf-182">示例2：更新 bannerLogo 的默认品牌</span><span class="sxs-lookup"><span data-stu-id="c11bf-182">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="c11bf-183">以下请求更新默认品牌的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="c11bf-183">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="c11bf-184">请求</span><span class="sxs-lookup"><span data-stu-id="c11bf-184">Request</span></span>

<span data-ttu-id="c11bf-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c11bf-185">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c11bf-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="c11bf-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="c11bf-187">C#</span><span class="sxs-lookup"><span data-stu-id="c11bf-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c11bf-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c11bf-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c11bf-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c11bf-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c11bf-190">Java</span><span class="sxs-lookup"><span data-stu-id="c11bf-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c11bf-191">响应</span><span class="sxs-lookup"><span data-stu-id="c11bf-191">Response</span></span>
<span data-ttu-id="c11bf-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c11bf-192">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="c11bf-193">示例3：更新本地化品牌</span><span class="sxs-lookup"><span data-stu-id="c11bf-193">Example 3: Update localized branding</span></span>
<span data-ttu-id="c11bf-194">如果指定了 Content Language 标头，则会创建与内容语言关联的本地化，如果尚不存在，然后使用指定的值进行更新。</span><span class="sxs-lookup"><span data-stu-id="c11bf-194">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="c11bf-195">不更改默认品牌。</span><span class="sxs-lookup"><span data-stu-id="c11bf-195">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="c11bf-196">请求</span><span class="sxs-lookup"><span data-stu-id="c11bf-196">Request</span></span>

<span data-ttu-id="c11bf-197">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c11bf-197">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="c11bf-198">响应</span><span class="sxs-lookup"><span data-stu-id="c11bf-198">Response</span></span>
<span data-ttu-id="c11bf-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c11bf-199">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="c11bf-200">按照此请求，将使用 backgroundColor 的新值更新 fr-fr 本地化，但不会对默认/branding. 进行任何更改。</span><span class="sxs-lookup"><span data-stu-id="c11bf-200">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="c11bf-201">示例4：替换默认品牌和所有 localizations</span><span class="sxs-lookup"><span data-stu-id="c11bf-201">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="c11bf-202">如果品牌已存在，则 PUT 将替换默认品牌和任何 localizations。</span><span class="sxs-lookup"><span data-stu-id="c11bf-202">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="c11bf-203">请求</span><span class="sxs-lookup"><span data-stu-id="c11bf-203">Request</span></span>

<span data-ttu-id="c11bf-204">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c11bf-204">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c11bf-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="c11bf-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[<span data-ttu-id="c11bf-206">C#</span><span class="sxs-lookup"><span data-stu-id="c11bf-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c11bf-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c11bf-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c11bf-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c11bf-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c11bf-209">Java</span><span class="sxs-lookup"><span data-stu-id="c11bf-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c11bf-210">响应</span><span class="sxs-lookup"><span data-stu-id="c11bf-210">Response</span></span>
<span data-ttu-id="c11bf-211">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c11bf-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="c11bf-212">在此请求之后，默认署名仅具有指定的 backgroundColor，并且只具有一个 id 为 fr 的本地化，同时还具有 backgroundColor 集。</span><span class="sxs-lookup"><span data-stu-id="c11bf-212">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
