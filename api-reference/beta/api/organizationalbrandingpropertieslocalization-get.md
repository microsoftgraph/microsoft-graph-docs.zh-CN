---
title: 获取本地化的组织BrandingProperties
description: 检索特定区域设置的组织品牌属性对象。
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 003688ed17b1fa5486d9482257cfdff8451fc3b8
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582695"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="08c43-103">获取本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="08c43-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08c43-104">检索 [organizationalBrandingProperties 对象](../resources/organizationalbrandingproperties.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="08c43-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08c43-105">权限</span><span class="sxs-lookup"><span data-stu-id="08c43-105">Permissions</span></span>

<span data-ttu-id="08c43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08c43-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="08c43-108">Permission type</span></span>                        | <span data-ttu-id="08c43-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08c43-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08c43-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08c43-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="08c43-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="08c43-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="08c43-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08c43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08c43-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c43-113">Not supported.</span></span> |
| <span data-ttu-id="08c43-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="08c43-114">Application</span></span>                            | <span data-ttu-id="08c43-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08c43-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08c43-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08c43-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="08c43-117">Optional query parameters</span></span>

<span data-ttu-id="08c43-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="08c43-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="08c43-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="08c43-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="08c43-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08c43-120">Request headers</span></span>

| <span data-ttu-id="08c43-121">名称</span><span class="sxs-lookup"><span data-stu-id="08c43-121">Name</span></span>      |<span data-ttu-id="08c43-122">说明</span><span class="sxs-lookup"><span data-stu-id="08c43-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08c43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c43-123">Authorization</span></span> | <span data-ttu-id="08c43-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08c43-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08c43-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08c43-126">Content-Type</span></span>  | <span data-ttu-id="08c43-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="08c43-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08c43-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="08c43-129">Request body</span></span>

<span data-ttu-id="08c43-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08c43-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08c43-131">响应</span><span class="sxs-lookup"><span data-stu-id="08c43-131">Response</span></span>

<span data-ttu-id="08c43-132">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08c43-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="08c43-133">"id"的值对应于请求的本地化。</span><span class="sxs-lookup"><span data-stu-id="08c43-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="08c43-134">示例</span><span class="sxs-lookup"><span data-stu-id="08c43-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="08c43-135">示例 1：获取特定区域设置或 (本地化) </span><span class="sxs-lookup"><span data-stu-id="08c43-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="08c43-136">对特定本地化的 GET 请求仅返回该本地化的值。</span><span class="sxs-lookup"><span data-stu-id="08c43-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="08c43-137">空值不会替换为默认品牌中的值。</span><span class="sxs-lookup"><span data-stu-id="08c43-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="08c43-138">请求</span><span class="sxs-lookup"><span data-stu-id="08c43-138">Request</span></span>

<span data-ttu-id="08c43-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08c43-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08c43-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="08c43-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_8"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="08c43-141">C#</span><span class="sxs-lookup"><span data-stu-id="08c43-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08c43-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08c43-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08c43-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08c43-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08c43-144">Java</span><span class="sxs-lookup"><span data-stu-id="08c43-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08c43-145">响应</span><span class="sxs-lookup"><span data-stu-id="08c43-145">Response</span></span>

<span data-ttu-id="08c43-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08c43-146">The following is an example of the response.</span></span>

> <span data-ttu-id="08c43-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="08c43-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
"backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
"bannerLogo@odata.mediaContentType":"image/*",
"bannerLogo@odata.mediaReadLink": null,
"bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
"id":"fr",
"squareLogo@odata.mediaContentType":"image/*",
"squareLogo@odata.mediaReadLink": null,
"squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
"signInPageText":null,
"usernameHintText":null
}
```

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="08c43-149">示例 2：获取已配置的所有特定语言的本地化</span><span class="sxs-lookup"><span data-stu-id="08c43-149">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="08c43-150">请求</span><span class="sxs-lookup"><span data-stu-id="08c43-150">Request</span></span>

<span data-ttu-id="08c43-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08c43-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08c43-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="08c43-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_9"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="08c43-153">C#</span><span class="sxs-lookup"><span data-stu-id="08c43-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-9-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08c43-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08c43-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-9-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08c43-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08c43-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-9-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08c43-156">Java</span><span class="sxs-lookup"><span data-stu-id="08c43-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-9-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08c43-157">响应</span><span class="sxs-lookup"><span data-stu-id="08c43-157">Response</span></span>

<span data-ttu-id="08c43-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08c43-158">The following is an example of the response.</span></span>

> <span data-ttu-id="08c43-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="08c43-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "backgroundImage@odata.mediaEditLink":"https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id":"en-us",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
   },
   {
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id":"fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":null,
    "usernameHintText":null
   }
 ]
}
```

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="08c43-161">示例 3：获取特定区域设置 signInPageText 的值</span><span class="sxs-lookup"><span data-stu-id="08c43-161">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="08c43-162">请求本地化的属性将返回该值，如果值为 null，则返回 204。</span><span class="sxs-lookup"><span data-stu-id="08c43-162">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="08c43-163">请求</span><span class="sxs-lookup"><span data-stu-id="08c43-163">Request</span></span>

<span data-ttu-id="08c43-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08c43-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08c43-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="08c43-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_10"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="08c43-166">C#</span><span class="sxs-lookup"><span data-stu-id="08c43-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-10-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08c43-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08c43-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-10-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08c43-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08c43-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-10-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08c43-169">Java</span><span class="sxs-lookup"><span data-stu-id="08c43-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-10-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08c43-170">响应</span><span class="sxs-lookup"><span data-stu-id="08c43-170">Response</span></span>

<span data-ttu-id="08c43-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08c43-171">The following is an example of the response.</span></span>

> <span data-ttu-id="08c43-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="08c43-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
