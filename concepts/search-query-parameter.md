---
title: 在 Microsoft Graph 中使用 $search 查询参数
description: Microsoft Graph 支持 $search OData 查询参数，以便限制请求的结果来匹配搜索条件。
author: mumbi-o
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: ffb1a8024f0db673d14177a06f0635fce5a2a271
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436944"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a>使用搜索查询参数匹配搜索条件

除了[其他 OData 查询参数](/graph/query-parameters)，Microsoft Graph 还支持`$search`查询参数，以便限制请求的结果来匹配搜索条件。

对`$search`查询参数的支持因实体而异，某些实体(例如派生自 [directoryObject](/graph/api/resources/directoryobject)的 Microsoft Azure Active Directory 资源)仅支持[高级查询](/graph/aad-advanced-queries)中的`$search`。

> [!NOTE]
> `$search`查询参数当前在 Azure AD B2C 租户中不可用。

## <a name="using-search-on-message-collections"></a>对 message 集合使用 $search

可根据特定邮件属性值搜索邮件。 搜索结果按邮件发送日期和时间进行排序。 `$search`请求最多返回 1000 个结果。

如果确实要搜索邮件，且仅指定值，而未指定特定邮件属性，搜索依据为默认搜索属性 **from**、**subject** 和 **body**。

下面的示例返回登录用户收件箱中三个默认搜索属性中有任意一个包含“pizza”的所有邮件：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

也可以指定下表中的邮件属性名来搜索邮件，这些属性名可由关键字查询语言 (KQL) 语法识别。 这些属性名对应于 Microsoft Graph **message** 实体中定义的属性。 Outlook 和其他 Microsoft 365 应用程序（如 SharePoint）支持 KQL 语法，从而为数据存储提供了方便使用的公共发现域。

| 可搜索的电子邮件属性 | 说明                                                                                                                                                             | 示例                                                                                                                          |
| :------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| **attachment**            | 电子邮件附件的文件名。                                                                                                                        | [GET][search-att-example] `../me/messages?$search="attachment:api-catalog.md"`                                                   |
| **bcc**                   | 电子邮件的 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。                                                                            | [GET][search-bcc-example] `../me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`                     |
| **body**                  | 电子邮件正文。                                                                                                                                           | [GET][search-body-example] `../me/messages?$search="body:excitement"`                                                            |
| **cc**                    | 电子邮件的 **cc** 字段，可指定为 SMTP 地址、显示名称或别名。                                                                             | [GET][search-cc-example] `../me/messages?$search="cc:danas"&$select=subject,ccRecipients`                                        |
| **from**                  | 电子邮件的发件人，可指定为 SMTP 地址、显示名称或别名。                                                                                   | [GET][search-from-example] `../me/messages?$search="from:randiw"&$select=subject,from`                                           |
| **hasAttachment**         | 如果电子邮件附件不是内联附件，则为 true；否则，为 false。                                                                      | [GET][search-from-example] `../me/messages?$search="hasAttachments:true"`                                                        |
| **importance**            | 发件人在发送邮件时可以指定的电子邮件重要性。 可取值包括 `low`、`medium` 或 `high`。                              | [GET][search-imp-example] `../me/messages?$search="importance:high"&$select=subject,importance`                                  |
| **Kind**                  | 邮件类型。 可取值包括 `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks` 或 `voicemail`。 | [GET][search-kind-example] `../me/messages?$search="kind:voicemail"`                                                             |
| **participants**          | 电子邮件的 **from**、**to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。                                             | [GET][search-part-example] `../me/messages?$search="participants:danas"`                                                         |
| **received**              | 收件人接收电子邮件的日期。                                                                                                             | [GET][search-rcvd-example] `../me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`                       |
| **recipients**            | 电子邮件的 **to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。                                                       | [GET][search-rcpts-example] `../me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients` |
| **sent**                  | 发件人发送电子邮件的日期。                                                                                                                  | [GET][search-sent-example] `../me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`                               |
| **size**                  | 邮件大小（以字节为单位）。                                                                                                                                           | [GET][search-size-example] `../me/messages?$search="size:1..500000"`                                                             |
| **subject**               | 电子邮件主题行中的文本。                                                                                                                     | [GET][search-sbj-example] `../me/messages?$search="subject:has"&$select=subject`                                                 |
| **to**                    | 电子邮件的 **to** 字段，可指定为 SMTP 地址、显示名称或别名。                                                                             | [GET][search-to-example]`.../me/messages?$search="to:randiw"&$select=subject,toRecipients`                                       |

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

