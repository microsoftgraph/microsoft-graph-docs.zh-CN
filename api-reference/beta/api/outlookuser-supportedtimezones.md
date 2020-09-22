---
title: 'outlookUser: supportedTimeZones'
description: 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1ab9cefa4c97aa718d3590556da751adc37a766a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076813"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="4b61b-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="4b61b-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="4b61b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b61b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b61b-105">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="4b61b-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="4b61b-106">可以显式指定以 Windows 时区格式返回时区，或者以 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（也称为“Olson 时区”）格式返回。</span><span class="sxs-lookup"><span data-stu-id="4b61b-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="4b61b-107">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="4b61b-107">The Windows format is the default.</span></span>

<span data-ttu-id="4b61b-108">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选时区。</span><span class="sxs-lookup"><span data-stu-id="4b61b-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="4b61b-109">随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选时区。</span><span class="sxs-lookup"><span data-stu-id="4b61b-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="4b61b-110">权限</span><span class="sxs-lookup"><span data-stu-id="4b61b-110">Permissions</span></span>
<span data-ttu-id="4b61b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b61b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b61b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b61b-113">Permission type</span></span>      | <span data-ttu-id="4b61b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b61b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b61b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b61b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4b61b-116">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4b61b-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="4b61b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b61b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b61b-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="4b61b-118">User.Read</span></span>    |
|<span data-ttu-id="4b61b-119">Application</span><span class="sxs-lookup"><span data-stu-id="4b61b-119">Application</span></span> | <span data-ttu-id="4b61b-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b61b-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b61b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b61b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="4b61b-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="4b61b-122">Function parameters</span></span>
| <span data-ttu-id="4b61b-123">参数</span><span class="sxs-lookup"><span data-stu-id="4b61b-123">Parameter</span></span>      | <span data-ttu-id="4b61b-124">类型</span><span class="sxs-lookup"><span data-stu-id="4b61b-124">Type</span></span>    | <span data-ttu-id="4b61b-125">说明</span><span class="sxs-lookup"><span data-stu-id="4b61b-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b61b-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="4b61b-126">TimeZoneStandard</span></span>  | <span data-ttu-id="4b61b-127">String</span><span class="sxs-lookup"><span data-stu-id="4b61b-127">String</span></span>  | <span data-ttu-id="4b61b-128">时区格式。</span><span class="sxs-lookup"><span data-stu-id="4b61b-128">A time zone format.</span></span> <span data-ttu-id="4b61b-129">支持的值：`Windows` 和 `Iana`。</span><span class="sxs-lookup"><span data-stu-id="4b61b-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="4b61b-130">可选。</span><span class="sxs-lookup"><span data-stu-id="4b61b-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4b61b-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b61b-131">Request headers</span></span>
| <span data-ttu-id="4b61b-132">名称</span><span class="sxs-lookup"><span data-stu-id="4b61b-132">Name</span></span>       | <span data-ttu-id="4b61b-133">类型</span><span class="sxs-lookup"><span data-stu-id="4b61b-133">Type</span></span> | <span data-ttu-id="4b61b-134">说明</span><span class="sxs-lookup"><span data-stu-id="4b61b-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b61b-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b61b-135">Authorization</span></span>  | <span data-ttu-id="4b61b-136">string</span><span class="sxs-lookup"><span data-stu-id="4b61b-136">string</span></span>  | <span data-ttu-id="4b61b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b61b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b61b-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b61b-139">Request body</span></span>
<span data-ttu-id="4b61b-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b61b-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b61b-141">响应</span><span class="sxs-lookup"><span data-stu-id="4b61b-141">Response</span></span>
<span data-ttu-id="4b61b-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [timeZoneInformation](../resources/timezoneinformation.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4b61b-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b61b-143">示例</span><span class="sxs-lookup"><span data-stu-id="4b61b-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="4b61b-144">请求 1</span><span class="sxs-lookup"><span data-stu-id="4b61b-144">Request 1</span></span>
<span data-ttu-id="4b61b-145">以下示例未指定 `timeZoneStandard` 参数，并获取以 Windows 时区格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="4b61b-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="4b61b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b61b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="4b61b-147">C#</span><span class="sxs-lookup"><span data-stu-id="4b61b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b61b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b61b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b61b-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b61b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="4b61b-150">响应 1</span><span class="sxs-lookup"><span data-stu-id="4b61b-150">Response 1</span></span>
<span data-ttu-id="4b61b-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4b61b-151">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="4b61b-152">请求 2</span><span class="sxs-lookup"><span data-stu-id="4b61b-152">Request 2</span></span>
<span data-ttu-id="4b61b-153">以下示例指定 `TimeZoneStandard` 参数的 `Iana`，并获取以 IANA 格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="4b61b-153">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4b61b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b61b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="4b61b-155">C#</span><span class="sxs-lookup"><span data-stu-id="4b61b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b61b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b61b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b61b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b61b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="4b61b-158">响应 2</span><span class="sxs-lookup"><span data-stu-id="4b61b-158">Response 2</span></span>
<span data-ttu-id="4b61b-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4b61b-159">Here is an example of the response.</span></span> 

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


