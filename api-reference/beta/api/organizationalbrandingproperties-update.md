---
title: 更新 organizationalBrandingProperties
description: 更新 organizationalBrandingProperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7655caa6e5c8eb1187bcc159f7f6d8c78641abc9
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031909"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="9de2d-103">更新 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="9de2d-103">Update organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9de2d-104">更新 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9de2d-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9de2d-105">权限</span><span class="sxs-lookup"><span data-stu-id="9de2d-105">Permissions</span></span>

<span data-ttu-id="9de2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9de2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9de2d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9de2d-108">Permission type</span></span>                        | <span data-ttu-id="9de2d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9de2d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9de2d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9de2d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9de2d-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de2d-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="9de2d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9de2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9de2d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9de2d-113">Not supported.</span></span> |
| <span data-ttu-id="9de2d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9de2d-114">Application</span></span>                            | <span data-ttu-id="9de2d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9de2d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9de2d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9de2d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="9de2d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9de2d-117">Request headers</span></span>

| <span data-ttu-id="9de2d-118">名称</span><span class="sxs-lookup"><span data-stu-id="9de2d-118">Name</span></span>       | <span data-ttu-id="9de2d-119">说明</span><span class="sxs-lookup"><span data-stu-id="9de2d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9de2d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9de2d-120">Authorization</span></span> | <span data-ttu-id="9de2d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9de2d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9de2d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9de2d-123">Content-Type</span></span>  | <span data-ttu-id="9de2d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9de2d-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="9de2d-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="9de2d-126">Content-Language</span></span>  | <span data-ttu-id="9de2d-127">位置.</span><span class="sxs-lookup"><span data-stu-id="9de2d-127">Locale.</span></span> <span data-ttu-id="9de2d-128">可选。</span><span class="sxs-lookup"><span data-stu-id="9de2d-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9de2d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9de2d-129">Request body</span></span>

<span data-ttu-id="9de2d-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9de2d-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9de2d-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9de2d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9de2d-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9de2d-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9de2d-133">属性</span><span class="sxs-lookup"><span data-stu-id="9de2d-133">Property</span></span>     | <span data-ttu-id="9de2d-134">类型</span><span class="sxs-lookup"><span data-stu-id="9de2d-134">Type</span></span>        | <span data-ttu-id="9de2d-135">Description</span><span class="sxs-lookup"><span data-stu-id="9de2d-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9de2d-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="9de2d-136">backgroundColor</span></span>|<span data-ttu-id="9de2d-137">String</span><span class="sxs-lookup"><span data-stu-id="9de2d-137">String</span></span>|<span data-ttu-id="9de2d-138">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="9de2d-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="9de2d-139">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="9de2d-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="9de2d-140">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="9de2d-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="9de2d-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="9de2d-141">backgroundImage</span></span>|<span data-ttu-id="9de2d-142">Stream</span><span class="sxs-lookup"><span data-stu-id="9de2d-142">Stream</span></span>|<span data-ttu-id="9de2d-143">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="9de2d-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="9de2d-144">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="9de2d-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="9de2d-145">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="9de2d-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="9de2d-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="9de2d-146">bannerLogo</span></span>|<span data-ttu-id="9de2d-147">Stream</span><span class="sxs-lookup"><span data-stu-id="9de2d-147">Stream</span></span>|<span data-ttu-id="9de2d-148">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="9de2d-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="9de2d-149">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="9de2d-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="9de2d-150">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="9de2d-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="9de2d-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="9de2d-151">signInPageText</span></span>|<span data-ttu-id="9de2d-152">String</span><span class="sxs-lookup"><span data-stu-id="9de2d-152">String</span></span>|<span data-ttu-id="9de2d-153">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="9de2d-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="9de2d-154">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="9de2d-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="9de2d-155">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="9de2d-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="9de2d-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="9de2d-156">squareLogo</span></span>|<span data-ttu-id="9de2d-157">Stream</span><span class="sxs-lookup"><span data-stu-id="9de2d-157">Stream</span></span>|<span data-ttu-id="9de2d-158">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="9de2d-158">Square version of your company logo.</span></span> <span data-ttu-id="9de2d-159">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="9de2d-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="9de2d-160">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="9de2d-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="9de2d-161">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="9de2d-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="9de2d-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="9de2d-162">usernameHintText</span></span>|<span data-ttu-id="9de2d-163">String</span><span class="sxs-lookup"><span data-stu-id="9de2d-163">String</span></span>|<span data-ttu-id="9de2d-164">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="9de2d-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="9de2d-165">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="9de2d-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="9de2d-166">**Id** 属性在传入时被忽略。</span><span class="sxs-lookup"><span data-stu-id="9de2d-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="9de2d-167">响应</span><span class="sxs-lookup"><span data-stu-id="9de2d-167">Response</span></span>

