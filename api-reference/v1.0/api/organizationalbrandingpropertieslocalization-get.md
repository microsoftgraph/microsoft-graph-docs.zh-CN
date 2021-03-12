---
title: 获取本地化的组织BrandingProperties
description: 检索特定区域设置的组织品牌属性对象。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 24ba0c96df393accfefa5930a60b9ca186819ac2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722533"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="7aad1-103">获取本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="7aad1-103">Get Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="7aad1-104">检索 [organizationalBrandingProperties 对象](../resources/organizationalbrandingproperties.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="7aad1-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aad1-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="7aad1-105">Permissions</span></span>

<span data-ttu-id="7aad1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7aad1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aad1-108">Permission type</span></span>                        | <span data-ttu-id="7aad1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7aad1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7aad1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aad1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aad1-111">Organization.Read.All、User.Read、User.Read.All、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="7aad1-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="7aad1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aad1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aad1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aad1-113">Not supported.</span></span> |
| <span data-ttu-id="7aad1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aad1-114">Application</span></span>                            | <span data-ttu-id="7aad1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aad1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aad1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aad1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="7aad1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aad1-117">Request headers</span></span>

| <span data-ttu-id="7aad1-118">名称</span><span class="sxs-lookup"><span data-stu-id="7aad1-118">Name</span></span>      |<span data-ttu-id="7aad1-119">说明</span><span class="sxs-lookup"><span data-stu-id="7aad1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7aad1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aad1-120">Authorization</span></span> | <span data-ttu-id="7aad1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7aad1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7aad1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aad1-123">Content-Type</span></span>  | <span data-ttu-id="7aad1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7aad1-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aad1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aad1-126">Request body</span></span>

<span data-ttu-id="7aad1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7aad1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aad1-128">响应</span><span class="sxs-lookup"><span data-stu-id="7aad1-128">Response</span></span>

<span data-ttu-id="7aad1-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7aad1-129">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="7aad1-130">"id"的值对应于请求的本地化。</span><span class="sxs-lookup"><span data-stu-id="7aad1-130">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="7aad1-131">示例</span><span class="sxs-lookup"><span data-stu-id="7aad1-131">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="7aad1-132">示例 1：获取特定区域设置或 (本地化) </span><span class="sxs-lookup"><span data-stu-id="7aad1-132">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="7aad1-133">对特定本地化的 GET 请求仅返回该本地化的值。</span><span class="sxs-lookup"><span data-stu-id="7aad1-133">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="7aad1-134">空值不会替换为默认品牌中的值。</span><span class="sxs-lookup"><span data-stu-id="7aad1-134">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="7aad1-135">请求</span><span class="sxs-lookup"><span data-stu-id="7aad1-135">Request</span></span>

<span data-ttu-id="7aad1-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7aad1-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

#### <a name="response"></a><span data-ttu-id="7aad1-137">响应</span><span class="sxs-lookup"><span data-stu-id="7aad1-137">Response</span></span>

<span data-ttu-id="7aad1-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7aad1-138">The following is an example of the response.</span></span>

> <span data-ttu-id="7aad1-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7aad1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="7aad1-141">示例 2：获取已配置的所有特定语言的本地化</span><span class="sxs-lookup"><span data-stu-id="7aad1-141">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="7aad1-142">请求</span><span class="sxs-lookup"><span data-stu-id="7aad1-142">Request</span></span>

<span data-ttu-id="7aad1-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7aad1-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```

#### <a name="response"></a><span data-ttu-id="7aad1-144">响应</span><span class="sxs-lookup"><span data-stu-id="7aad1-144">Response</span></span>

<span data-ttu-id="7aad1-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7aad1-145">The following is an example of the response.</span></span>

> <span data-ttu-id="7aad1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7aad1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="7aad1-148">示例 3：获取特定区域设置 signInPageText 的值</span><span class="sxs-lookup"><span data-stu-id="7aad1-148">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="7aad1-149">请求本地化的属性将返回该值，如果值为 null，则返回 204。</span><span class="sxs-lookup"><span data-stu-id="7aad1-149">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="7aad1-150">请求</span><span class="sxs-lookup"><span data-stu-id="7aad1-150">Request</span></span>

<span data-ttu-id="7aad1-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7aad1-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```

#### <a name="response"></a><span data-ttu-id="7aad1-152">响应</span><span class="sxs-lookup"><span data-stu-id="7aad1-152">Response</span></span>

<span data-ttu-id="7aad1-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7aad1-153">The following is an example of the response.</span></span>

> <span data-ttu-id="7aad1-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7aad1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
