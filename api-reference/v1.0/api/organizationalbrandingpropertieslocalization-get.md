---
title: 获取本地化的组织BrandingProperties
description: 检索特定区域设置的组织品牌属性对象。
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6286aff9e9a128efbaf1f15a7d2150a5f9754b2b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682465"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="096ed-103">获取本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="096ed-103">Get Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="096ed-104">检索 [organizationalBrandingProperties 对象](../resources/organizationalbrandingproperties.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="096ed-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="096ed-105">权限</span><span class="sxs-lookup"><span data-stu-id="096ed-105">Permissions</span></span>

<span data-ttu-id="096ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="096ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="096ed-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="096ed-108">Permission type</span></span>                        | <span data-ttu-id="096ed-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="096ed-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="096ed-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="096ed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="096ed-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="096ed-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="096ed-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="096ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="096ed-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="096ed-113">Not supported.</span></span> |
| <span data-ttu-id="096ed-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="096ed-114">Application</span></span>                            | <span data-ttu-id="096ed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="096ed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="096ed-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="096ed-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{tenant id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="096ed-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="096ed-117">Request headers</span></span>

| <span data-ttu-id="096ed-118">名称</span><span class="sxs-lookup"><span data-stu-id="096ed-118">Name</span></span>      |<span data-ttu-id="096ed-119">说明</span><span class="sxs-lookup"><span data-stu-id="096ed-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="096ed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="096ed-120">Authorization</span></span> | <span data-ttu-id="096ed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="096ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="096ed-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="096ed-123">Content-Type</span></span>  | <span data-ttu-id="096ed-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="096ed-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="096ed-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="096ed-126">Request body</span></span>

<span data-ttu-id="096ed-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="096ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="096ed-128">响应</span><span class="sxs-lookup"><span data-stu-id="096ed-128">Response</span></span>

<span data-ttu-id="096ed-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="096ed-129">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="096ed-130">"id"的值对应于请求的本地化。</span><span class="sxs-lookup"><span data-stu-id="096ed-130">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="096ed-131">示例</span><span class="sxs-lookup"><span data-stu-id="096ed-131">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="096ed-132">示例 1：获取特定区域设置或 (本地化) </span><span class="sxs-lookup"><span data-stu-id="096ed-132">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="096ed-133">对特定本地化的 GET 请求仅返回该本地化的值。</span><span class="sxs-lookup"><span data-stu-id="096ed-133">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="096ed-134">空值不会替换为默认品牌中的值。</span><span class="sxs-lookup"><span data-stu-id="096ed-134">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="096ed-135">请求</span><span class="sxs-lookup"><span data-stu-id="096ed-135">Request</span></span>

<span data-ttu-id="096ed-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="096ed-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="096ed-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="096ed-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_8"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="096ed-138">C#</span><span class="sxs-lookup"><span data-stu-id="096ed-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096ed-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096ed-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096ed-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096ed-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096ed-141">Java</span><span class="sxs-lookup"><span data-stu-id="096ed-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="096ed-142">响应</span><span class="sxs-lookup"><span data-stu-id="096ed-142">Response</span></span>

<span data-ttu-id="096ed-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="096ed-143">The following is an example of the response.</span></span>

> <span data-ttu-id="096ed-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="096ed-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
"backgroundColor":"#00000F",
"backgroundImage@odata.mediaContentType":"image/*",
"backgroundImage@odata.mediaReadLink": null,
"backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
"bannerLogo@odata.mediaContentType":"image/*",
"bannerLogo@odata.mediaReadLink": null,
"bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
"id":"fr",
"squareLogo@odata.mediaContentType":"image/*",
"squareLogo@odata.mediaReadLink": null,
"squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
"signInPageText":null,
"usernameHintText":null
}
```

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="096ed-145">示例 2：获取已配置的所有特定语言的本地化</span><span class="sxs-lookup"><span data-stu-id="096ed-145">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="096ed-146">请求</span><span class="sxs-lookup"><span data-stu-id="096ed-146">Request</span></span>

<span data-ttu-id="096ed-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="096ed-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="096ed-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="096ed-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_9"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="096ed-149">C#</span><span class="sxs-lookup"><span data-stu-id="096ed-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-9-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096ed-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096ed-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-9-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096ed-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096ed-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-9-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096ed-152">Java</span><span class="sxs-lookup"><span data-stu-id="096ed-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-9-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="096ed-153">响应</span><span class="sxs-lookup"><span data-stu-id="096ed-153">Response</span></span>

<span data-ttu-id="096ed-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="096ed-154">The following is an example of the response.</span></span>

> <span data-ttu-id="096ed-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="096ed-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "values": [
   {
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "backgroundImage@odata.mediaEditLink":"https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id":"en-us",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
   },
   {
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id":"fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":null,
    "usernameHintText":null
   }
 ]
}
```

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="096ed-156">示例 3：获取特定区域设置 signInPageText 的值</span><span class="sxs-lookup"><span data-stu-id="096ed-156">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="096ed-157">请求本地化的属性将返回该值，如果值为 null，则返回 204。</span><span class="sxs-lookup"><span data-stu-id="096ed-157">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="096ed-158">请求</span><span class="sxs-lookup"><span data-stu-id="096ed-158">Request</span></span>

<span data-ttu-id="096ed-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="096ed-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="096ed-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="096ed-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_10"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="096ed-161">C#</span><span class="sxs-lookup"><span data-stu-id="096ed-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-10-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096ed-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096ed-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-10-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096ed-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096ed-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-10-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096ed-164">Java</span><span class="sxs-lookup"><span data-stu-id="096ed-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-10-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="096ed-165">响应</span><span class="sxs-lookup"><span data-stu-id="096ed-165">Response</span></span>

<span data-ttu-id="096ed-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="096ed-166">The following is an example of the response.</span></span>

> <span data-ttu-id="096ed-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="096ed-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
"value":"Welcome"
}
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
