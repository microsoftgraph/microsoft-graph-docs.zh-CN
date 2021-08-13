---
title: 在 Outlook 中共享或委派日历
description: 在 Outlook 中，日历所有者可与其他用户共享日历，或委派其他用户来管理所有者主要日历中的会议。
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 3e86fa3ec032e17e5859bd9bb76c9db4cb91df4571e59178264e8ef1c764e3cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237045"
---
# <a name="share-or-delegate-a-calendar-in-outlook"></a>在 Outlook 中共享或委派日历

在 Outlook 中，日历所有者可与其他用户共享日历。 所有者可以指定非私人活动中的哪些信息是可供查看的，并且可向同一组织中的用户授予对日历的写入访问权限。 

所有者还可以委派其他用户来管理所有者 _主要_ 日历中的会议。 委托人是指可以查看所有信息并对非私人活动具有写入访问权限的共享者。 他们还会收到会议请求和响应，并代表所有者响应会议请求。 此外，所有者可以向委托人授予在日历上查看所有者的 _私人_ 活动的显式权限。 

在日历共享或委派生效之前，所有者将向共享者或委托人发送邀请，共享者或委托人需要接受邀请，或者显式添加共享日历或委派日历以进行访问。邀请和添加共享日历或委派日历发生在 Outlook 客户端中。 

在 Outlook 中设置共享或委派后，应用可使用 Microsoft Graph API 管理共享和委派。

本文的其余部分基于以下示例方案：

- Alex Wilber 已将 Megan Bowen 委派到其主要日历，并且还允许 Megan 查看该日历中的私人活动。 
- Alex 与 Adele Vance 和 Megan Bowen 共享了一个“儿童派对”日历，并向 Adele 和 Megan 授予了`read`权限，允许他们查看“儿童派对”日历上的非私人活动的所有详细信息，以及私人活动的忙/闲状态。 

本文介绍如何使用共享或委派日历以编程方式执行以下任务：