派生自 [directoryObject](/graph/api/resources/directoryobject) 的 Azure AD 资源及其关系仅在高级查询中支持 `$search` 查询参数。 搜索执行 **不** 支持`contains` 。 相反，它使用词汇点化方法，该方法的工作方式是使用空格、数字、不同的大小写和符号从属性值和搜索字符串中提取单词，如以下示例所示：

- **空格**：`hello world` => `hello`、 `world`
- **不同的大小写**⁽¹⁾：`HelloWorld` 或 `helloWORLD` => `hello`、`world`
- **符号**⁽⁾：`hello.world` => `hello`、`.`、`world`， `helloworld`
- **数字**：`hello123world` => `hello`、`123`、 `world`

⁽¹⁾ 目前，标记化仅在大小写从小写转换为大写时才有效，因此 `HELLOworld` 被视为一个标记：`helloworld`，`HelloWORld` 是两个标记：`hello`、`world`。
⁽²⁾ 标记化逻辑还会合并仅由符号分隔的单词；例如，搜索 `helloworld` 将找到 `hello-world` 和 `hello.world`。

> [!NOTE]
>
> - 标记化后，标记将独立于原始大小写进行匹配，并且将以任何顺序匹配。 例如，displayName `李四(David Li)` 将匹配搜索字符串，例如 `李四(David Li)`、`李四`、`David`、`Li`、`David)`、`(李四`、 `Li 李`。
> - 标记化搜索仅适用于 **displayName** 和 **description** 字段。 字符串类型的任何字段都可以放入 `$search`; **displayName** 和 **说明之外的字段** 默认为 `$filter` `startswith` 行为。

例如：
# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/?$search="displayName:OneVideo OR mail:onevideo"
```

这将查找具有 `one` 和 `video` 令牌的所有显示名称的组，或以 `onevideo` 开头的邮件。  

`$search` 可与 `$filter` 一起使用：
# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_filter_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"
```

这将查找显示名称类似于“OneVideo”的所有启用邮件的组。
结果是根据逻辑结合（"AND"）和`$filter`整个查询`$search`来限制。

搜索的语法遵循以下规则：

- 通用格式：$search="clause1" \[AND \| OR\] "\[clauseX\]"\.
- 支持任何子句。 支持适用于优先级的括号。
- 每个子句的语法是："\<property>:\<text to search>"。
- 必须在子句中指定属性名称。 可以在中使用的任何属性`$filter`也可以在内使用 `$search`。 根据属性的不同，如果属性不支持搜索，则搜索行为是“search”或“startWith”。
- 必须在双引号内声明整个子句。 如果它包含双引号或反斜杠，则应使用反斜杠进行转义。 必须对所有其他特殊字符进行 URL 编码。
- 逻辑 `AND` 和 `OR` 运算符必须放在双引号之外，并且必须为大写。

下表显示了一些示例。

| 对象类 | 说明                                            | 示例                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------ | ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 用户         | 通讯簿显示用户的名称。                 | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr"`                                                                                                                    |
| 用户         | 通讯簿显示用户的名称或邮件。         | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr" OR "mail:Guthr"`                                                                          |
| Group        | 通讯簿显群组的名称或说明。 | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive"` |
| Group        | 通讯簿在启用邮件组上显示名称。     | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"`                                          |

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
- [查询参数限制](known-issues.md#query-parameters)
