---
title: 获取 regionalAndLanguageSettings 资源
description: 检索用户的 regionalAndLanguageSettings 的属性
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: a78c2f22e6e08ea7dc4709fbf3eaaaa8a5c1d5bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050365"
---
# <a name="get-regionalandlanguagesettings"></a><span data-ttu-id="d16a1-103">获取 regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="d16a1-103">Get regionalAndLanguageSettings</span></span>

<span data-ttu-id="d16a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d16a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d16a1-105">获取 [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d16a1-105">Get the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d16a1-106">权限</span><span class="sxs-lookup"><span data-stu-id="d16a1-106">Permissions</span></span>
<span data-ttu-id="d16a1-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d16a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d16a1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d16a1-109">Permission Type</span></span>                   |<span data-ttu-id="d16a1-110">从至少到最高特权的) 的权限 (</span><span class="sxs-lookup"><span data-stu-id="d16a1-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="d16a1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d16a1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d16a1-112">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="d16a1-112">User.Read, User.Read.All</span></span>                        |
|<span data-ttu-id="d16a1-113">委派 (个人帐户) </span><span class="sxs-lookup"><span data-stu-id="d16a1-113">Delegated (personal account)</span></span>      |<span data-ttu-id="d16a1-114">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="d16a1-114">User.Read, User.Read.All</span></span>              |
|<span data-ttu-id="d16a1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d16a1-115">Application</span></span>                       |<span data-ttu-id="d16a1-116">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="d16a1-116">User.Read, User.Read.All</span></span>              |

## <a name="http-request"></a><span data-ttu-id="d16a1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d16a1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d16a1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d16a1-118">Optional query parameters</span></span>
<span data-ttu-id="d16a1-119">您可以使用 `$select` 获取特定的 regionalAndLanguageSettings 属性，包括默认情况下不返回的属性。</span><span class="sxs-lookup"><span data-stu-id="d16a1-119">You can use `$select` to get specific regionalAndLanguageSettings properties, including those that are not returned by default.</span></span>

<span data-ttu-id="d16a1-120">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d16a1-120">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d16a1-121">请求头</span><span class="sxs-lookup"><span data-stu-id="d16a1-121">Request headers</span></span>
| <span data-ttu-id="d16a1-122">标头</span><span class="sxs-lookup"><span data-stu-id="d16a1-122">Header</span></span>       | <span data-ttu-id="d16a1-123">值</span><span class="sxs-lookup"><span data-stu-id="d16a1-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d16a1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d16a1-124">Authorization</span></span>  | <span data-ttu-id="d16a1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d16a1-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d16a1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d16a1-127">Content-Type</span></span>   | <span data-ttu-id="d16a1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d16a1-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d16a1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d16a1-129">Request body</span></span>
<span data-ttu-id="d16a1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d16a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d16a1-131">响应</span><span class="sxs-lookup"><span data-stu-id="d16a1-131">Response</span></span>

<span data-ttu-id="d16a1-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d16a1-132">If successful, this method returns a `200 OK` response code and [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d16a1-133">示例</span><span class="sxs-lookup"><span data-stu-id="d16a1-133">Example</span></span>

<span data-ttu-id="d16a1-134">下面的示例获取已登录用户的属性。</span><span class="sxs-lookup"><span data-stu-id="d16a1-134">The following example gets the properties of the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="d16a1-135">请求</span><span class="sxs-lookup"><span data-stu-id="d16a1-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d16a1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d16a1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```
# <a name="c"></a>[<span data-ttu-id="d16a1-137">C#</span><span class="sxs-lookup"><span data-stu-id="d16a1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d16a1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d16a1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d16a1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d16a1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d16a1-140">响应</span><span class="sxs-lookup"><span data-stu-id="d16a1-140">Response</span></span>

><span data-ttu-id="d16a1-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d16a1-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "get_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR",
            "displayName": "French (France)"
        },
        {
            "locale": "de-DE",
            "displayName": "German (Germany)"
        },
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB",
        "displayName": "English (United Kingdom)"
    },
    "regionalFormatOverrides": {
        "calendar": "Gregorian Calendar",
        "firstDayOfWeek": "Sunday",
        "shortDateFormat": "yyyy-MM-dd",
        "longDateFormat": "dddd, MMMM d, yyyy",
        "shortTimeFormat": "HH:mm",
        "longTimeFormat": "h:mm:ss tt",
        "timeZone": "Pacific Standard Time"
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


