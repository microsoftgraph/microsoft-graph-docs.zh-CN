---
title: 获取本地化的 organizationalBrandingProperties
description: 检索特定区域设置的 organizationalbrandingproperties 对象。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75ba4f8ef3202f95d7538ef6017d01e005db60c9
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031906"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="ba00a-103">获取本地化的 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="ba00a-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba00a-104">检索 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ba00a-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba00a-105">权限</span><span class="sxs-lookup"><span data-stu-id="ba00a-105">Permissions</span></span>

<span data-ttu-id="ba00a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba00a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba00a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba00a-108">Permission type</span></span>                        | <span data-ttu-id="ba00a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba00a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba00a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba00a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba00a-111">全部、User.readbasic.all、用户读取、全部、用户、全部。</span><span class="sxs-lookup"><span data-stu-id="ba00a-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="ba00a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba00a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba00a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba00a-113">Not supported.</span></span> |
| <span data-ttu-id="ba00a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba00a-114">Application</span></span>                            | <span data-ttu-id="ba00a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba00a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba00a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba00a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba00a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba00a-117">Optional query parameters</span></span>

<span data-ttu-id="ba00a-p102">此方法支持使用某些 OData 查询参数来帮助自定义响应。有关常规信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ba00a-p102">This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba00a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba00a-120">Request headers</span></span>

| <span data-ttu-id="ba00a-121">名称</span><span class="sxs-lookup"><span data-stu-id="ba00a-121">Name</span></span>      |<span data-ttu-id="ba00a-122">说明</span><span class="sxs-lookup"><span data-stu-id="ba00a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba00a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba00a-123">Authorization</span></span> | <span data-ttu-id="ba00a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba00a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba00a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba00a-126">Content-Type</span></span>  | <span data-ttu-id="ba00a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ba00a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba00a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba00a-129">Request body</span></span>

<span data-ttu-id="ba00a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba00a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba00a-131">响应</span><span class="sxs-lookup"><span data-stu-id="ba00a-131">Response</span></span>

<span data-ttu-id="ba00a-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba00a-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="ba00a-133">"Id" 的值与请求的本地化对应。</span><span class="sxs-lookup"><span data-stu-id="ba00a-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="ba00a-134">示例</span><span class="sxs-lookup"><span data-stu-id="ba00a-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="ba00a-135">示例1：获取特定区域设置的本地化品牌 (fr) </span><span class="sxs-lookup"><span data-stu-id="ba00a-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="ba00a-136">对特定本地化的 GET 请求仅返回该本地化的值。</span><span class="sxs-lookup"><span data-stu-id="ba00a-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="ba00a-137">Null 值不会替换为默认署名中的值。</span><span class="sxs-lookup"><span data-stu-id="ba00a-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="ba00a-138">请求</span><span class="sxs-lookup"><span data-stu-id="ba00a-138">Request</span></span>

<span data-ttu-id="ba00a-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba00a-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

#### <a name="response"></a><span data-ttu-id="ba00a-140">响应</span><span class="sxs-lookup"><span data-stu-id="ba00a-140">Response</span></span>

<span data-ttu-id="ba00a-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba00a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ba00a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba00a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="ba00a-144">示例2：获取已配置的所有特定于语言的 localizations</span><span class="sxs-lookup"><span data-stu-id="ba00a-144">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="ba00a-145">请求</span><span class="sxs-lookup"><span data-stu-id="ba00a-145">Request</span></span>

<span data-ttu-id="ba00a-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba00a-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```

#### <a name="response"></a><span data-ttu-id="ba00a-147">响应</span><span class="sxs-lookup"><span data-stu-id="ba00a-147">Response</span></span>

<span data-ttu-id="ba00a-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba00a-148">The following is an example of the response.</span></span>

> <span data-ttu-id="ba00a-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba00a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="ba00a-151">示例3：获取特定区域设置的 signInPageText 的值</span><span class="sxs-lookup"><span data-stu-id="ba00a-151">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="ba00a-152">请求本地化的属性返回该值，如果值为 null，则返回204。</span><span class="sxs-lookup"><span data-stu-id="ba00a-152">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="ba00a-153">请求</span><span class="sxs-lookup"><span data-stu-id="ba00a-153">Request</span></span>

<span data-ttu-id="ba00a-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba00a-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```

#### <a name="response"></a><span data-ttu-id="ba00a-155">响应</span><span class="sxs-lookup"><span data-stu-id="ba00a-155">Response</span></span>

<span data-ttu-id="ba00a-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba00a-156">The following is an example of the response.</span></span>

> <span data-ttu-id="ba00a-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba00a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
