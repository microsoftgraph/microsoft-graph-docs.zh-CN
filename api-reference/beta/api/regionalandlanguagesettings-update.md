---
title: 更新 regionalAndLanguageSettings
description: 更新用户的区域和语言设置
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: c84023c281dcda00db756a80f5d14668d213e727
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744210"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="a80ac-103">更新 regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="a80ac-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="a80ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a80ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a80ac-105">更新[regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md)对象的部分或全部属性。</span><span class="sxs-lookup"><span data-stu-id="a80ac-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a80ac-106">权限</span><span class="sxs-lookup"><span data-stu-id="a80ac-106">Permissions</span></span>
<span data-ttu-id="a80ac-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a80ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a80ac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a80ac-109">Permission Type</span></span>                   |<span data-ttu-id="a80ac-110">权限（从至少到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a80ac-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="a80ac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a80ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a80ac-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a80ac-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="a80ac-113">委派（个人帐户）</span><span class="sxs-lookup"><span data-stu-id="a80ac-113">Delegated (personal account)</span></span>      |<span data-ttu-id="a80ac-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a80ac-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="a80ac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a80ac-115">Application</span></span>                       |<span data-ttu-id="a80ac-116">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a80ac-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="a80ac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a80ac-117">HTTP request</span></span>

<span data-ttu-id="a80ac-118">若要更新用户的所有区域和语言设置，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a80ac-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="a80ac-119">若要更新用户区域和语言设置的属性子集，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a80ac-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="a80ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a80ac-120">Request headers</span></span>
| <span data-ttu-id="a80ac-121">标头</span><span class="sxs-lookup"><span data-stu-id="a80ac-121">Header</span></span>       | <span data-ttu-id="a80ac-122">值</span><span class="sxs-lookup"><span data-stu-id="a80ac-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a80ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a80ac-123">Authorization</span></span>  | <span data-ttu-id="a80ac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a80ac-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a80ac-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a80ac-126">Content-Type</span></span>  | <span data-ttu-id="a80ac-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a80ac-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a80ac-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a80ac-129">Request body</span></span>
 <span data-ttu-id="a80ac-130">**PUT**：在请求正文中，提供一个[regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a80ac-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="a80ac-131">**PATCH**：仅提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a80ac-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a80ac-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a80ac-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a80ac-133">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="a80ac-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="a80ac-134">响应</span><span class="sxs-lookup"><span data-stu-id="a80ac-134">Response</span></span>

<span data-ttu-id="a80ac-135">如果成功，此方法将返回一个200响应代码和更新的 regionalAndLanguageSettings 对象</span><span class="sxs-lookup"><span data-stu-id="a80ac-135">If successful, this method returns a 200 response code and the updated regionalAndLanguageSettings object</span></span>

## <a name="example"></a><span data-ttu-id="a80ac-136">示例</span><span class="sxs-lookup"><span data-stu-id="a80ac-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="a80ac-137">示例1：更新已登录用户的整个 regionalAndLanguageSettings 对象</span><span class="sxs-lookup"><span data-stu-id="a80ac-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="a80ac-138">请求</span><span class="sxs-lookup"><span data-stu-id="a80ac-138">Request</span></span>

<span data-ttu-id="a80ac-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a80ac-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a80ac-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a80ac-140">HTTP</span></span>](#tab/http)
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
    }
}
```

---

#### <a name="response"></a><span data-ttu-id="a80ac-141">响应</span><span class="sxs-lookup"><span data-stu-id="a80ac-141">Response</span></span>

<span data-ttu-id="a80ac-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a80ac-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="a80ac-143">示例2：更新已登录用户的选定属性</span><span class="sxs-lookup"><span data-stu-id="a80ac-143">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="a80ac-144">请求</span><span class="sxs-lookup"><span data-stu-id="a80ac-144">Request</span></span>

<span data-ttu-id="a80ac-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a80ac-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a80ac-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a80ac-146">HTTP</span></span>](#tab/http)
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

---

#### <a name="response"></a><span data-ttu-id="a80ac-147">响应</span><span class="sxs-lookup"><span data-stu-id="a80ac-147">Response</span></span>

<span data-ttu-id="a80ac-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a80ac-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
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
