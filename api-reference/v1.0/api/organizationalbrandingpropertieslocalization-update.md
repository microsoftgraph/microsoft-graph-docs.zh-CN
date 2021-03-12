---
title: 更新本地化的组织品牌设置
description: 更新特定本地化的 organizationalbrandingproperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0c38656b71c2fdc5b3832a106effecfe9970c811
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722532"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="25f3a-103">更新本地化的组织品牌设置</span><span class="sxs-lookup"><span data-stu-id="25f3a-103">Update localized organizationalbrandingproperties</span></span>

<span data-ttu-id="25f3a-104">更新 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性，以用于特定本地化。</span><span class="sxs-lookup"><span data-stu-id="25f3a-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="25f3a-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="25f3a-105">Permissions</span></span>

<span data-ttu-id="25f3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25f3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25f3a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="25f3a-108">Permission type</span></span>                        | <span data-ttu-id="25f3a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25f3a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25f3a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25f3a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="25f3a-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25f3a-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="25f3a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25f3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25f3a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="25f3a-113">Not supported.</span></span> |
| <span data-ttu-id="25f3a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="25f3a-114">Application</span></span>                            | <span data-ttu-id="25f3a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25f3a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25f3a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25f3a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="25f3a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="25f3a-117">Request headers</span></span>

| <span data-ttu-id="25f3a-118">名称</span><span class="sxs-lookup"><span data-stu-id="25f3a-118">Name</span></span>       | <span data-ttu-id="25f3a-119">说明</span><span class="sxs-lookup"><span data-stu-id="25f3a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="25f3a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="25f3a-120">Authorization</span></span> | <span data-ttu-id="25f3a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25f3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25f3a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25f3a-123">Content-Type</span></span>  | <span data-ttu-id="25f3a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="25f3a-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="25f3a-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="25f3a-126">Content-Language</span></span>  | <span data-ttu-id="25f3a-127">区域设置。</span><span class="sxs-lookup"><span data-stu-id="25f3a-127">Locale.</span></span> <span data-ttu-id="25f3a-128">可选。</span><span class="sxs-lookup"><span data-stu-id="25f3a-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25f3a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="25f3a-129">Request body</span></span>

<span data-ttu-id="25f3a-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="25f3a-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="25f3a-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="25f3a-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="25f3a-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="25f3a-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="25f3a-133">属性</span><span class="sxs-lookup"><span data-stu-id="25f3a-133">Property</span></span>     | <span data-ttu-id="25f3a-134">类型</span><span class="sxs-lookup"><span data-stu-id="25f3a-134">Type</span></span>        | <span data-ttu-id="25f3a-135">说明</span><span class="sxs-lookup"><span data-stu-id="25f3a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25f3a-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="25f3a-136">backgroundColor</span></span>|<span data-ttu-id="25f3a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="25f3a-137">String</span></span>|<span data-ttu-id="25f3a-138">将出现在低带宽连接中的背景图像上的颜色。</span><span class="sxs-lookup"><span data-stu-id="25f3a-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="25f3a-139">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="25f3a-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="25f3a-140">以十六进制表示 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="25f3a-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="25f3a-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="25f3a-141">backgroundImage</span></span>|<span data-ttu-id="25f3a-142">Stream</span><span class="sxs-lookup"><span data-stu-id="25f3a-142">Stream</span></span>|<span data-ttu-id="25f3a-143">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="25f3a-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="25f3a-144">.png 或 .jpg 不大于 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="25f3a-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="25f3a-145">较小的图像将降低带宽要求，提高页面加载性能。</span><span class="sxs-lookup"><span data-stu-id="25f3a-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="25f3a-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="25f3a-146">bannerLogo</span></span>|<span data-ttu-id="25f3a-147">Stream</span><span class="sxs-lookup"><span data-stu-id="25f3a-147">Stream</span></span>|<span data-ttu-id="25f3a-148">显示在登录页上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="25f3a-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="25f3a-149">.png 或 .jpg 不超过 36x245px。</span><span class="sxs-lookup"><span data-stu-id="25f3a-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="25f3a-150">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="25f3a-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="25f3a-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="25f3a-151">signInPageText</span></span>|<span data-ttu-id="25f3a-152">字符串</span><span class="sxs-lookup"><span data-stu-id="25f3a-152">String</span></span>|<span data-ttu-id="25f3a-153">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="25f3a-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="25f3a-154">您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="25f3a-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="25f3a-155">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="25f3a-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="25f3a-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="25f3a-156">squareLogo</span></span>|<span data-ttu-id="25f3a-157">Stream</span><span class="sxs-lookup"><span data-stu-id="25f3a-157">Stream</span></span>|<span data-ttu-id="25f3a-158">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="25f3a-158">Square version of your company logo.</span></span> <span data-ttu-id="25f3a-159">这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="25f3a-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="25f3a-160">.png 或 .jpg 不超过 240x240px 且大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="25f3a-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="25f3a-161">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="25f3a-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="25f3a-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="25f3a-162">usernameHintText</span></span>|<span data-ttu-id="25f3a-163">字符串</span><span class="sxs-lookup"><span data-stu-id="25f3a-163">String</span></span>|<span data-ttu-id="25f3a-164">字符串，在登录屏幕的用户名文本框中作为提示显示。</span><span class="sxs-lookup"><span data-stu-id="25f3a-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="25f3a-165">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="25f3a-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="25f3a-166">id</span><span class="sxs-lookup"><span data-stu-id="25f3a-166">id</span></span>|<span data-ttu-id="25f3a-167">字符串</span><span class="sxs-lookup"><span data-stu-id="25f3a-167">String</span></span>|<span data-ttu-id="25f3a-168">要更新其品牌设置的本地设置</span><span class="sxs-lookup"><span data-stu-id="25f3a-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="25f3a-169">响应</span><span class="sxs-lookup"><span data-stu-id="25f3a-169">Response</span></span>

