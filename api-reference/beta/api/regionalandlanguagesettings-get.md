---
title: 获取 regionalAndLanguageSettings 资源
description: 检索用户的区域AndLanguageSettings 的属性
author: jasonbro
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 6bd4f758a2e7b0113ba6da5eb04b1823171986b8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516631"
---
# <a name="get-regionalandlanguagesettings"></a><span data-ttu-id="630ba-103">获取 regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="630ba-103">Get regionalAndLanguageSettings</span></span>

<span data-ttu-id="630ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="630ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="630ba-105">获取 [regionalAndLanguageSettings 对象](../resources/regionalAndLanguageSettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="630ba-105">Get the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="630ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="630ba-106">Permissions</span></span>
<span data-ttu-id="630ba-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="630ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="630ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="630ba-109">Permission Type</span></span>                   |<span data-ttu-id="630ba-110">权限 (从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="630ba-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="630ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="630ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="630ba-112">User.Read、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="630ba-112">User.Read, User.Read.All</span></span>                        |
|<span data-ttu-id="630ba-113">委派 (个人帐户) </span><span class="sxs-lookup"><span data-stu-id="630ba-113">Delegated (personal account)</span></span>      |<span data-ttu-id="630ba-114">User.Read、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="630ba-114">User.Read, User.Read.All</span></span>              |
|<span data-ttu-id="630ba-115">Application</span><span class="sxs-lookup"><span data-stu-id="630ba-115">Application</span></span>                       |<span data-ttu-id="630ba-116">User.Read、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="630ba-116">User.Read, User.Read.All</span></span>              |

## <a name="http-request"></a><span data-ttu-id="630ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="630ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="630ba-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="630ba-118">Optional query parameters</span></span>
<span data-ttu-id="630ba-119">可用于获取 `$select` 特定的 regionalAndLanguageSettings 属性，包括默认情况下未返回的属性。</span><span class="sxs-lookup"><span data-stu-id="630ba-119">You can use `$select` to get specific regionalAndLanguageSettings properties, including those that are not returned by default.</span></span>

<span data-ttu-id="630ba-120">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="630ba-120">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="630ba-121">请求头</span><span class="sxs-lookup"><span data-stu-id="630ba-121">Request headers</span></span>
| <span data-ttu-id="630ba-122">标头</span><span class="sxs-lookup"><span data-stu-id="630ba-122">Header</span></span>       | <span data-ttu-id="630ba-123">值</span><span class="sxs-lookup"><span data-stu-id="630ba-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="630ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="630ba-124">Authorization</span></span>  | <span data-ttu-id="630ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="630ba-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="630ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="630ba-127">Request body</span></span>
<span data-ttu-id="630ba-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="630ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="630ba-129">响应</span><span class="sxs-lookup"><span data-stu-id="630ba-129">Response</span></span>

<span data-ttu-id="630ba-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="630ba-130">If successful, this method returns a `200 OK` response code and [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="630ba-131">示例</span><span class="sxs-lookup"><span data-stu-id="630ba-131">Example</span></span>

<span data-ttu-id="630ba-132">以下示例获取已登录用户的属性。</span><span class="sxs-lookup"><span data-stu-id="630ba-132">The following example gets the properties of the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="630ba-133">请求</span><span class="sxs-lookup"><span data-stu-id="630ba-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="630ba-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="630ba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```
# <a name="c"></a>[<span data-ttu-id="630ba-135">C#</span><span class="sxs-lookup"><span data-stu-id="630ba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="630ba-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="630ba-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="630ba-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="630ba-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="630ba-138">Java</span><span class="sxs-lookup"><span data-stu-id="630ba-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="630ba-139">响应</span><span class="sxs-lookup"><span data-stu-id="630ba-139">Response</span></span>

><span data-ttu-id="630ba-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="630ba-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    },
    "translationPreferences": {
        "translationBehavior": "Yes",
        "languageOverrides": [
            {
                "languageTag": "fr",
                "translationBehavior": "Yes" 
            }
        ],
        "untranslatedLanguages": ["de"]
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


