---
title: 更新 regionalAndLanguageSettings
description: 更新用户的区域和语言设置。
author: jasonbro
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: fb1621d05daa04a3387d728dfdfbea073cf56704
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787504"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="4d53e-103">更新 regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="4d53e-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="4d53e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d53e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d53e-105">更新 [regionalAndLanguageSettings 对象的部分或所有](../resources/regionalAndLanguageSettings.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="4d53e-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d53e-106">权限</span><span class="sxs-lookup"><span data-stu-id="4d53e-106">Permissions</span></span>
<span data-ttu-id="4d53e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d53e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d53e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d53e-109">Permission Type</span></span>                   |<span data-ttu-id="4d53e-110">权限 (权限级别从最低到最多) </span><span class="sxs-lookup"><span data-stu-id="4d53e-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="4d53e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d53e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d53e-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d53e-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="4d53e-113">委派 (个人帐户) </span><span class="sxs-lookup"><span data-stu-id="4d53e-113">Delegated (personal account)</span></span>      |<span data-ttu-id="4d53e-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d53e-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="4d53e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d53e-115">Application</span></span>                       |<span data-ttu-id="4d53e-116">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d53e-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="4d53e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d53e-117">HTTP request</span></span>

<span data-ttu-id="4d53e-118">更新用户的所有区域和语言设置：</span><span class="sxs-lookup"><span data-stu-id="4d53e-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="4d53e-119">若要更新用户区域和语言设置的属性子集，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4d53e-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="4d53e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d53e-120">Request headers</span></span>
| <span data-ttu-id="4d53e-121">标头</span><span class="sxs-lookup"><span data-stu-id="4d53e-121">Header</span></span>       | <span data-ttu-id="4d53e-122">值</span><span class="sxs-lookup"><span data-stu-id="4d53e-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4d53e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d53e-123">Authorization</span></span>  | <span data-ttu-id="4d53e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d53e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4d53e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d53e-126">Content-Type</span></span>  | <span data-ttu-id="4d53e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4d53e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d53e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d53e-129">Request body</span></span>
 <span data-ttu-id="4d53e-130">**PUT**：在请求正文中，提供 [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d53e-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="4d53e-131">**PATCH：** 仅提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4d53e-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4d53e-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4d53e-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4d53e-133">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="4d53e-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="4d53e-134">响应</span><span class="sxs-lookup"><span data-stu-id="4d53e-134">Response</span></span>

<span data-ttu-id="4d53e-135">如果成功，此方法返回 200 响应代码和更新的 **regionalAndLanguageSettings** 对象。</span><span class="sxs-lookup"><span data-stu-id="4d53e-135">If successful, this method returns a 200 response code and the updated **regionalAndLanguageSettings** object.</span></span>

## <a name="example"></a><span data-ttu-id="4d53e-136">示例</span><span class="sxs-lookup"><span data-stu-id="4d53e-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="4d53e-137">示例 1：更新已登录用户的整个 regionalAndLanguageSettings 对象</span><span class="sxs-lookup"><span data-stu-id="4d53e-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="4d53e-138">请求</span><span class="sxs-lookup"><span data-stu-id="4d53e-138">Request</span></span>

<span data-ttu-id="4d53e-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d53e-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d53e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d53e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_regionalAndLanguageSettings"
}-->
```http
PUT https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR"
        },
        {
            "locale": "de-DE"
        }
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB"
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
        ]
     }
}
```
# <a name="c"></a>[<span data-ttu-id="4d53e-141">C#</span><span class="sxs-lookup"><span data-stu-id="4d53e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d53e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d53e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d53e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d53e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d53e-144">Java</span><span class="sxs-lookup"><span data-stu-id="4d53e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="4d53e-145">响应</span><span class="sxs-lookup"><span data-stu-id="4d53e-145">Response</span></span>

<span data-ttu-id="4d53e-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d53e-146">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="4d53e-147">示例 2：更新已登录用户的选定属性</span><span class="sxs-lookup"><span data-stu-id="4d53e-147">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="4d53e-148">请求</span><span class="sxs-lookup"><span data-stu-id="4d53e-148">Request</span></span>

<span data-ttu-id="4d53e-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d53e-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d53e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d53e-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_regionalAndLanguageSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
  "authoringLanguages": [
    {
     "locale": "en-US" },
    {
     "locale": "es-MX" }
  ],
  "defaultRegionalFormat": {
     "locale": "en-US"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="4d53e-151">C#</span><span class="sxs-lookup"><span data-stu-id="4d53e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d53e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d53e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d53e-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d53e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d53e-154">Java</span><span class="sxs-lookup"><span data-stu-id="4d53e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="4d53e-155">响应</span><span class="sxs-lookup"><span data-stu-id="4d53e-155">Response</span></span>

<span data-ttu-id="4d53e-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d53e-156">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "patch_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


