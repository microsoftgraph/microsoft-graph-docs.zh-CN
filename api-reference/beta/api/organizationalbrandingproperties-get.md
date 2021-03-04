---
title: 获取 organizationalBrandingProperties
description: 检索 organizationalBrandingProperties 对象的属性和关系。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3e0d5b77b3420e6019a61b7f3545a4e333dfad58
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434097"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="53635-103">获取 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="53635-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53635-104">检索 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53635-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53635-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="53635-105">Permissions</span></span>

<span data-ttu-id="53635-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53635-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53635-108">Permission type</span></span>                        | <span data-ttu-id="53635-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53635-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53635-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53635-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53635-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="53635-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="53635-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53635-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53635-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="53635-113">Not supported.</span></span> |
| <span data-ttu-id="53635-114">Application</span><span class="sxs-lookup"><span data-stu-id="53635-114">Application</span></span>                            | <span data-ttu-id="53635-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53635-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53635-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53635-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53635-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53635-117">Optional query parameters</span></span>

<span data-ttu-id="53635-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53635-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="53635-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="53635-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="53635-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53635-120">Request headers</span></span>

| <span data-ttu-id="53635-121">名称</span><span class="sxs-lookup"><span data-stu-id="53635-121">Name</span></span>      |<span data-ttu-id="53635-122">说明</span><span class="sxs-lookup"><span data-stu-id="53635-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53635-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53635-123">Authorization</span></span> | <span data-ttu-id="53635-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53635-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="53635-126">如果在 Graph 资源管理器中尝试查询，还必须包含具有有效 ISO-639 Accept-Language请求标头。</span><span class="sxs-lookup"><span data-stu-id="53635-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="53635-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53635-127">Request body</span></span>

<span data-ttu-id="53635-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53635-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53635-129">响应</span><span class="sxs-lookup"><span data-stu-id="53635-129">Response</span></span>

<span data-ttu-id="53635-130">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53635-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53635-131">示例</span><span class="sxs-lookup"><span data-stu-id="53635-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="53635-132">示例 1：获取默认品牌</span><span class="sxs-lookup"><span data-stu-id="53635-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="53635-133">如果在 Graph 资源管理器中试用该示例，还必须包含具有有效 ISO-639 区域设置的 Accept-Language 请求标头，以避免出现错误"无效区域设置 id 值 en-US，en;q=0.9"。</span><span class="sxs-lookup"><span data-stu-id="53635-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="53635-134">它必须是有效的 ISO-639 区域设置。"</span><span class="sxs-lookup"><span data-stu-id="53635-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="53635-135">请求</span><span class="sxs-lookup"><span data-stu-id="53635-135">Request</span></span>

<span data-ttu-id="53635-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53635-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53635-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="53635-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="53635-138">C#</span><span class="sxs-lookup"><span data-stu-id="53635-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53635-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53635-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53635-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53635-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53635-141">Java</span><span class="sxs-lookup"><span data-stu-id="53635-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="53635-142">响应</span><span class="sxs-lookup"><span data-stu-id="53635-142">Response</span></span>

<span data-ttu-id="53635-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53635-143">The following is an example of the response.</span></span>

> <span data-ttu-id="53635-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53635-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "bannerLogo@odata.mediaContentType":"image/*",
  "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "id": "und",
  "squareLogo@odata.mediaContentType":"image/*",
  "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "signInPageText":"Default",
  "usernameHintText":"DefaultHint"
}
```

<span data-ttu-id="53635-146">/branding 请求始终返回 **mediaContentType、mediaReadLink** 和 **mediaEditLink** 属性。</span><span class="sxs-lookup"><span data-stu-id="53635-146">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="53635-147">如果已应用区域设置，**则 mediaEditLink** 是区域设置 (的 **mediaEditLink，** 它始终为非 null) ;如果区域设置的 **mediaReadLink** 为非 null，则 **mediaReadLink** 和 **mediaContentType** 为区域设置的 **mediaReadLink** 和 **mediaContentType;** 否则为默认的 **mediaReadLink** 和 **mediaContentType。**</span><span class="sxs-lookup"><span data-stu-id="53635-147">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="53635-148">示例 2：获取组织品牌，但没有配置品牌</span><span class="sxs-lookup"><span data-stu-id="53635-148">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="53635-149">请求</span><span class="sxs-lookup"><span data-stu-id="53635-149">Request</span></span>

<span data-ttu-id="53635-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53635-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="53635-151">响应</span><span class="sxs-lookup"><span data-stu-id="53635-151">Response</span></span>

<span data-ttu-id="53635-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53635-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="53635-153">示例 3：获取法语区域设置的组织品牌</span><span class="sxs-lookup"><span data-stu-id="53635-153">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="53635-154">the Accept-Langauge header is used to apply a particular localization to the branding.</span><span class="sxs-lookup"><span data-stu-id="53635-154">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="53635-155">指定本地化中为 null 的属性从默认品牌中返回。</span><span class="sxs-lookup"><span data-stu-id="53635-155">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="53635-156">如果在Accept-Language中指定了该标头，则响应将包含 Content-Language 标头，除非它是 `und` 。</span><span class="sxs-lookup"><span data-stu-id="53635-156">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="53635-157">请求</span><span class="sxs-lookup"><span data-stu-id="53635-157">Request</span></span>

<span data-ttu-id="53635-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53635-158">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="53635-159">响应</span><span class="sxs-lookup"><span data-stu-id="53635-159">Response</span></span>

<span data-ttu-id="53635-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53635-160">The following is an example of the response.</span></span>

> <span data-ttu-id="53635-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53635-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "und",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="53635-163">示例 4：获取法语区域设置横幅Logo</span><span class="sxs-lookup"><span data-stu-id="53635-163">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="53635-164">返回 fr 区域设置（如果存在）的 **bannerLogo。**</span><span class="sxs-lookup"><span data-stu-id="53635-164">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="53635-165">如果本地化不存在，则返回默认的 **bannerLogo**。</span><span class="sxs-lookup"><span data-stu-id="53635-165">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="53635-166">请求</span><span class="sxs-lookup"><span data-stu-id="53635-166">Request</span></span>

<span data-ttu-id="53635-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53635-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53635-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="53635-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="53635-169">C#</span><span class="sxs-lookup"><span data-stu-id="53635-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53635-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53635-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53635-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53635-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53635-172">Java</span><span class="sxs-lookup"><span data-stu-id="53635-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="53635-173">响应</span><span class="sxs-lookup"><span data-stu-id="53635-173">Response</span></span>

<span data-ttu-id="53635-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53635-174">The following is an example of the response.</span></span>

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
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
}
```

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="53635-175">示例 5：在未配置横幅Logo 时获取 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="53635-175">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="53635-176">本示例显示对默认品牌设置或页眉中指定的语言上不存在Accept-Language的请求。</span><span class="sxs-lookup"><span data-stu-id="53635-176">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="53635-177">请求</span><span class="sxs-lookup"><span data-stu-id="53635-177">Request</span></span>

<span data-ttu-id="53635-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53635-178">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="53635-179">响应</span><span class="sxs-lookup"><span data-stu-id="53635-179">Response</span></span>

<span data-ttu-id="53635-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53635-180">The following is an example of the response.</span></span>

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
