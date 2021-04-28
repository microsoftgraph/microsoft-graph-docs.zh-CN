---
title: 获取 organizationalBrandingProperties
description: 检索 organizationalBrandingProperties 对象的属性和关系。
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0eaf4bb551a1f75faa3c68252ca7ec72d7ced189
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052213"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="516b3-103">获取 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="516b3-103">Get organizationalBrandingProperties</span></span>

<span data-ttu-id="516b3-104">检索 [organizationalBrandingProperties 对象的属性和](../resources/organizationalbrandingproperties.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="516b3-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="516b3-105">权限</span><span class="sxs-lookup"><span data-stu-id="516b3-105">Permissions</span></span>

<span data-ttu-id="516b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="516b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="516b3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="516b3-108">Permission type</span></span>                        | <span data-ttu-id="516b3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="516b3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="516b3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="516b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="516b3-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="516b3-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="516b3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="516b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="516b3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="516b3-113">Not supported.</span></span> |
| <span data-ttu-id="516b3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="516b3-114">Application</span></span>                            | <span data-ttu-id="516b3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="516b3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="516b3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="516b3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="516b3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="516b3-117">Request headers</span></span>

| <span data-ttu-id="516b3-118">名称</span><span class="sxs-lookup"><span data-stu-id="516b3-118">Name</span></span>      |<span data-ttu-id="516b3-119">说明</span><span class="sxs-lookup"><span data-stu-id="516b3-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="516b3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="516b3-120">Authorization</span></span> | <span data-ttu-id="516b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="516b3-p102">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="516b3-123">如果在资源管理器中尝试Graph，还必须包含具有有效 ISO-639 区域设置的 **Accept-Language** 请求标头。</span><span class="sxs-lookup"><span data-stu-id="516b3-123">If you try the query in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="516b3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="516b3-124">Request body</span></span>

<span data-ttu-id="516b3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="516b3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="516b3-126">响应</span><span class="sxs-lookup"><span data-stu-id="516b3-126">Response</span></span>

<span data-ttu-id="516b3-127">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="516b3-127">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="516b3-128">示例</span><span class="sxs-lookup"><span data-stu-id="516b3-128">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="516b3-129">示例 1：获取默认品牌</span><span class="sxs-lookup"><span data-stu-id="516b3-129">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="516b3-130">如果尝试 Graph Explorer 中的示例，还必须包含具有有效 ISO-639 区域设置的 **Accept-Language** 请求标头，以避免收到错误"无效区域设置 id 值 *en-US，en;q=0.9"。它必须是有效的 ISO-639 区域设置。*</span><span class="sxs-lookup"><span data-stu-id="516b3-130">If you try the example in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale to avoid getting an error "*Invalid locale id value en-US,en;q=0.9. It must be a valid ISO-639 locale.*"</span></span>

#### <a name="request"></a><span data-ttu-id="516b3-131">请求</span><span class="sxs-lookup"><span data-stu-id="516b3-131">Request</span></span>

<span data-ttu-id="516b3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516b3-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="516b3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="516b3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="516b3-134">C#</span><span class="sxs-lookup"><span data-stu-id="516b3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="516b3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="516b3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="516b3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="516b3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="516b3-137">Java</span><span class="sxs-lookup"><span data-stu-id="516b3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="516b3-138">响应</span><span class="sxs-lookup"><span data-stu-id="516b3-138">Response</span></span>

<span data-ttu-id="516b3-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="516b3-139">The following is an example of the response.</span></span>

> <span data-ttu-id="516b3-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="516b3-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="516b3-141">对 /branding 的请求始终返回 **mediaContentType、mediaReadLink** 和 **mediaEditLink** 属性。 </span><span class="sxs-lookup"><span data-stu-id="516b3-141">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="516b3-142">如果已应用区域设置，**则 mediaEditLink** 为区域设置 (（始终为非 null) ）的 **mediaEditLink;** 如果区域设置的 **mediaReadLink** 为非 null，则 **mediaReadLink** 和 **mediaContentType** 为区域设置中的 **mediaReadLink** 和 **mediaContentType;** 否则，默认 **mediaReadLink** 和 **mediaContentType**。</span><span class="sxs-lookup"><span data-stu-id="516b3-142">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="516b3-143">示例 2：获取组织品牌，但没有配置品牌</span><span class="sxs-lookup"><span data-stu-id="516b3-143">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="516b3-144">请求</span><span class="sxs-lookup"><span data-stu-id="516b3-144">Request</span></span>

<span data-ttu-id="516b3-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516b3-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="516b3-146">响应</span><span class="sxs-lookup"><span data-stu-id="516b3-146">Response</span></span>

<span data-ttu-id="516b3-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="516b3-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="516b3-148">示例 3：获取法语区域设置的组织品牌</span><span class="sxs-lookup"><span data-stu-id="516b3-148">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="516b3-149">**Accept-Language** 标头用于将特定本地化应用到品牌。</span><span class="sxs-lookup"><span data-stu-id="516b3-149">The **Accept-Language** header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="516b3-150">指定 `null` 本地化中的属性从默认品牌返回。</span><span class="sxs-lookup"><span data-stu-id="516b3-150">Properties that are `null` in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="516b3-151">如果在 **请求中指定了 Accept-Language** 标头，则响应将包括 **Content-Language** 标头，除非是 `und` 。</span><span class="sxs-lookup"><span data-stu-id="516b3-151">If the **Accept-Language** header is specified in the request, the response will include the **Content-Language** header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="516b3-152">请求</span><span class="sxs-lookup"><span data-stu-id="516b3-152">Request</span></span>

<span data-ttu-id="516b3-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516b3-153">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="516b3-154">响应</span><span class="sxs-lookup"><span data-stu-id="516b3-154">Response</span></span>

<span data-ttu-id="516b3-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="516b3-155">The following is an example of the response.</span></span>

> <span data-ttu-id="516b3-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="516b3-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="516b3-157">示例 4：获取法语区域设置的 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="516b3-157">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="516b3-158">如果 **区域设置** 存在， `fr` 则返回 bannerLogo。</span><span class="sxs-lookup"><span data-stu-id="516b3-158">Returns **bannerLogo** for the `fr` locale if it exists.</span></span> <span data-ttu-id="516b3-159">如果本地化不存在，则返回默认的 **bannerLogo**。</span><span class="sxs-lookup"><span data-stu-id="516b3-159">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="516b3-160">请求</span><span class="sxs-lookup"><span data-stu-id="516b3-160">Request</span></span>

<span data-ttu-id="516b3-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516b3-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="516b3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="516b3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_5"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="516b3-163">C#</span><span class="sxs-lookup"><span data-stu-id="516b3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="516b3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="516b3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="516b3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="516b3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="516b3-166">Java</span><span class="sxs-lookup"><span data-stu-id="516b3-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="516b3-167">响应</span><span class="sxs-lookup"><span data-stu-id="516b3-167">Response</span></span>

<span data-ttu-id="516b3-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="516b3-168">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="516b3-169">示例 5：在未配置 bannerLogo 时获取 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="516b3-169">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="516b3-170">本示例显示对默认品牌或 **Accept-Language** 标头中指定的语言上不存在的属性的请求。</span><span class="sxs-lookup"><span data-stu-id="516b3-170">This example shows a request for a property that does not exist on the default branding or the language specified in the **Accept-Language** header.</span></span>

#### <a name="request"></a><span data-ttu-id="516b3-171">请求</span><span class="sxs-lookup"><span data-stu-id="516b3-171">Request</span></span>

<span data-ttu-id="516b3-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516b3-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="516b3-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="516b3-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_6"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```
# <a name="c"></a>[<span data-ttu-id="516b3-174">C#</span><span class="sxs-lookup"><span data-stu-id="516b3-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="516b3-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="516b3-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="516b3-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="516b3-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="516b3-177">Java</span><span class="sxs-lookup"><span data-stu-id="516b3-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="516b3-178">响应</span><span class="sxs-lookup"><span data-stu-id="516b3-178">Response</span></span>

<span data-ttu-id="516b3-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="516b3-179">The following is an example of the response.</span></span>

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
