---
title: 获取 organizationalBrandingProperties
description: 检索 organizationalBrandingProperties 对象的属性和关系。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f46f6487fc067aaab780f06395f5ff2b5b682f80
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031910"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="ab93e-103">获取 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="ab93e-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab93e-104">检索 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab93e-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab93e-105">权限</span><span class="sxs-lookup"><span data-stu-id="ab93e-105">Permissions</span></span>

<span data-ttu-id="ab93e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab93e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab93e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab93e-108">Permission type</span></span>                        | <span data-ttu-id="ab93e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab93e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab93e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab93e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab93e-111">全部、User.readbasic.all、用户读取、全部、用户、全部。</span><span class="sxs-lookup"><span data-stu-id="ab93e-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="ab93e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab93e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab93e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab93e-113">Not supported.</span></span> |
| <span data-ttu-id="ab93e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab93e-114">Application</span></span>                            | <span data-ttu-id="ab93e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab93e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab93e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab93e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab93e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab93e-117">Optional query parameters</span></span>

<span data-ttu-id="ab93e-p102">此方法支持使用某些 OData 查询参数来帮助自定义响应。有关常规信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ab93e-p102">This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab93e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab93e-120">Request headers</span></span>

| <span data-ttu-id="ab93e-121">名称</span><span class="sxs-lookup"><span data-stu-id="ab93e-121">Name</span></span>      |<span data-ttu-id="ab93e-122">说明</span><span class="sxs-lookup"><span data-stu-id="ab93e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab93e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab93e-123">Authorization</span></span> | <span data-ttu-id="ab93e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab93e-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="ab93e-126">如果您在 Graph 浏览器中尝试查询，则还必须将 Accept-Language 请求标头包含在有效的 ISO-639 区域设置中。</span><span class="sxs-lookup"><span data-stu-id="ab93e-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="ab93e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab93e-127">Request body</span></span>

<span data-ttu-id="ab93e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab93e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab93e-129">响应</span><span class="sxs-lookup"><span data-stu-id="ab93e-129">Response</span></span>

<span data-ttu-id="ab93e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab93e-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab93e-131">示例</span><span class="sxs-lookup"><span data-stu-id="ab93e-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="ab93e-132">示例1：获取默认品牌</span><span class="sxs-lookup"><span data-stu-id="ab93e-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="ab93e-133">如果您尝试使用 Graph 浏览器中的示例，则还必须将 Accept-Language 请求标头包含在有效的 ISO-639 区域设置中，以避免出现错误 "无效的区域设置 id 值 en-us，en; q = 0.9."。</span><span class="sxs-lookup"><span data-stu-id="ab93e-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="ab93e-134">它必须是有效的 ISO-639 区域设置。</span><span class="sxs-lookup"><span data-stu-id="ab93e-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="ab93e-135">请求</span><span class="sxs-lookup"><span data-stu-id="ab93e-135">Request</span></span>

<span data-ttu-id="ab93e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab93e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="ab93e-137">响应</span><span class="sxs-lookup"><span data-stu-id="ab93e-137">Response</span></span>

<span data-ttu-id="ab93e-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab93e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ab93e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab93e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="ab93e-141">对/branding 的请求始终返回 **mediaContentType** 、 **mediaReadLink** 和 **mediaEditLink** 属性。</span><span class="sxs-lookup"><span data-stu-id="ab93e-141">Requests for /branding always return the **mediaContentType** , **mediaReadLink** , and **mediaEditLink** properties.</span></span> <span data-ttu-id="ab93e-142">如果已应用区域设置，则 **mediaEditLink** 是区域设置 (的 **mediaEditLink** ，它始终为非 null) ， **mediaReadLink** 和 **MediaContentType** 是区域 **设置的** mediaReadLink 和 mediaContentType **，如果** 区域设置为非 null，则为区域设置的 mediaReadLink 和 **mediaContentType** 。否则，默认的 **mediaReadLink** 和 **mediaContentType** 。</span><span class="sxs-lookup"><span data-stu-id="ab93e-142">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="ab93e-143">示例2：获取组织品牌，但不配置品牌</span><span class="sxs-lookup"><span data-stu-id="ab93e-143">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="ab93e-144">请求</span><span class="sxs-lookup"><span data-stu-id="ab93e-144">Request</span></span>

<span data-ttu-id="ab93e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab93e-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="ab93e-146">响应</span><span class="sxs-lookup"><span data-stu-id="ab93e-146">Response</span></span>

<span data-ttu-id="ab93e-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab93e-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="ab93e-148">示例3：获取法语区域设置的组织品牌</span><span class="sxs-lookup"><span data-stu-id="ab93e-148">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="ab93e-149">Accept-Langauge 标头用于将特定本地化应用于品牌。</span><span class="sxs-lookup"><span data-stu-id="ab93e-149">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="ab93e-150">在指定的本地化中，为 null 的属性将从默认品牌打造返回。</span><span class="sxs-lookup"><span data-stu-id="ab93e-150">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="ab93e-151">如果请求中指定了 Accept-Language 标头，则响应将包含内容语言标头，除非它是 `und` 。</span><span class="sxs-lookup"><span data-stu-id="ab93e-151">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="ab93e-152">请求</span><span class="sxs-lookup"><span data-stu-id="ab93e-152">Request</span></span>

<span data-ttu-id="ab93e-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab93e-153">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="ab93e-154">响应</span><span class="sxs-lookup"><span data-stu-id="ab93e-154">Response</span></span>

<span data-ttu-id="ab93e-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab93e-155">The following is an example of the response.</span></span>

> <span data-ttu-id="ab93e-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab93e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="ab93e-158">示例4：获取法语区域设置的 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="ab93e-158">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="ab93e-159">如果存在，则返回 fr-fr 区域设置的 **bannerLogo** 。</span><span class="sxs-lookup"><span data-stu-id="ab93e-159">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="ab93e-160">如果本地化不存在，则返回默认的 **bannerLogo** 。</span><span class="sxs-lookup"><span data-stu-id="ab93e-160">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="ab93e-161">请求</span><span class="sxs-lookup"><span data-stu-id="ab93e-161">Request</span></span>

<span data-ttu-id="ab93e-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab93e-162">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="ab93e-163">响应</span><span class="sxs-lookup"><span data-stu-id="ab93e-163">Response</span></span>

<span data-ttu-id="ab93e-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab93e-164">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="ab93e-165">示例5：在未配置 bannerLogo 时获取 bannerLogo</span><span class="sxs-lookup"><span data-stu-id="ab93e-165">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="ab93e-166">此示例演示在默认品牌或 Accept-Language 标头中指定的语言中不存在的属性的请求。</span><span class="sxs-lookup"><span data-stu-id="ab93e-166">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="ab93e-167">请求</span><span class="sxs-lookup"><span data-stu-id="ab93e-167">Request</span></span>

<span data-ttu-id="ab93e-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab93e-168">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="ab93e-169">响应</span><span class="sxs-lookup"><span data-stu-id="ab93e-169">Response</span></span>

<span data-ttu-id="ab93e-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab93e-170">The following is an example of the response.</span></span>

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