- [获取有关共享者、委托人和允许的权限的日历信息，以及更新各个权限](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions)。
- [获取用于描述日历的共享或委派的属性](#get-properties-of-a-shared-or-delegated-calendar)。
- [获取或设置邮箱设置以接收委派日历的会议请求和响应](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses)。
- [删除日历的共享者或委托人](#delete-a-sharee-or-delegate-of-a-calendar)。

应用还可以使用通用版 API 执行以下操作：

- [获取共享或委托 Outlook 日历或其活动](outlook-get-shared-events-calendars.md)
- [在共享或委托日历中创建 Outlook 活动](outlook-create-event-in-shared-delegated-calendar.md)

> [!NOTE]
> 除日历属性 **isShared** 和 **isSharedWithMe** 外，该主题中描述的日历共享和委托的属性和 API 当前在 v1.0 终结点中可用。 这两个属性仅在 beta 终结点中公开。

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a>获取有关共享者和委托人的日历信息，以及更新各个权限

本节内容：

- [日历所有者：获取共享或委派信息及权限](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [日历所有者：在日历上更新现有共享者或委托人的权限](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

每个日历都与 [calendarPermission](/graph/api/resources/calendarpermission) 对象的集合相关联，其中每个对象都描述了日历所有者已设置的共享者或委托人以及关联权限。 [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) 枚举定义了 Microsoft Graph 支持的权限范围：

- `none` 此值仅适用于对日历没有任何权限的 `My Organization`。 它不适用于单个用户，因为只有具有权限的用户才与日历的 **calendarPermission** 对象相关联。
- `freeBusyRead` 共享者可以查看所有者的忙/闲状态，但不能查看日历上的其他详细信息。
- `limitedRead` 共享者可以查看所有者的忙/闲状态以及日历上的非私人活动的标题和位置。
- `read` 共享者可以查看所有者在私人活动中的忙/闲状态，以及日历上的非私人活动的所有详细信息。
- `write` 共享者可以查看所有者在私人活动中的忙/闲状态，还可以查看日历上的非私人活动的所有详细信息并进行编辑（创建、更新或删除）。
- `delegateWithoutPrivateEventAccess` _委托人_ 可以查看所有者在私人活动中的忙/闲状态，并且对日历上的非私人活动具有`write`访问权限。
- `delegateWithPrivateEventAccess` _委托人_ 可以查看所有者的私人活动和非私人活动的详细信息，并且对日历上的所有活动都具有`write`访问权限。

用户的主要日历始终与“我的组织”共享，它代表与所有者位于同一组织中的用户。 默认情况下，他们可以在该日历上读取所有者的忙/闲状态，并且具有`freeBusyRead`权限。


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a>日历所有者：获取共享或委派信息及权限

此示例演示在 Alex 或管理员同意的情况下，如何获取与 Alex 的主要日历关联的 **calendarPermission** 对象。 请求将返回两个此类权限对象：

- 第一个 **calendarPermission** 对象已分配给委托人 Megan，并且具有下列属性值：

  - **isRemovable** 设置为 true，为 Alex 提供了取消委派的选项。
  - **isInsideOrganization** 为 true，因为只有同一组织中的用户才能成为委托人。
  - Megan 的 **role** 是由 Alex 设置的 `delegateWithPrivateEventAccess`。
  - **allowedRoles** 包括支持委派的角色类型 `delegateWithoutPrivateEventAccess` 和 `delegateWithPrivateEventAccess`。
  - **emailAddress** 指定 Megan。

- 第二个 **calendarPermission** 对象是分配给“我的组织”的默认对象，并且具有下列属性值：

  - **isRemovable** 设置为 false，因为主要日历始终与所有者的组织共享。
  - **isInsideOrganization** 为 true。
  - **role** 为 `freeBusyRead`，即“我的组织”的默认设置。
  - **emailAddress** 将 **name** 子属性指定为“我的组织”；“我的组织”的 **address** 默认为 null。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派或应用程序权限，`Calendars.Read`。 有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarperms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarperms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarperms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendarperms",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/calendarPermissions",
    "value": [
        {
            "id": "L289RXhjaGFuZ2VMYWJTWVnYW5C",
            "isRemovable": true,
            "isInsideOrganization": true,
            "role": "delegateWithPrivateEventAccess",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read",
                "write",
                "delegateWithoutPrivateEventAccess",
                "delegateWithPrivateEventAccess"
            ],
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a>日历所有者：在日历上更新现有共享者或委托人的权限

在 Alex 或管理员同意的情况下，只要最初为该日历的共享者或委托人设置的这些 **allowedRoles** 支持新权限，你就可以更新分配给现有共享者或委托人的权限（由 **role** 属性指定）。 

除了 **role** 属性之外，你不能更新现有共享者或委托人的其他属性。 更改 **emailAddress** 属性值需要删除共享者或委托人，并再次设置 **calendarPermission** 的新实例。

此部分的示例更新了 **role** 属性，将自定义日历“儿童派对”的现有共享者 Adele 的权限从 `read` 更改为 `write`。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派或应用程序权限，`Calendars.ReadWrite`。 有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarperm",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJQWRlbGVW"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarperm-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarperm-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarperm-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "update_calendarperm",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AAMkADAwAABf02bAAAA%3D')/calendarPermissions/$entity",
    "id": "L289RXhjaGFuZ2VMYWJQWRlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a>获取共享或委托日历的属性

本节内容：

- [日历所有者：获取共享或委托日历的属性](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [共享者或委托人：获取共享或委托日历的属性](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

在本示例中，Alex 委派了他的主要日历，并向委托人 Megan Bowen 授予了查看标记为“私人”的日历项目的权限。
此部分显示委派日历的属性，首先从所有者 Alex 的角度出发并征得其同意，然后从委托人 Megan 的角度出发并征得其同意。 来自管理员的同意也适用于每种情况。

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a>日历所有者：获取共享或委托日历的属性

此部分的示例从所有者 Alex 的角度获取主要日历的属性。 

注意以下代表 Alex 的属性：

- **canShare** 为 true，因为 Alex 是所有者。
- **canViewPrivateItems** 为 true，因为 Alex 是所有者。
- **isShared** 设置为 true，因为 Alex 为此日历设置了委托人。
- 对于日历所有者，**isSharedWithMe** 始终为 false。
- **owner** 显示 Alex 为所有者。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派或应用程序权限，`Calendars.Read`。 有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAw7QAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": true,
    "isSharedWithMe": false,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a>共享者或委托人：获取共享或委托日历的属性

此部分的示例从委托人 Megan 的角度获取同一日历的属性。 

注意下列属性：

- 默认情况下，日历的 **name** 是所有者的显示名称。 在本例中，它是“Alex Wilber”，因为这是 Alex 委派给 Megan 的日历。 
- **canShare** 为 false，因为 Megan 不是此日历的所有者。
- 对于由 Alex 设置的委托人 Megan，**canViewPrivateItems** 为 true。 对于不是委托人的共享者，此属性始终为 false。
- **isShared** 为 false。 此属性仅向日历 _所有者_ 指示日历是共享日历还是委派日历。
- **isSharedWithMe** 属性为 true，因为 Megan 是委托人。
- **canEdit** 是 true，因为包括 Megan 在内的委托人具有写入访问权限。
- **owner** 设置为 Alex。

> [!NOTE] 
> 共享者或委托人只能自定义共享/委派日历的 **name** 属性。 更新仅对他们自己可见；日历所有者无法查看此类日历名称更改。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派权限 `Calendars.Read.Shared` 或应用程序权限 `Calendars.Read`。 有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-delegate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-delegate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-delegate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_delegate",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('meganb%40contoso.OnMicrosoft.com')/calendars/$entity",
    "id": "AAMkADlAABhbftjAAA=",
    "name": "Alex Wilber",
    "color": "auto",
    "hexColor": "",
    "changeKey": "E6LznKWmX0KTsAD9qRJjeAAAYWo3EQ==",
    "canShare": false,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": true,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": true,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a>获取或设置邮箱设置以接收会议请求和响应

本节内容：

- [获取用户邮箱的委派传递设置](#get-delegation-delivery-setting-for-a-users-mailbox)
- [设置用户邮箱的委派传递设置](#set-delegation-delivery-setting-for-a-users-mailbox)

根据日历所有者首选的委派级别，所有者可以指定接收会议请求和响应的人员，以管理日历上的会议。 

可通过编程方式获取或设置日历所有者的 [mailboxSettings](/graph/api/resources/mailboxsettings) 的 **delegateMeetingMessageDeliveryOptions** 属性，以指定 Outlook 应将 [eventMessageRequest](/graph/api/resources/eventmessagerequest) 和 [eventMessageResponse](/graph/api/resources/eventmessageresponse) 实例定向到的人员：

- `sendToDelegateOnly`

    Outlook 仅将 **eventMessageRequest** 和 **eventMessageResponse** 实例定向到委托人。 这是默认设置。 所有者可以通过委派日历中的相应 **活动** 来查看对会议的响应或对邀请的响应。
- `sendToDelegateAndInformationToPrincipal`

    Outlook 将 **eventMessageRequest** 和 **eventMessageResponse** 实例定向到委托人和日历所有者。 只有委托人才能看到接受和拒绝会议请求的选项。发送给所有者的通知将以一般电子邮件的形式显示。 所有者仍可以通过在委派日历中打开 **活动** 并做出响应来响应会议。
- `sendToDelegateAndPrincipal`

    Outlook 将 **eventMessageRequest** 和 **eventMessageResponse** 实例定向到委托人和日历所有者，他们都可以响应会议请求。

这是邮箱范围的设置，因此相同的设置适用于邮箱所有者的所有委托人。

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a>获取用户邮箱的委派传递设置

此部分的示例将获取日历所有者的 **mailboxSettings**，该所有者仅允许 Outlook 将会议请求和响应定向到日历委托人；即 **delegateMeetingMessageDeliveryOptions** 设置为 `sendToDelegateOnly`。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派或应用程序权限，`MailboxSettings.Read`。 有关邮箱权限的详细信息，请参阅[邮件权限](permissions-reference.md#mail-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "archiveFolder": "AQMkADAwAGVQAAAKfowAAAA==",
    "timeZone": "Pacific Standard Time",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly",
    "dateFormat": "M/d/yyyy",
    "timeFormat": "h:mm tt",
    "automaticRepliesSetting": {
        "status": "disabled",
        "externalAudience": "all",
        "internalReplyMessage": "",
        "externalReplyMessage": "",
        "scheduledStartDateTime": {
            "dateTime": "2019-12-24T05:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2019-12-25T05:00:00.0000000",
            "timeZone": "UTC"
        }
    },
    "language": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "workingHours": {
        "daysOfWeek": [
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone": {
            "name": "Pacific Standard Time"
        }
    }
}
```

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a>设置用户邮箱的委派传递设置

此部分的示例将 **delegateMeetingMessageDeliveryOptions** 属性更新为 `sendToDelegateAndPrincipal`，以让 Outlook 将委派日历的会议请求和响应定向到所有委托人和所有者。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派或应用程序权限，`MailboxSettings.ReadWrite`。 有关邮箱权限的详细信息，请参阅[邮件权限](permissions-reference.md#mail-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
Content-type: application/json

{
  "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "patch_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a>删除日历的共享者或委托人

在下面的示例中，Alex 将删除作为“儿童派对”日历共享者的 Megan。

**Microsoft Graph 权限**

对此操作视情况使用权限最低的委派或应用程序权限，`Calendars.ReadWrite`。 有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharee-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharee-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sharee-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "delete_sharee",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- Outlook 客户端如何支持共享和委派日历：
  - [与其他人共享 Outlook 日历](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [允许其他人作为委托人管理你的邮件和日历](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [在 Outlook 网页版中共享日历](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [Outlook 网页版中的日历委派](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [获取共享日历或委托日历中的 Outlook 事件](outlook-get-shared-events-calendars.md)
- [在共享或委托日历中创建 Outlook 活动](outlook-create-event-in-shared-delegated-calendar.md)
- [为什么要与 Outlook 日历集成](outlook-calendar-concept-overview.md)
- Microsoft Graph beta 中的[日历 API](/graph/api/resources/calendar)。
