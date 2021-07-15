---
title: Azure AD 目录对象的高级查询功能
description: Azure AD 目录对象支持高级查询功能以高效访问数据。
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: eb8b5b7b8438f900535efd6ce625059919d76952
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443198"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Azure AD 目录对象的高级查询功能

随着 Azure AD 在稳定性、可用性和性能方面不断提供更多功能和改进，Microsoft Graph 也在不断改进和扩展以便高效访问数据。 一个途径是 Microsoft Graph 对各种 Azure AD 对象及其属性的高级查询功能加强支持。 例如，在 2020 年 10 月，为 `$filter` 查询参数上添加了 **Not** (`NOT`)、**Not equals** (`ne`) 和 **Ends with** (`endsWith`) 运算符。

Microsoft Graph 查询引擎使用索引存储来满足查询请求。 为了进一步支持某些属性的查询功能，这些属性现在在单独的服务器中编制索引。 这种单独的索引使 Azure AD 可以增加支持并提高查询请求的性能。 然而，这些高级查询功能在默认情况下不可用，但是，请求者还必须将 **ConsistencyLevel** 标头设置为 `eventual` *和* (`$search`除外)，并使用 `$count` 查询参数。 **ConsistencyLevel** 标头和`$count`被称为 *高级查询参数*。

例如，如果只想检索非活动用户帐户，则可以运行使用 `$filter` 查询参数的查询之一。

+ 将 `$filter` 查询参数与 `eq` 运算符一起使用。 默认情况下，此请求将起作用，即请求不需要高级查询参数。

