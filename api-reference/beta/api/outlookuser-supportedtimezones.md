---
title: 'outlookUser: supportedTimeZones'
description: 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4fe5c0b66a6c5b1a4574a0bfeb578808195fe38b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269130"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="f68d9-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="f68d9-103">outlookUser: supportedTimeZones</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f68d9-104">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="f68d9-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="f68d9-105">可以显式指定以 Windows 时区格式返回时区，或者以 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（也称为“Olson 时区”）格式返回。</span><span class="sxs-lookup"><span data-stu-id="f68d9-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="f68d9-106">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="f68d9-106">The Windows format is the default.</span></span>

<span data-ttu-id="f68d9-107">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选时区。</span><span class="sxs-lookup"><span data-stu-id="f68d9-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="f68d9-108">随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选时区。</span><span class="sxs-lookup"><span data-stu-id="f68d9-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="f68d9-109">权限</span><span class="sxs-lookup"><span data-stu-id="f68d9-109">Permissions</span></span>
<span data-ttu-id="f68d9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f68d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f68d9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f68d9-112">Permission type</span></span>      | <span data-ttu-id="f68d9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f68d9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f68d9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f68d9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f68d9-115">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f68d9-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="f68d9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f68d9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f68d9-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="f68d9-117">User.Read</span></span>    |
|<span data-ttu-id="f68d9-118">Application</span><span class="sxs-lookup"><span data-stu-id="f68d9-118">Application</span></span> | <span data-ttu-id="f68d9-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f68d9-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f68d9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f68d9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="f68d9-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="f68d9-121">Function parameters</span></span>
| <span data-ttu-id="f68d9-122">参数</span><span class="sxs-lookup"><span data-stu-id="f68d9-122">Parameter</span></span>      | <span data-ttu-id="f68d9-123">类型</span><span class="sxs-lookup"><span data-stu-id="f68d9-123">Type</span></span>    | <span data-ttu-id="f68d9-124">说明</span><span class="sxs-lookup"><span data-stu-id="f68d9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f68d9-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="f68d9-125">TimeZoneStandard</span></span>  | <span data-ttu-id="f68d9-126">String</span><span class="sxs-lookup"><span data-stu-id="f68d9-126">String</span></span>  | <span data-ttu-id="f68d9-127">时区格式。</span><span class="sxs-lookup"><span data-stu-id="f68d9-127">A time zone format.</span></span> <span data-ttu-id="f68d9-128">支持的值：`Windows` 和 `Iana`。</span><span class="sxs-lookup"><span data-stu-id="f68d9-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="f68d9-129">可选。</span><span class="sxs-lookup"><span data-stu-id="f68d9-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f68d9-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="f68d9-130">Request headers</span></span>
| <span data-ttu-id="f68d9-131">名称</span><span class="sxs-lookup"><span data-stu-id="f68d9-131">Name</span></span>       | <span data-ttu-id="f68d9-132">类型</span><span class="sxs-lookup"><span data-stu-id="f68d9-132">Type</span></span> | <span data-ttu-id="f68d9-133">说明</span><span class="sxs-lookup"><span data-stu-id="f68d9-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f68d9-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f68d9-134">Authorization</span></span>  | <span data-ttu-id="f68d9-135">string</span><span class="sxs-lookup"><span data-stu-id="f68d9-135">string</span></span>  | <span data-ttu-id="f68d9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f68d9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f68d9-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="f68d9-138">Request body</span></span>
<span data-ttu-id="f68d9-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f68d9-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f68d9-140">响应</span><span class="sxs-lookup"><span data-stu-id="f68d9-140">Response</span></span>
<span data-ttu-id="f68d9-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [timeZoneInformation](../resources/timezoneinformation.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f68d9-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f68d9-142">示例</span><span class="sxs-lookup"><span data-stu-id="f68d9-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="f68d9-143">请求 1</span><span class="sxs-lookup"><span data-stu-id="f68d9-143">Request 1</span></span>
<span data-ttu-id="f68d9-144">以下示例未指定 `timeZoneStandard` 参数，并获取以 Windows 时区格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="f68d9-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="f68d9-145">响应 1</span><span class="sxs-lookup"><span data-stu-id="f68d9-145">Response 1</span></span>
<span data-ttu-id="f68d9-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f68d9-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f68d9-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f68d9-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f68d9-148">C#</span><span class="sxs-lookup"><span data-stu-id="f68d9-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f68d9-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="f68d9-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f68d9-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="f68d9-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="f68d9-151">请求 2</span><span class="sxs-lookup"><span data-stu-id="f68d9-151">Request 2</span></span>
<span data-ttu-id="f68d9-152">以下示例指定 `TimeZoneStandard` 参数的 `Iana`，并获取以 IANA 格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="f68d9-152">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="f68d9-153">响应 2</span><span class="sxs-lookup"><span data-stu-id="f68d9-153">Response 2</span></span>
<span data-ttu-id="f68d9-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f68d9-154">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f68d9-155">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f68d9-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f68d9-156">C#</span><span class="sxs-lookup"><span data-stu-id="f68d9-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f68d9-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="f68d9-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f68d9-158">目标-C</span><span class="sxs-lookup"><span data-stu-id="f68d9-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
