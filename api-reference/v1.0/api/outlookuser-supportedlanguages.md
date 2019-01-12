---
title: 'outlookUser: supportedLanguages'
description: 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 78d459ed423a1942d438c6efdedf2eec7a8ff28c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962224"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="6301b-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="6301b-103">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="6301b-104">获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。</span><span class="sxs-lookup"><span data-stu-id="6301b-104">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="6301b-105">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选语言。</span><span class="sxs-lookup"><span data-stu-id="6301b-105">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="6301b-106">随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选语言。</span><span class="sxs-lookup"><span data-stu-id="6301b-106">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="6301b-107">权限</span><span class="sxs-lookup"><span data-stu-id="6301b-107">Permissions</span></span>
<span data-ttu-id="6301b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6301b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6301b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6301b-110">Permission type</span></span>      | <span data-ttu-id="6301b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6301b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6301b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6301b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6301b-113">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6301b-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="6301b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6301b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6301b-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="6301b-115">User.Read</span></span>    |
|<span data-ttu-id="6301b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6301b-116">Application</span></span> | <span data-ttu-id="6301b-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6301b-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6301b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6301b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="6301b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6301b-119">Request headers</span></span>
| <span data-ttu-id="6301b-120">名称</span><span class="sxs-lookup"><span data-stu-id="6301b-120">Name</span></span>       | <span data-ttu-id="6301b-121">类型</span><span class="sxs-lookup"><span data-stu-id="6301b-121">Type</span></span> | <span data-ttu-id="6301b-122">说明</span><span class="sxs-lookup"><span data-stu-id="6301b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6301b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6301b-123">Authorization</span></span>  | <span data-ttu-id="6301b-124">string</span><span class="sxs-lookup"><span data-stu-id="6301b-124">string</span></span>  | <span data-ttu-id="6301b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6301b-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6301b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6301b-127">Request body</span></span>
<span data-ttu-id="6301b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6301b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6301b-129">响应</span><span class="sxs-lookup"><span data-stu-id="6301b-129">Response</span></span>
<span data-ttu-id="6301b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [localeInfo](../resources/localeinfo.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="6301b-130">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6301b-131">示例</span><span class="sxs-lookup"><span data-stu-id="6301b-131">Example</span></span>
<span data-ttu-id="6301b-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6301b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6301b-133">请求</span><span class="sxs-lookup"><span data-stu-id="6301b-133">Request</span></span>
<span data-ttu-id="6301b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6301b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="6301b-135">响应</span><span class="sxs-lookup"><span data-stu-id="6301b-135">Response</span></span>
<span data-ttu-id="6301b-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6301b-136">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