<!-- {
  "blockType": "ignored",
  "name": "get_users_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
```

+ 将 `$filter` 查询参数与 `ne` 运算符一起使用。 默认情况下不支持此请求，因为仅在高级查询中支持 `ne` 运算符。 因此，必须将 **ConsistencyLevel** 标头设置为 `eventual` *并* 使用 `$count=true` 查询字符串。

<!-- {
  "blockType": "ignored",
  "name": "get_users_not_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
ConsistencyLevel: eventual
```

这些高级查询功能仅在 Azure AD 对象上受支持，也就是以下资源及其派生自 [directoryObject](/graph/api/resources/directoryobject) 的关系:

- [application](/graph/api/resources/application)
- [orgContact](/graph/api/resources/orgcontact)
- [设备](/graph/api/resources/device)
- [组](/graph/api/resources/group)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [用户](/graph/api/resources/user)

下表列出了仅在高级查询中支持的目录对象的查询方案。

| 说明                                                              | 示例                                                                                                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 使用 `$count` 作为 URL 段                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                       |
| 使用 `$count` 作为查询字符串参数                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                     |
| 使用 `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                     |
| 对选择属性使用 `$orderby`                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                               |
| 将 `$filter` 与 `endsWith` 运算符结合使用                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                       |
| 在同一查询中使用`$filter`和`$orderby`                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                       |
| 对特定属性将 `$filter` 与 `startsWith` 运算符结合使用. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true` |
| 将 `$filter` 与 `ne` 和 `NOT` 运算符结合使用                           | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                     |
| 将 `$filter` 与 `NOT` 和 `startsWith` 运算符结合使用                   | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                |
| 将 OData 强制转换与其他查询参数一起使用                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                             |

> [!NOTE]
> 这些高级查询功能在 Azure AD B2C 租户中不可用。

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>支持筛选 Azure AD 目录对象的属性

目录对象的属性对查询参数的支持行为各不相同。 以下是目录对象的常见应用场景:

+ 除另有指示外，跨目录资源的同名属性支持相同的 `$filter` 运算符。 例如，**application**、**group**、**organization** 和 **user** 资源中提供了 **createdDateTime** 属性。 默认情况下，它支持 `eq`、 `ge`和 `le` 运算符，并且仅在高级查询中支持 `in`、 `ne`和 `NOT` 运算符。
+ 仅有 **mail** 和 **userPrincipalName** 属性支持`endsWith`运算符。
+ 默认情况下支持的查询也适用于高级查询。
+ 仅在高级查询中支持 `NOT` 和 `ne` 求反运算符。 
  + 支持 `eq` 运算符的所有属性也支持 `ne` 或 `NOT` 运算符。
  + 当`eq`运算符的计算结果为 `true`时，`ne`运算符求反。 对于使用 `any` lambda 运算符的查询，请使用 `NOT` 运算符。 请参阅[使用 lambda 运算符的筛选器](/graph/query-parameters#filter-using-lambda-operators)。

下表汇总了[users](/graph/api/resources/user)目录对象的属性对`$filter`运算符的支持。

- ![默认情况下有效。 不需要高级查询参数。](/graph/images/advanced-query-parameters/default.png) 默认情况下，该属性支持`$filter`使用运算符。
- ![需要高级查询参数。](/graph/images/advanced-query-parameters/advanced.png) 特定的 `$filter` 运算符需要 *高级查询参数*:
  - `ConsistencyLevel=eventual` 标头
  - `$count=true` 查询字符串
- 空白单元格表示该属性不支持 `$filter` 使用运算符。
- **null value** 列表明属性可根据 `null` 值进行筛选。
- 此处未列出的属性不支持 `$filter`。

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]


## <a name="error-handling-for-advanced-queries-on-directory-objects"></a>针对目录对象的高级查询的错误处理

仅支持使用高级查询参数对目录对象进行计数。 如果未指定 `ConsistencyLevel=eventual` 标头，则在使用 `$count` URL 段时，请求将返回错误或以无提示方式忽略 `$count` 查询参数(`?$count=true`)。

```http
https://graph.microsoft.com/v1.0/users/$count
```

```json
{
    "error": {
        "code": "Request_BadRequest",
        "message": "$count is not currently supported.",
        "innerError": {
            "date": "2021-05-18T19:03:10",
            "request-id": "d9bbd4d8-bb2d-44e6-99a1-71a9516da744",
            "client-request-id": "539da3bd-942f-25db-636b-27f6f6e8eae4"
        }
    }
}
```

对于目录对象， `$search` 仅适用于高级查询。 如果未指定 **ConsistencyLevel** 标头，则请求将返回错误。

```http
https://graph.microsoft.com/v1.0/applications?$search="displayName:Browser"
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Request with $search query parameter only works through MSGraph with a special request header: 'ConsistencyLevel: eventual'",
        "innerError": {
            "date": "2021-05-27T14:26:47",
            "request-id": "9b600954-ba11-4899-8ce9-6abad341f299",
            "client-request-id": "7964ef27-13a3-6ca4-ed7b-73c271110867"
        }
    }
}
```

如果 URL 中的属性或查询参数仅在高级查询中受支持，但缺少 **ConsistencyLevel** 标头或 `$count=true` 查询字符串，则请求将返回错误。

```http
https://graph.microsoft.com/v1.0/users?$filter=endsWith(mail,'@outlook.com')
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Unsupported Query.",
        "innerError": {
            "date": "2021-05-18T19:12:36",
            "request-id": "63f2093c-399c-4350-9609-3ce9b62abe3c",
            "client-request-id": "e60ed0ba-df5d-e190-f056-f9c0318456d7"
        }
    }
}
```

如果尚未为某个属性编制索引以支持查询参数，即使指定了高级查询参数，请求也将返回错误。

```http
https://graph.microsoft.com/v1.0/users?$filter=id ge '398164b1-5196-49dd-ada2-364b49f99b27'&$count=true
ConsistencyLevel: eventual
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "The request uses a filter property that is not indexed",
        "innerError": {
            "date": "2021-06-10T19:32:01",
            "request-id": "5625ba13-0c9f-4fce-a853-4b52f3e0bd09",
            "client-request-id": "76fe4cd8-df3a-f8c3-659b-594274b6bb31"
        }
    }
}
```

但是，值得注意的是请求中指定的查询参数可能会自行失败。 不支持的查询参数以及不支持的查询参数组合的情况就是如此。 在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。 例如，在下面的示例中，即使查询成功， `@odata.count` 参数也缺失。

```http
https://graph.microsoft.com/v1.0/users?$count=true
```

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "displayName":"Oscar Ward",
      "mail":"oscarward@contoso.com",
      "userPrincipalName":"oscarward@contoso.com"
    },
  ]
}
```

## <a name="see-also"></a>另请参阅

- [使用查询参数自定义响应](/graph/query-parameters)
- [查询参数限制](known-issues.md#query-parameter-limitations)
- [使用$search查询参数匹配搜索条件](/graph/search-query-parameter)
