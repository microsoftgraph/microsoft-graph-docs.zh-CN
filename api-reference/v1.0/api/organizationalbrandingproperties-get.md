---
title: 获取 organizationalBrandingProperties
description: 检索 organizationalBrandingProperties 对象的属性和关系。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: df77f6b26cab6324574ce22335e0b0c3236ee7b9
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722537"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="9b766-103">获取 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="9b766-103">Get organizationalBrandingProperties</span></span>

<span data-ttu-id="9b766-104">检索 [organizationalBrandingProperties 对象的属性和](../resources/organizationalbrandingproperties.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9b766-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b766-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="9b766-105">Permissions</span></span>

<span data-ttu-id="9b766-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b766-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b766-108">Permission type</span></span>                        | <span data-ttu-id="9b766-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b766-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b766-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b766-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b766-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="9b766-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="9b766-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b766-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b766-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b766-113">Not supported.</span></span> |
| <span data-ttu-id="9b766-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b766-114">Application</span></span>                            | <span data-ttu-id="9b766-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b766-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b766-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b766-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="9b766-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b766-117">Request headers</span></span>

| <span data-ttu-id="9b766-118">名称</span><span class="sxs-lookup"><span data-stu-id="9b766-118">Name</span></span>      |<span data-ttu-id="9b766-119">说明</span><span class="sxs-lookup"><span data-stu-id="9b766-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b766-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b766-120">Authorization</span></span> | <span data-ttu-id="9b766-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b766-p102">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="9b766-123">如果在 Graph 浏览器中尝试查询，还必须包含具有有效 ISO-639 区域设置的 **Accept-Language** 请求标头。</span><span class="sxs-lookup"><span data-stu-id="9b766-123">If you try the query in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="9b766-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b766-124">Request body</span></span>

<span data-ttu-id="9b766-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b766-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b766-126">响应</span><span class="sxs-lookup"><span data-stu-id="9b766-126">Response</span></span>

<span data-ttu-id="9b766-127">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b766-127">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b766-128">示例</span><span class="sxs-lookup"><span data-stu-id="9b766-128">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="9b766-129">示例 1：获取默认品牌</span><span class="sxs-lookup"><span data-stu-id="9b766-129">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="9b766-130">如果尝试 Graph 浏览器中的示例，还必须包含具有有效 ISO-639 区域设置的 **Accept-Language** 请求标头，以避免收到错误"无效 *区域设置 id 值 en-US，en;q=0.9"。它必须是有效的 ISO-639 区域设置。*</span><span class="sxs-lookup"><span data-stu-id="9b766-130">If you try the example in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale to avoid getting an error "*Invalid locale id value en-US,en;q=0.9. It must be a valid ISO-639 locale.*"</span></span>

#### <a name="request"></a><span data-ttu-id="9b766-131">请求</span><span class="sxs-lookup"><span data-stu-id="9b766-131">Request</span></span>

<span data-ttu-id="9b766-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b766-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="9b766-133">响应</span><span class="sxs-lookup"><span data-stu-id="9b766-133">Response</span></span>

<span data-ttu-id="9b766-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b766-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9b766-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b766-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "backgroundColor":"#FFFF33",
  "backgroundImage@odata.mediaContentType":"image/*",
  "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "bannerLogo@odata.mediaContentType":"image/*",
  "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "id": "und",
  "squareLogo@odata.mediaContentType":"image/*",
  "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "signInPageText":"Default",
  "usernameHintText":"DefaultHint"
}
```

<span data-ttu-id="9b766-137">对 /branding 的请求始终返回 **mediaContentType、mediaReadLink** 和 **mediaEditLink** 属性。 </span><span class="sxs-lookup"><span data-stu-id="9b766-137">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="9b766-138">如果已应用区域设置，**则 mediaEditLink** 为区域设置 (（始终为非 null) ）的 **mediaEditLink;** 如果区域设置的 **mediaReadLink** 为非 null，则 **mediaReadLink** 和 **mediaContentType** 为区域设置中的 **mediaReadLink** 和 **mediaContentType;** 否则，默认 **mediaReadLink** 和 **mediaContentType**。</span><span class="sxs-lookup"><span data-stu-id="9b766-138">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="9b766-139">示例 2：获取组织品牌，但没有配置品牌</span><span class="sxs-lookup"><span data-stu-id="9b766-139">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="9b766-140">请求</span><span class="sxs-lookup"><span data-stu-id="9b766-140">Request</span></span>

<span data-ttu-id="9b766-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b766-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="9b766-142">响应</span><span class="sxs-lookup"><span data-stu-id="9b766-142">Response</span></span>

<span data-ttu-id="9b766-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b766-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="9b766-144">示例 3：获取法语区域设置的组织品牌</span><span class="sxs-lookup"><span data-stu-id="9b766-144">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="9b766-145">**Accept-Language** 标头用于将特定本地化应用到品牌。</span><span class="sxs-lookup"><span data-stu-id="9b766-145">The **Accept-Language** header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="9b766-146">指定 `null` 本地化中的属性从默认品牌返回。</span><span class="sxs-lookup"><span data-stu-id="9b766-146">Properties that are `null` in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="9b766-147">如果在 **请求中指定了 Accept-Language** 标头，则响应将包括 **Content-Language** 标头，除非是 `und` 。</span><span class="sxs-lookup"><span data-stu-id="9b766-147">If the **Accept-Language** header is specified in the request, the response will include the **Content-Language** header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="9b766-148">请求</span><span class="sxs-lookup"><span data-stu-id="9b766-148">Request</span></span>

<span data-ttu-id="9b766-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b766-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="9b766-150">响应</span><span class="sxs-lookup"><span data-stu-id="9b766-150">Response</span></span>

<span data-ttu-id="9b766-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b766-151">The following is an example of the response.</span></span>

> <span data-ttu-id="9b766-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b766-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "und",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="9b766-154">示例 4：获取法语区域设置的 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="9b766-154">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="9b766-155">如果 **区域设置** 存在， `fr` 则返回 bannerLogo。</span><span class="sxs-lookup"><span data-stu-id="9b766-155">Returns **bannerLogo** for the `fr` locale if it exists.</span></span> <span data-ttu-id="9b766-156">如果本地化不存在，则返回默认的 **bannerLogo**。</span><span class="sxs-lookup"><span data-stu-id="9b766-156">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="9b766-157">请求</span><span class="sxs-lookup"><span data-stu-id="9b766-157">Request</span></span>

<span data-ttu-id="9b766-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b766-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="9b766-159">响应</span><span class="sxs-lookup"><span data-stu-id="9b766-159">Response</span></span>

<span data-ttu-id="9b766-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b766-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
}
```

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="9b766-161">示例 5：在未配置 bannerLogo 时获取 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="9b766-161">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="9b766-162">本示例显示对默认品牌或 **Accept-Language** 标头中指定的语言上不存在的属性的请求。</span><span class="sxs-lookup"><span data-stu-id="9b766-162">This example shows a request for a property that does not exist on the default branding or the language specified in the **Accept-Language** header.</span></span>

#### <a name="request"></a><span data-ttu-id="9b766-163">请求</span><span class="sxs-lookup"><span data-stu-id="9b766-163">Request</span></span>

<span data-ttu-id="9b766-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b766-164">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="9b766-165">响应</span><span class="sxs-lookup"><span data-stu-id="9b766-165">Response</span></span>

<span data-ttu-id="9b766-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b766-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