<span data-ttu-id="9de2d-168">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9de2d-168">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9de2d-169">示例</span><span class="sxs-lookup"><span data-stu-id="9de2d-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="9de2d-170">示例1：更新默认品牌</span><span class="sxs-lookup"><span data-stu-id="9de2d-170">Example 1: Update default branding</span></span>
<span data-ttu-id="9de2d-171">如果署名已存在，则修补程序将仅替换指定的属性，但未指定的属性保持不变。</span><span class="sxs-lookup"><span data-stu-id="9de2d-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="9de2d-172">请求</span><span class="sxs-lookup"><span data-stu-id="9de2d-172">Request</span></span>

<span data-ttu-id="9de2d-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9de2d-173">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9de2d-174">响应</span><span class="sxs-lookup"><span data-stu-id="9de2d-174">Response</span></span>
<span data-ttu-id="9de2d-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9de2d-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="9de2d-176">在这种情况下，将更新默认/branding 的值，但不会对任何本地化更改任何值。</span><span class="sxs-lookup"><span data-stu-id="9de2d-176">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="9de2d-177">示例2：更新 bannerLogo 的默认品牌</span><span class="sxs-lookup"><span data-stu-id="9de2d-177">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="9de2d-178">以下请求更新默认品牌的横幅徽标。</span><span class="sxs-lookup"><span data-stu-id="9de2d-178">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="9de2d-179">请求</span><span class="sxs-lookup"><span data-stu-id="9de2d-179">Request</span></span>

<span data-ttu-id="9de2d-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9de2d-180">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="9de2d-181">响应</span><span class="sxs-lookup"><span data-stu-id="9de2d-181">Response</span></span>
<span data-ttu-id="9de2d-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9de2d-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="9de2d-183">示例3：更新本地化品牌</span><span class="sxs-lookup"><span data-stu-id="9de2d-183">Example 3: Update localized branding</span></span>
<span data-ttu-id="9de2d-184">如果指定了 Content Language 标头，则会创建与内容语言关联的本地化，如果尚不存在，然后使用指定的值进行更新。</span><span class="sxs-lookup"><span data-stu-id="9de2d-184">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="9de2d-185">不更改默认品牌。</span><span class="sxs-lookup"><span data-stu-id="9de2d-185">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="9de2d-186">请求</span><span class="sxs-lookup"><span data-stu-id="9de2d-186">Request</span></span>

<span data-ttu-id="9de2d-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9de2d-187">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9de2d-188">响应</span><span class="sxs-lookup"><span data-stu-id="9de2d-188">Response</span></span>
<span data-ttu-id="9de2d-189">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9de2d-189">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="9de2d-190">按照此请求，将使用 backgroundColor 的新值更新 fr-fr 本地化，但不会对默认/branding. 进行任何更改。</span><span class="sxs-lookup"><span data-stu-id="9de2d-190">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="9de2d-191">示例4：替换默认品牌和所有 localizations</span><span class="sxs-lookup"><span data-stu-id="9de2d-191">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="9de2d-192">如果品牌已存在，则 PUT 将替换默认品牌和任何 localizations。</span><span class="sxs-lookup"><span data-stu-id="9de2d-192">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="9de2d-193">请求</span><span class="sxs-lookup"><span data-stu-id="9de2d-193">Request</span></span>

<span data-ttu-id="9de2d-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9de2d-194">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9de2d-195">响应</span><span class="sxs-lookup"><span data-stu-id="9de2d-195">Response</span></span>
<span data-ttu-id="9de2d-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9de2d-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="9de2d-197">在此请求之后，默认署名仅具有指定的 backgroundColor，并且只具有一个 id 为 fr 的本地化，同时还具有 backgroundColor 集。</span><span class="sxs-lookup"><span data-stu-id="9de2d-197">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
