---
title: 获取 organizationalBrandingProperties
description: 检索 organizationalBrandingProperties 对象的属性和关系。
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 53f6ed90959c2559a18754bd4c5bd4bb25ca5210
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298234"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="66ec6-103">获取 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="66ec6-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ec6-104">检索 [organizationalBrandingProperties 对象的属性和](../resources/organizationalbrandingproperties.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="66ec6-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66ec6-105">权限</span><span class="sxs-lookup"><span data-stu-id="66ec6-105">Permissions</span></span>

<span data-ttu-id="66ec6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66ec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66ec6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="66ec6-108">Permission type</span></span>                        | <span data-ttu-id="66ec6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66ec6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66ec6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66ec6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="66ec6-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="66ec6-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="66ec6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66ec6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66ec6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="66ec6-113">Not supported.</span></span> |
| <span data-ttu-id="66ec6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="66ec6-114">Application</span></span>                            | <span data-ttu-id="66ec6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66ec6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66ec6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66ec6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{tenant id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66ec6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66ec6-117">Optional query parameters</span></span>

<span data-ttu-id="66ec6-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66ec6-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="66ec6-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="66ec6-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="66ec6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66ec6-120">Request headers</span></span>

| <span data-ttu-id="66ec6-121">名称</span><span class="sxs-lookup"><span data-stu-id="66ec6-121">Name</span></span>      |<span data-ttu-id="66ec6-122">说明</span><span class="sxs-lookup"><span data-stu-id="66ec6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66ec6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66ec6-123">Authorization</span></span> | <span data-ttu-id="66ec6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66ec6-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="66ec6-126">如果在资源管理器中尝试Graph，还必须包含具有有效 ISO-639 Accept-Language请求标头。</span><span class="sxs-lookup"><span data-stu-id="66ec6-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="66ec6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66ec6-127">Request body</span></span>

<span data-ttu-id="66ec6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66ec6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66ec6-129">响应</span><span class="sxs-lookup"><span data-stu-id="66ec6-129">Response</span></span>

<span data-ttu-id="66ec6-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66ec6-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66ec6-131">示例</span><span class="sxs-lookup"><span data-stu-id="66ec6-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="66ec6-132">示例 1：获取默认品牌</span><span class="sxs-lookup"><span data-stu-id="66ec6-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="66ec6-133">如果在 Graph 资源管理器中试用该示例，还必须包含具有有效 ISO-639 区域设置的 Accept-Language 请求标头，以避免收到错误"无效区域设置 id 值 en-US，en;q=0.9"。</span><span class="sxs-lookup"><span data-stu-id="66ec6-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="66ec6-134">它必须是有效的 ISO-639 区域设置。"</span><span class="sxs-lookup"><span data-stu-id="66ec6-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="66ec6-135">请求</span><span class="sxs-lookup"><span data-stu-id="66ec6-135">Request</span></span>

<span data-ttu-id="66ec6-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66ec6-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66ec6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="66ec6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="66ec6-138">C#</span><span class="sxs-lookup"><span data-stu-id="66ec6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66ec6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66ec6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66ec6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66ec6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66ec6-141">Java</span><span class="sxs-lookup"><span data-stu-id="66ec6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66ec6-142">响应</span><span class="sxs-lookup"><span data-stu-id="66ec6-142">Response</span></span>

<span data-ttu-id="66ec6-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66ec6-143">The following is an example of the response.</span></span>

> <span data-ttu-id="66ec6-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66ec6-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="66ec6-145">对 /branding 的请求始终返回 **mediaContentType、mediaReadLink** 和 **mediaEditLink** 属性。 </span><span class="sxs-lookup"><span data-stu-id="66ec6-145">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="66ec6-146">如果已应用区域设置，**则 mediaEditLink** 为区域设置 (（始终为非 null) ）的 **mediaEditLink;** 如果区域设置的 **mediaReadLink** 为非 null，则 **mediaReadLink** 和 **mediaContentType** 为区域设置中的 **mediaReadLink** 和 **mediaContentType;** 否则，默认 **mediaReadLink** 和 **mediaContentType**。</span><span class="sxs-lookup"><span data-stu-id="66ec6-146">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="66ec6-147">示例 2：获取组织品牌，但没有配置品牌</span><span class="sxs-lookup"><span data-stu-id="66ec6-147">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="66ec6-148">请求</span><span class="sxs-lookup"><span data-stu-id="66ec6-148">Request</span></span>

<span data-ttu-id="66ec6-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66ec6-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="66ec6-150">响应</span><span class="sxs-lookup"><span data-stu-id="66ec6-150">Response</span></span>

<span data-ttu-id="66ec6-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66ec6-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="66ec6-152">示例 3：获取法语区域设置的组织品牌</span><span class="sxs-lookup"><span data-stu-id="66ec6-152">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="66ec6-153">the Accept-Langauge header is used to apply a particular localization to the branding.</span><span class="sxs-lookup"><span data-stu-id="66ec6-153">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="66ec6-154">指定本地化中为 null 的属性从默认品牌返回。</span><span class="sxs-lookup"><span data-stu-id="66ec6-154">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="66ec6-155">如果在Accept-Language中指定了内容语言标头，响应将包含 Content-Language 标头，除非是 `und` 。</span><span class="sxs-lookup"><span data-stu-id="66ec6-155">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="66ec6-156">请求</span><span class="sxs-lookup"><span data-stu-id="66ec6-156">Request</span></span>

<span data-ttu-id="66ec6-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66ec6-157">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="66ec6-158">响应</span><span class="sxs-lookup"><span data-stu-id="66ec6-158">Response</span></span>

<span data-ttu-id="66ec6-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66ec6-159">The following is an example of the response.</span></span>

> <span data-ttu-id="66ec6-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66ec6-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="66ec6-161">示例 4：获取法语区域设置的 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="66ec6-161">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="66ec6-162">如果 fr 区域设置存在，则返回 **bannerLogo。**</span><span class="sxs-lookup"><span data-stu-id="66ec6-162">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="66ec6-163">如果本地化不存在，则返回默认的 **bannerLogo**。</span><span class="sxs-lookup"><span data-stu-id="66ec6-163">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="66ec6-164">请求</span><span class="sxs-lookup"><span data-stu-id="66ec6-164">Request</span></span>

<span data-ttu-id="66ec6-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66ec6-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66ec6-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="66ec6-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_5"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="66ec6-167">C#</span><span class="sxs-lookup"><span data-stu-id="66ec6-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66ec6-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66ec6-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66ec6-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66ec6-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66ec6-170">Java</span><span class="sxs-lookup"><span data-stu-id="66ec6-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66ec6-171">响应</span><span class="sxs-lookup"><span data-stu-id="66ec6-171">Response</span></span>

<span data-ttu-id="66ec6-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66ec6-172">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="66ec6-173">示例 5：在未配置 bannerLogo 时获取 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="66ec6-173">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="66ec6-174">本示例显示对默认品牌或页面标题中指定的语言中不存在Accept-Language的请求。</span><span class="sxs-lookup"><span data-stu-id="66ec6-174">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="66ec6-175">请求</span><span class="sxs-lookup"><span data-stu-id="66ec6-175">Request</span></span>

<span data-ttu-id="66ec6-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66ec6-176">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66ec6-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="66ec6-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_6"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```
# <a name="c"></a>[<span data-ttu-id="66ec6-178">C#</span><span class="sxs-lookup"><span data-stu-id="66ec6-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66ec6-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66ec6-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66ec6-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66ec6-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66ec6-181">Java</span><span class="sxs-lookup"><span data-stu-id="66ec6-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="66ec6-182">响应</span><span class="sxs-lookup"><span data-stu-id="66ec6-182">Response</span></span>

<span data-ttu-id="66ec6-183">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66ec6-183">The following is an example of the response.</span></span>

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
