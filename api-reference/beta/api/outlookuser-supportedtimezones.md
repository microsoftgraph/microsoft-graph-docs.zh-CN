---
title: 'outlookUser: supportedTimeZones'
description: 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9a6e536c5eec85057a6c0788e282164a3bf24ee2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128671"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="5dcf2-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="5dcf2-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="5dcf2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dcf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dcf2-105">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="5dcf2-106">可以显式指定以 Windows 时区格式返回时区，或者以 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（也称为“Olson 时区”）格式返回。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="5dcf2-107">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-107">The Windows format is the default.</span></span>

<span data-ttu-id="5dcf2-108">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选时区。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="5dcf2-109">随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选时区。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="5dcf2-110">权限</span><span class="sxs-lookup"><span data-stu-id="5dcf2-110">Permissions</span></span>
<span data-ttu-id="5dcf2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dcf2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dcf2-113">Permission type</span></span>      | <span data-ttu-id="5dcf2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dcf2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dcf2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dcf2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5dcf2-116">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="5dcf2-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="5dcf2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dcf2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dcf2-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="5dcf2-118">User.Read</span></span>    |
|<span data-ttu-id="5dcf2-119">Application</span><span class="sxs-lookup"><span data-stu-id="5dcf2-119">Application</span></span> | <span data-ttu-id="5dcf2-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5dcf2-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dcf2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dcf2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="5dcf2-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="5dcf2-122">Function parameters</span></span>
| <span data-ttu-id="5dcf2-123">参数</span><span class="sxs-lookup"><span data-stu-id="5dcf2-123">Parameter</span></span>      | <span data-ttu-id="5dcf2-124">类型</span><span class="sxs-lookup"><span data-stu-id="5dcf2-124">Type</span></span>    | <span data-ttu-id="5dcf2-125">说明</span><span class="sxs-lookup"><span data-stu-id="5dcf2-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5dcf2-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="5dcf2-126">TimeZoneStandard</span></span>  | <span data-ttu-id="5dcf2-127">String</span><span class="sxs-lookup"><span data-stu-id="5dcf2-127">String</span></span>  | <span data-ttu-id="5dcf2-128">时区格式。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-128">A time zone format.</span></span> <span data-ttu-id="5dcf2-129">支持的值：`Windows` 和 `Iana`。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="5dcf2-130">可选。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5dcf2-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dcf2-131">Request headers</span></span>
| <span data-ttu-id="5dcf2-132">名称</span><span class="sxs-lookup"><span data-stu-id="5dcf2-132">Name</span></span>       | <span data-ttu-id="5dcf2-133">类型</span><span class="sxs-lookup"><span data-stu-id="5dcf2-133">Type</span></span> | <span data-ttu-id="5dcf2-134">说明</span><span class="sxs-lookup"><span data-stu-id="5dcf2-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5dcf2-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dcf2-135">Authorization</span></span>  | <span data-ttu-id="5dcf2-136">string</span><span class="sxs-lookup"><span data-stu-id="5dcf2-136">string</span></span>  | <span data-ttu-id="5dcf2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dcf2-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dcf2-139">Request body</span></span>
<span data-ttu-id="5dcf2-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dcf2-141">响应</span><span class="sxs-lookup"><span data-stu-id="5dcf2-141">Response</span></span>
<span data-ttu-id="5dcf2-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [timeZoneInformation](../resources/timezoneinformation.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dcf2-143">示例</span><span class="sxs-lookup"><span data-stu-id="5dcf2-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="5dcf2-144">请求 1</span><span class="sxs-lookup"><span data-stu-id="5dcf2-144">Request 1</span></span>
<span data-ttu-id="5dcf2-145">以下示例未指定 `timeZoneStandard` 参数，并获取以 Windows 时区格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="5dcf2-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dcf2-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="5dcf2-147">C#</span><span class="sxs-lookup"><span data-stu-id="5dcf2-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5dcf2-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5dcf2-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5dcf2-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5dcf2-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5dcf2-150">Java</span><span class="sxs-lookup"><span data-stu-id="5dcf2-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="5dcf2-151">响应 1</span><span class="sxs-lookup"><span data-stu-id="5dcf2-151">Response 1</span></span>
<span data-ttu-id="5dcf2-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-152">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="5dcf2-153">请求 2</span><span class="sxs-lookup"><span data-stu-id="5dcf2-153">Request 2</span></span>
<span data-ttu-id="5dcf2-154">以下示例指定 `TimeZoneStandard` 参数的 `Iana`，并获取以 IANA 格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-154">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5dcf2-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dcf2-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="5dcf2-156">C#</span><span class="sxs-lookup"><span data-stu-id="5dcf2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5dcf2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5dcf2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5dcf2-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5dcf2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5dcf2-159">Java</span><span class="sxs-lookup"><span data-stu-id="5dcf2-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="5dcf2-160">响应 2</span><span class="sxs-lookup"><span data-stu-id="5dcf2-160">Response 2</span></span>
<span data-ttu-id="5dcf2-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5dcf2-161">Here is an example of the response.</span></span> 

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
  ]
}
-->