<span data-ttu-id="25f3a-170">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25f3a-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25f3a-171">示例</span><span class="sxs-lookup"><span data-stu-id="25f3a-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="25f3a-172">示例 1：使用 PUT 为 fr 本地化设置 **bannerLogo**</span><span class="sxs-lookup"><span data-stu-id="25f3a-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="25f3a-173">以下请求更新本地化的横幅 `fr` 徽标。</span><span class="sxs-lookup"><span data-stu-id="25f3a-173">The following request updates the banner logo for the `fr` localization.</span></span> <span data-ttu-id="25f3a-174">使用 PUT 时，如果 fr 本地化不存在， `404 not found` 则返回错误。</span><span class="sxs-lookup"><span data-stu-id="25f3a-174">Using PUT, if the fr localization does not exist, a `404 not found` error is returned.</span></span> <span data-ttu-id="25f3a-175">如果有效负载包含 `id` 属性或 **Content-Language** 标头，并且它们在 URL 中不匹配， `id` `Bad Request` 则返回错误。</span><span class="sxs-lookup"><span data-stu-id="25f3a-175">If the payload contains an `id` property or **Content-Language** header, and they don't match `id` in URL, a `Bad Request` error is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="25f3a-176">请求</span><span class="sxs-lookup"><span data-stu-id="25f3a-176">Request</span></span>

<span data-ttu-id="25f3a-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25f3a-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="25f3a-178">响应</span><span class="sxs-lookup"><span data-stu-id="25f3a-178">Response</span></span>

<span data-ttu-id="25f3a-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25f3a-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="25f3a-180">示例 2：使用 PATCH 更新 fr 本地化的 **bannerLogo**</span><span class="sxs-lookup"><span data-stu-id="25f3a-180">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="25f3a-181">以下请求更新 fr 本地化的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="25f3a-181">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="25f3a-182">使用 PATCH，如果指定的本地化尚未存在，将创建它，并写入属性。</span><span class="sxs-lookup"><span data-stu-id="25f3a-182">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="25f3a-183">请求</span><span class="sxs-lookup"><span data-stu-id="25f3a-183">Request</span></span>

<span data-ttu-id="25f3a-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25f3a-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a><span data-ttu-id="25f3a-185">响应</span><span class="sxs-lookup"><span data-stu-id="25f3a-185">Response</span></span>
<span data-ttu-id="25f3a-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25f3a-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="25f3a-187">示例 3：使用空字符串替代默认品牌值</span><span class="sxs-lookup"><span data-stu-id="25f3a-187">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="25f3a-188">如果本地化中的属性值为 null，则该值将继承自默认品牌。</span><span class="sxs-lookup"><span data-stu-id="25f3a-188">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="25f3a-189">为了防止发生这种情况，请设置一个空字符串或字符串，其中仅包含本地化品牌中的空白。</span><span class="sxs-lookup"><span data-stu-id="25f3a-189">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="25f3a-190">请求</span><span class="sxs-lookup"><span data-stu-id="25f3a-190">Request</span></span>

<span data-ttu-id="25f3a-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25f3a-191">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="25f3a-192">响应</span><span class="sxs-lookup"><span data-stu-id="25f3a-192">Response</span></span>

<span data-ttu-id="25f3a-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25f3a-193">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="25f3a-194">在此请求后，fr 本地化的 usernameHintText 将为空，而不是从默认品牌继承值。</span><span class="sxs-lookup"><span data-stu-id="25f3a-194">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="25f3a-195">示例 4：将法语本地化替换为 PUT</span><span class="sxs-lookup"><span data-stu-id="25f3a-195">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="25f3a-196">若要使用 PUT 更新本地化，应在正文中添加所有属性以及需要更新的属性，因为 PUT 将现有对象替换为新对象。</span><span class="sxs-lookup"><span data-stu-id="25f3a-196">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="25f3a-197">其他不在 PUT 的有效负载正文中的属性将设置为 NULL。</span><span class="sxs-lookup"><span data-stu-id="25f3a-197">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="25f3a-198">下面的示例中，仅保留 backgroundColor 属性，并更新 signInPageText，而其他属性设置为 null。</span><span class="sxs-lookup"><span data-stu-id="25f3a-198">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="25f3a-199">如果指定的本地化不存在，PUT 到指定本地化创建它的 URL。</span><span class="sxs-lookup"><span data-stu-id="25f3a-199">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="25f3a-200">如果有效负载包含 id 属性或 Content-Language 标头，并且它们与 URL 中的 id 不匹配，我们将引发错误请求。</span><span class="sxs-lookup"><span data-stu-id="25f3a-200">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="25f3a-201">请求</span><span class="sxs-lookup"><span data-stu-id="25f3a-201">Request</span></span>

<span data-ttu-id="25f3a-202">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25f3a-202">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a><span data-ttu-id="25f3a-203">响应</span><span class="sxs-lookup"><span data-stu-id="25f3a-203">Response</span></span>
<span data-ttu-id="25f3a-204">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25f3a-204">The following is an example of the response.</span></span>

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
