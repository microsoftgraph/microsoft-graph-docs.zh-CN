---
title: 更新 organizationalBrandingProperties
description: 更新 organizationalBrandingProperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1fd15c3ae41af043cb7c5163d8b7ac8b06a36ae0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722536"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="8a294-103">更新 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="8a294-103">Update organizationalBrandingProperties</span></span>

<span data-ttu-id="8a294-104">更新 [organizationalBrandingProperties 对象](../resources/organizationalbrandingproperties.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8a294-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a294-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8a294-105">Permissions</span></span>

<span data-ttu-id="8a294-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a294-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a294-108">Permission type</span></span>                        | <span data-ttu-id="8a294-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a294-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8a294-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a294-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a294-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a294-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="8a294-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a294-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a294-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a294-113">Not supported.</span></span> |
| <span data-ttu-id="8a294-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a294-114">Application</span></span>                            | <span data-ttu-id="8a294-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a294-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a294-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a294-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="8a294-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a294-117">Request headers</span></span>

| <span data-ttu-id="8a294-118">名称</span><span class="sxs-lookup"><span data-stu-id="8a294-118">Name</span></span>       | <span data-ttu-id="8a294-119">说明</span><span class="sxs-lookup"><span data-stu-id="8a294-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8a294-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a294-120">Authorization</span></span> | <span data-ttu-id="8a294-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a294-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a294-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a294-123">Content-Type</span></span>  | <span data-ttu-id="8a294-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8a294-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="8a294-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="8a294-126">Content-Language</span></span>  | <span data-ttu-id="8a294-127">区域设置。</span><span class="sxs-lookup"><span data-stu-id="8a294-127">Locale.</span></span> <span data-ttu-id="8a294-128">可选。</span><span class="sxs-lookup"><span data-stu-id="8a294-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a294-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a294-129">Request body</span></span>

<span data-ttu-id="8a294-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8a294-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8a294-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8a294-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8a294-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8a294-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a294-133">属性</span><span class="sxs-lookup"><span data-stu-id="8a294-133">Property</span></span>     | <span data-ttu-id="8a294-134">类型</span><span class="sxs-lookup"><span data-stu-id="8a294-134">Type</span></span>        | <span data-ttu-id="8a294-135">说明</span><span class="sxs-lookup"><span data-stu-id="8a294-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a294-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="8a294-136">backgroundColor</span></span>|<span data-ttu-id="8a294-137">字符串</span><span class="sxs-lookup"><span data-stu-id="8a294-137">String</span></span>|<span data-ttu-id="8a294-138">将出现在低带宽连接中的背景图像上的颜色。</span><span class="sxs-lookup"><span data-stu-id="8a294-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="8a294-139">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="8a294-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="8a294-140">以十六进制表示 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="8a294-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="8a294-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="8a294-141">backgroundImage</span></span>|<span data-ttu-id="8a294-142">Stream</span><span class="sxs-lookup"><span data-stu-id="8a294-142">Stream</span></span>|<span data-ttu-id="8a294-143">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="8a294-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="8a294-144">.png 或 .jpg 不大于 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="8a294-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="8a294-145">较小的图像将降低带宽要求，提高页面加载性能。</span><span class="sxs-lookup"><span data-stu-id="8a294-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="8a294-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="8a294-146">bannerLogo</span></span>|<span data-ttu-id="8a294-147">Stream</span><span class="sxs-lookup"><span data-stu-id="8a294-147">Stream</span></span>|<span data-ttu-id="8a294-148">显示在登录页上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="8a294-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="8a294-149">.png 或 .jpg 不超过 36x245px。</span><span class="sxs-lookup"><span data-stu-id="8a294-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="8a294-150">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="8a294-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="8a294-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="8a294-151">signInPageText</span></span>|<span data-ttu-id="8a294-152">字符串</span><span class="sxs-lookup"><span data-stu-id="8a294-152">String</span></span>|<span data-ttu-id="8a294-153">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="8a294-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="8a294-154">您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="8a294-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="8a294-155">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="8a294-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="8a294-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="8a294-156">squareLogo</span></span>|<span data-ttu-id="8a294-157">Stream</span><span class="sxs-lookup"><span data-stu-id="8a294-157">Stream</span></span>|<span data-ttu-id="8a294-158">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="8a294-158">Square version of your company logo.</span></span> <span data-ttu-id="8a294-159">这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="8a294-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="8a294-160">.png 或 .jpg 不超过 240x240px 且大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="8a294-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="8a294-161">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="8a294-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="8a294-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="8a294-162">usernameHintText</span></span>|<span data-ttu-id="8a294-163">字符串</span><span class="sxs-lookup"><span data-stu-id="8a294-163">String</span></span>|<span data-ttu-id="8a294-164">字符串，在登录屏幕的用户名文本框中作为提示显示。</span><span class="sxs-lookup"><span data-stu-id="8a294-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="8a294-165">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="8a294-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="8a294-166">传入 `id` 时将忽略该属性。</span><span class="sxs-lookup"><span data-stu-id="8a294-166">The `id` property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="8a294-167">响应</span><span class="sxs-lookup"><span data-stu-id="8a294-167">Response</span></span>

<span data-ttu-id="8a294-168">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8a294-168">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8a294-169">示例</span><span class="sxs-lookup"><span data-stu-id="8a294-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="8a294-170">示例 1：更新默认品牌</span><span class="sxs-lookup"><span data-stu-id="8a294-170">Example 1: Update default branding</span></span>
<span data-ttu-id="8a294-171">如果品牌已存在，PATCH 将仅替换指定的属性，保留未指定的属性不变。</span><span class="sxs-lookup"><span data-stu-id="8a294-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="8a294-172">请求</span><span class="sxs-lookup"><span data-stu-id="8a294-172">Request</span></span>

<span data-ttu-id="8a294-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a294-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

#### <a name="response"></a><span data-ttu-id="8a294-174">响应</span><span class="sxs-lookup"><span data-stu-id="8a294-174">Response</span></span>
<span data-ttu-id="8a294-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a294-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="8a294-176">在这种情况下，默认 /branding 的值会更新，但在任何本地化上不会更改任何值。</span><span class="sxs-lookup"><span data-stu-id="8a294-176">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="8a294-177">示例 2：为默认品牌更新 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="8a294-177">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="8a294-178">以下请求更新默认品牌打造的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="8a294-178">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="8a294-179">请求</span><span class="sxs-lookup"><span data-stu-id="8a294-179">Request</span></span>

<span data-ttu-id="8a294-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a294-180">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="8a294-181">响应</span><span class="sxs-lookup"><span data-stu-id="8a294-181">Response</span></span>
<span data-ttu-id="8a294-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a294-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="8a294-183">示例 3：更新本地化品牌</span><span class="sxs-lookup"><span data-stu-id="8a294-183">Example 3: Update localized branding</span></span>
<span data-ttu-id="8a294-184">如果指定了 Content-Language 标头，则创建与 Content-Language 关联的本地化（如果不存在的话）然后使用指定的值进行更新。</span><span class="sxs-lookup"><span data-stu-id="8a294-184">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="8a294-185">默认品牌不会更改。</span><span class="sxs-lookup"><span data-stu-id="8a294-185">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="8a294-186">请求</span><span class="sxs-lookup"><span data-stu-id="8a294-186">Request</span></span>

<span data-ttu-id="8a294-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a294-187">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="8a294-188">响应</span><span class="sxs-lookup"><span data-stu-id="8a294-188">Response</span></span>
<span data-ttu-id="8a294-189">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a294-189">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="8a294-190">在此请求后，fr 本地化会使用 backgroundColor 的新值进行更新，但对默认 /branding 没有任何更改。</span><span class="sxs-lookup"><span data-stu-id="8a294-190">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="8a294-191">示例 4：替换默认品牌和所有本地化</span><span class="sxs-lookup"><span data-stu-id="8a294-191">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="8a294-192">如果品牌已存在，PUT 将替换默认品牌和任何本地化。</span><span class="sxs-lookup"><span data-stu-id="8a294-192">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="8a294-193">请求</span><span class="sxs-lookup"><span data-stu-id="8a294-193">Request</span></span>

<span data-ttu-id="8a294-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a294-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="8a294-195">响应</span><span class="sxs-lookup"><span data-stu-id="8a294-195">Response</span></span>
<span data-ttu-id="8a294-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a294-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="8a294-197">在此请求后，默认品牌仅指定了 backgroundColor，并且具有 id fr 以及 backgroundColor 集的仅一个本地化。</span><span class="sxs-lookup"><span data-stu-id="8a294-197">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
