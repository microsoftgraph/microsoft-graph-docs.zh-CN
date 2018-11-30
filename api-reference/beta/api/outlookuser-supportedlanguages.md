---
title: 'outlookUser: supportedLanguages'
description: 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。
ms.openlocfilehash: ac1b9693121f3ba3f180b53532bb6a6c917e2108
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041703"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="5d5d7-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="5d5d7-103">outlookUser: supportedLanguages</span></span>

> <span data-ttu-id="5d5d7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d5d7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d5d7-106">获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-106">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="5d5d7-107">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选语言。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-107">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="5d5d7-108">随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选语言。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-108">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="5d5d7-109">权限</span><span class="sxs-lookup"><span data-stu-id="5d5d7-109">Permissions</span></span>
<span data-ttu-id="5d5d7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d5d7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d5d7-112">Permission type</span></span>      | <span data-ttu-id="5d5d7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d5d7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d5d7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d5d7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5d5d7-115">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="5d5d7-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="5d5d7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d5d7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d5d7-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="5d5d7-117">User.Read</span></span>    |
|<span data-ttu-id="5d5d7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d5d7-118">Application</span></span> | <span data-ttu-id="5d5d7-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d5d7-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d5d7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d5d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="5d5d7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d5d7-121">Request headers</span></span>
| <span data-ttu-id="5d5d7-122">名称</span><span class="sxs-lookup"><span data-stu-id="5d5d7-122">Name</span></span>       | <span data-ttu-id="5d5d7-123">类型</span><span class="sxs-lookup"><span data-stu-id="5d5d7-123">Type</span></span> | <span data-ttu-id="5d5d7-124">说明</span><span class="sxs-lookup"><span data-stu-id="5d5d7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d5d7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d5d7-125">Authorization</span></span>  | <span data-ttu-id="5d5d7-126">string</span><span class="sxs-lookup"><span data-stu-id="5d5d7-126">string</span></span>  | <span data-ttu-id="5d5d7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5d5d7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d5d7-129">Request body</span></span>
<span data-ttu-id="5d5d7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d5d7-131">响应</span><span class="sxs-lookup"><span data-stu-id="5d5d7-131">Response</span></span>
<span data-ttu-id="5d5d7-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [localeInfo](../resources/localeinfo.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-132">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d5d7-133">示例</span><span class="sxs-lookup"><span data-stu-id="5d5d7-133">Example</span></span>
<span data-ttu-id="5d5d7-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d5d7-135">请求</span><span class="sxs-lookup"><span data-stu-id="5d5d7-135">Request</span></span>
<span data-ttu-id="5d5d7-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="5d5d7-137">响应</span><span class="sxs-lookup"><span data-stu-id="5d5d7-137">Response</span></span>
<span data-ttu-id="5d5d7-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-138">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.localeInfo)",
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
  "tocPath": ""
}-->