---
title: 在 Microsoft Graph 中使用 $search 查询参数
description: Microsoft Graph 支持 $search OData 查询参数，以便限制请求的结果来匹配搜索条件。
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: c552f510eb65370cd331784c98ea7359b278a56d
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367008"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a>使用搜索查询参数匹配搜索条件

除了[其他 OData 查询参数](/graph/query-parameters)，Microsoft Graph 还支持`$search`查询参数，以便限制请求的结果来匹配搜索条件。

对`$search`查询参数的支持因实体而异，某些实体(例如派生自 [directoryObject](/graph/api/resources/directoryobject)的 Microsoft Azure Active Directory 资源)仅支持[高级查询](/graph/aad-advanced-queries)中的`$search`。

> [!NOTE]
> `$search`查询参数当前在 Azure AD B2C 租户中不可用。

## <a name="using-search-on-message-collections"></a>对 message 集合使用 $search

可根据特定邮件属性值搜索邮件。 搜索结果按邮件发送日期和时间进行排序。 `$search` 请求最多可返回 250 个结果。

如果确实要搜索邮件，且仅指定值，而未指定特定邮件属性，搜索依据为默认搜索属性 **from**、**subject** 和 **body**。

下面的示例返回登录用户收件箱中三个默认搜索属性中有任意一个包含“pizza”的所有邮件：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

也可以指定下表中的邮件属性名来搜索邮件，这些属性名可由关键字查询语言 (KQL) 语法识别。 这些属性名对应于 Microsoft Graph **message** 实体中定义的属性。 Outlook 和其他 Microsoft 365 应用程序（如 SharePoint）支持 KQL 语法，从而为数据存储提供了方便使用的公共发现域。


| 可搜索的电子邮件属性                | 说明 | 示例 
|:-------------------------|:------------|:---------|
| **attachment**           | 电子邮件附件的文件名。|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| **bcc**           | 电子邮件的 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| **body**           | 电子邮件正文。|[`me/messages?$search="body:excitement"`][search-body-example]
| **cc**           | 电子邮件的 **cc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| **from**           | 电子邮件的发件人，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| **hasAttachment** | 如果电子邮件附件不是内联附件，则为 true；否则，为 false。 |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| **importance**           | 发件人在发送邮件时可以指定的电子邮件重要性。 可取值包括 `low`、`medium` 或 `high`。|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| **Kind**           | 邮件类型。 可取值包括 `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks` 或 `voicemail`。|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| **participants**           | 电子邮件的 **from**、**to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="participants:danas"`][search-part-example]
| **received**           | 收件人接收电子邮件的日期。|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| **recipients**           | 电子邮件的 **to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| **sent**           | 发件人发送电子邮件的日期。|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| **size**           | 邮件大小（以字节为单位）。|[`me/messages?$search="size:1..500000"`][search-size-example]
| **subject**           | 电子邮件主题行中的文本。|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| **to**           | 电子邮件的 **to** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


若要详细了解 可搜索的电子邮件属性、KQL 语法、受支持的运算符和搜索技巧，请参阅以下文章：

- [Exchange 中的可搜索属性](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。

- [关键字查询语言 (KQL) 语法参考](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

## <a name="using-search-on-person-collections"></a>对 person 集合使用 $search

可以使用 Microsoft Graph [People API](/graph/api/resources/person) 检索与用户最相关的人员。 相关性由用户的通信和协作模式及业务关系决定。 People API 支持 `$search` 查询参数。 `$search` 请求最多可返回 250 个结果。

人员搜索就是按 [person](/graph/api/resources/person) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。

以下请求在已登录用户的 **人员** 集合中的每个人员的 **displayName** 和 **emailAddress** 属性中，为名为“Irene McGowen”的人员执行搜索。 由于一个名为“Irene McGowan”的人员与登录用户相关，因此返回了“Irene McGowan”的信息。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

以下示例显示了相应的响应。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people-example.md#search-people)。  

## <a name="using-search-on-directory-object-collections"></a>在目录对象集合上使用 $search

派生自 [directoryObject](/graph/api/resources/directoryobject) 的 Azure AD 资源及其关系仅在高级查询中支持 `$search` 查询参数。 使用标记化方法的搜索的工作原理是提取输入和输出字符串中的单词，并使用空格、数字、不同的大小写和符号分隔这些词，如下所示:

* **空格**：`hello world` => `hello`、 `world`
* **不同的大小写**⁽¹⁾：`HelloWorld` 或 `helloWORLD` => `hello`、`world`
* **符号**⁽⁾：`hello.world` => `hello`、`.`、`world`， `helloworld`
* **数字**：`hello123world` => `hello`、`123`、 `world`

⁽¹⁾ 目前，标记化仅在大小写从小写转换为大写时才有效，因此 `HELLOworld` 被视为一个标记：`helloworld`，`HelloWORld` 是两个标记：`hello`、`world`。 ⁽²⁾ 标记化逻辑还会合并仅由符号分隔的单词；例如，搜索 `helloworld` 将找到 `hello-world` 和 `hello.world`。

> **注意**：标记化后，标记将独立于原始大小写进行匹配，并且将以任何顺序匹配。

标记化搜索仅适用于 **displayName** 和 **description** 字段。 任何字符串类型的字段都可以放入 `$search`；非 **displayName** 和 **description** 的字段将默认遵循 `$filter` `startswith` 行为。 例如：

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

这将查找显示名称看起来像 "OneVideo" 的所有组。 也可与`$search`配合使用`$filter`。 例如：

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

这将查找显示名称类似于“OneVideo”的所有启用邮件的组。 结果是根据逻辑结合（"AND"）和`$filter`整个查询`$search`来限制。 搜索文本基于大小写进行标记，但是匹配以不区分大小写的方式执行。 例如，“OneVideo”将被分割成两个输入标记“one”和“video”，但是匹配不区分大小写的属性。

搜索的语法遵循以下规则：

* 通用格式：$search="clause1" \[AND \| OR\] "\[clauseX\]"\.
* 支持任何子句。 支持适用于优先级的括号。
* 每个子句的语法是："\<property>:\<text to search>"。
* 必须在子句中指定属性名称。 可以在中使用的任何属性`$filter`也可以在内使用 `$search`。 根据属性的不同，如果属性不支持搜索，那么搜索行为要么是“search”，要么是“start with”。
* 必须将完整子句部分置于双引号内。
* 必须将逻辑运算符 "AND" 和 "OR" 置于双引号之外。 它们必须处于大写形式。
* 考虑到整个子句部分需要放在双引号内，如果包含双引号和反斜杠，则需要使用反斜杠对其进行转义。其他字符不需要进行转义。

下表显示了一些示例。

| 对象类 | 说明 | 示例 |
| ------------ | ----------- | ------- |
| 用户 | 通讯簿显示用户的名称。 | 
  [
  https://graph.microsoft.com/beta/users?$search="displayName:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| 用户 | 通讯簿显示用户的名称或邮件。 | 
  [
  https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| Group | 通讯簿显群组的名称或说明。 | 
  [
  https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| Group | 通讯簿在启用邮件组上显示名称。 | 
  [
  https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |

你在 `$search` 中提供的字符串输入以及可搜索属性都按空格、不同的大小写和字符类型（数字和特殊字符）划分为多个部分。

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

## <a name="see-also"></a>另请参阅

- [使用查询参数自定义响应](/graph/query-parameters)
- [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)
- [查询参数限制](known-issues.md#query-parameter-limitations)