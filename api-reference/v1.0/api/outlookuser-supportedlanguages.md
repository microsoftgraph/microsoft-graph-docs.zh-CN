---
title: 'outlookUser: supportedLanguages'
description: 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dfb094b07ff89457e885c1b24ae882e653a9bc73
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128286"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="4ec39-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="4ec39-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="4ec39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ec39-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ec39-105">获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。</span><span class="sxs-lookup"><span data-stu-id="4ec39-105">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="4ec39-106">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选语言。</span><span class="sxs-lookup"><span data-stu-id="4ec39-106">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="4ec39-107">随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选语言。</span><span class="sxs-lookup"><span data-stu-id="4ec39-107">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="4ec39-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ec39-108">Permissions</span></span>
<span data-ttu-id="4ec39-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ec39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ec39-111">Permission type</span></span>      | <span data-ttu-id="4ec39-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ec39-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ec39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec39-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4ec39-114">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4ec39-114">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="4ec39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec39-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ec39-116">User.Read</span><span class="sxs-lookup"><span data-stu-id="4ec39-116">User.Read</span></span>    |
|<span data-ttu-id="4ec39-117">Application</span><span class="sxs-lookup"><span data-stu-id="4ec39-117">Application</span></span> | <span data-ttu-id="4ec39-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ec39-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ec39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ec39-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="4ec39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ec39-120">Request headers</span></span>
| <span data-ttu-id="4ec39-121">名称</span><span class="sxs-lookup"><span data-stu-id="4ec39-121">Name</span></span>       | <span data-ttu-id="4ec39-122">类型</span><span class="sxs-lookup"><span data-stu-id="4ec39-122">Type</span></span> | <span data-ttu-id="4ec39-123">说明</span><span class="sxs-lookup"><span data-stu-id="4ec39-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ec39-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ec39-124">Authorization</span></span>  | <span data-ttu-id="4ec39-125">string</span><span class="sxs-lookup"><span data-stu-id="4ec39-125">string</span></span>  | <span data-ttu-id="4ec39-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ec39-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4ec39-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ec39-128">Request body</span></span>
<span data-ttu-id="4ec39-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ec39-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec39-130">响应</span><span class="sxs-lookup"><span data-stu-id="4ec39-130">Response</span></span>
<span data-ttu-id="4ec39-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [localeInfo](../resources/localeinfo.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4ec39-131">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ec39-132">示例</span><span class="sxs-lookup"><span data-stu-id="4ec39-132">Example</span></span>
<span data-ttu-id="4ec39-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4ec39-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ec39-134">请求</span><span class="sxs-lookup"><span data-stu-id="4ec39-134">Request</span></span>
<span data-ttu-id="4ec39-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ec39-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ec39-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec39-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```
# <a name="c"></a>[<span data-ttu-id="4ec39-137">C#</span><span class="sxs-lookup"><span data-stu-id="4ec39-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedlanguages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ec39-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ec39-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedlanguages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ec39-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ec39-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedlanguages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ec39-140">Java</span><span class="sxs-lookup"><span data-stu-id="4ec39-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedlanguages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ec39-141">响应</span><span class="sxs-lookup"><span data-stu-id="4ec39-141">Response</span></span>
<span data-ttu-id="4ec39-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ec39-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

