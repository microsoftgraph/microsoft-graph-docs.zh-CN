---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括 （通知时自动的人员的自动答复设置 '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 569a891e51d09c03467108c0a7ed012e04ba6352
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510244"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="4540b-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="4540b-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4540b-105">获取用户的[mailboxSettings](../resources/mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="4540b-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="4540b-106">这包括 （通知自动在收到其电子邮件时的人员） 的自动答复、 区域设置 （语言和国家/地区）、 时区、 和工作时间的设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-106">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="4540b-107">可以查看所有邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="4540b-108">时区是用户可以为用户邮箱设置的首选设置之一。</span><span class="sxs-lookup"><span data-stu-id="4540b-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="4540b-109">用户可选择它从[支持的时区](outlookuser-supportedtimezones.md)的管理员设置的用户的邮箱服务器。</span><span class="sxs-lookup"><span data-stu-id="4540b-109">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="4540b-110">管理员将设置中的 Windows 所在的时区格式或[Internet 分配编号证书颁发机构 (IANA) 所在的时区](https://www.iana.org/time-zones)（也称为 Olson 时区） 格式的时区。</span><span class="sxs-lookup"><span data-stu-id="4540b-110">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="4540b-111">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="4540b-111">The Windows format is the default.</span></span> 

<span data-ttu-id="4540b-112">获取用户的首选时区时，时区按创建时的格式返回。</span><span class="sxs-lookup"><span data-stu-id="4540b-112">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="4540b-113">若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="4540b-113">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="4540b-114">随后便可以获取相应格式的时区。</span><span class="sxs-lookup"><span data-stu-id="4540b-114">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="4540b-115">也可以在应用中单独管理格式转换。</span><span class="sxs-lookup"><span data-stu-id="4540b-115">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="4540b-116">权限</span><span class="sxs-lookup"><span data-stu-id="4540b-116">Permissions</span></span>
<span data-ttu-id="4540b-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4540b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4540b-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4540b-119">Permission type</span></span>      | <span data-ttu-id="4540b-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4540b-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4540b-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4540b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="4540b-122">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4540b-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4540b-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4540b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4540b-124">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4540b-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4540b-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="4540b-125">Application</span></span> | <span data-ttu-id="4540b-126">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4540b-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4540b-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4540b-127">HTTP request</span></span>
<span data-ttu-id="4540b-128">若要获取所有用户的邮箱设置：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4540b-128">To get all the mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="4540b-129">若要获取特定设置-仅自动答复设置、 区域设置、 时区、 或工作时间：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4540b-129">To get specific settings - only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4540b-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4540b-130">Optional query parameters</span></span>
<span data-ttu-id="4540b-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4540b-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4540b-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="4540b-132">Request headers</span></span>
| <span data-ttu-id="4540b-133">名称</span><span class="sxs-lookup"><span data-stu-id="4540b-133">Name</span></span>       | <span data-ttu-id="4540b-134">类型</span><span class="sxs-lookup"><span data-stu-id="4540b-134">Type</span></span> | <span data-ttu-id="4540b-135">说明</span><span class="sxs-lookup"><span data-stu-id="4540b-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4540b-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="4540b-136">Authorization</span></span>  | <span data-ttu-id="4540b-137">string</span><span class="sxs-lookup"><span data-stu-id="4540b-137">string</span></span>  | <span data-ttu-id="4540b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4540b-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4540b-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="4540b-140">Request body</span></span>
<span data-ttu-id="4540b-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4540b-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4540b-142">响应</span><span class="sxs-lookup"><span data-stu-id="4540b-142">Response</span></span>

<span data-ttu-id="4540b-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="4540b-143">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="4540b-144">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="4540b-144">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="4540b-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="4540b-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="4540b-146">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="4540b-146">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="4540b-147">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="4540b-147">string (for **timeZone**)</span></span>
- [<span data-ttu-id="4540b-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="4540b-148">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="4540b-149">示例</span><span class="sxs-lookup"><span data-stu-id="4540b-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="4540b-150">请求 1</span><span class="sxs-lookup"><span data-stu-id="4540b-150">Request 1</span></span>
<span data-ttu-id="4540b-151">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括时区、自动答复、区域设置（语言和国家/地区）和工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-151">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="4540b-152">响应 1</span><span class="sxs-lookup"><span data-stu-id="4540b-152">Response 1</span></span>
<span data-ttu-id="4540b-153">该响应中包括登录用户的所有邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-153">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="4540b-154">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4540b-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4540b-155">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4540b-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="4540b-156">请求 2</span><span class="sxs-lookup"><span data-stu-id="4540b-156">Request 2</span></span>
<span data-ttu-id="4540b-157">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-157">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="4540b-158">响应 2</span><span class="sxs-lookup"><span data-stu-id="4540b-158">Response 2</span></span>
<span data-ttu-id="4540b-p108">该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4540b-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```


##### <a name="request-3"></a><span data-ttu-id="4540b-162">请求 3</span><span class="sxs-lookup"><span data-stu-id="4540b-162">Request 3</span></span>
<span data-ttu-id="4540b-163">第三个示例专门获取已登录用户邮箱的工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-163">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="4540b-164">响应 3</span><span class="sxs-lookup"><span data-stu-id="4540b-164">Response 3</span></span>
<span data-ttu-id="4540b-165">该响应仅包括工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="4540b-165">The response includes only the working hours settings.</span></span> <span data-ttu-id="4540b-166">请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。</span><span class="sxs-lookup"><span data-stu-id="4540b-166">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="4540b-167">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4540b-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4540b-168">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4540b-168">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
