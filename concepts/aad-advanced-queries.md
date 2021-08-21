---
title: Azure AD 目录对象的高级查询功能
description: Azure AD 目录对象支持高级查询功能以高效访问数据。
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 2393e21fd73d5aa9d599e234708b98ba3b9a9a4d
ms.sourcegitcommit: f645c2db38fe6354422a96b54569af53cd65b967
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2021
ms.locfileid: "58409051"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Azure AD 目录对象的高级查询功能

随着 Azure AD 在稳定性、可用性和性能方面不断提供更多功能和改进，Microsoft Graph 也在不断改进和扩展以便高效访问数据。 一个途径是 Microsoft Graph 对各种 Azure AD 对象及其属性的高级查询功能加强支持。 例如，在`$filter`查询参数上添加 **Not** （`not`），**不等于** （`ne`），**以** （`endsWith`） 运算符结尾。

Microsoft Graph 查询引擎使用索引存储来满足查询请求。 为了添加对某些属性的其他查询功能的支持，这些属性现在在单独的存储中编制索引。 这种单独的索引使 Azure AD 可以增加支持并提高查询请求的性能。 但是，这些高级查询功能在默认情况下不可用，但是，请求者还必须将 **ConsistencyLevel** 标头设置为`eventual`*，*（`$search`除外）使用`$count`查询参数。 **ConsistencyLevel** 标头和`$count`被称为 *高级查询参数*。

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

仅以下Azure AD目录对象子集及其关系支持这些高级查询功能：

| API/对象                                                                    | 关系                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [管理单元](/graph/api/resources/administrativeunit)           | <li>[members](/graph/api/administrativeunit-list-members)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [应用](/graph/api/resources/application)                          | <li>[所有者](/graph/api/application-list-owners)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [联系人](/graph/api/resources/orgContact)                                  | <li>[memberOf](/graph/api/orgcontact-list-memberof)<li> [transitiveMemberOf](/graph/api/orgcontact-list-transitiveMemberOf)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [Devices](/graph/api/resources/device)                                    | <li>[memberOf](/graph/api/device-list-memberof) <li> [transitiveMemberOf](/graph/api/device-list-transitivememberof) <li> [registeredUsers](/graph/api/device-list-registeredusers) <li> [registeredOwners](/graph/api/device-list-registeredowners)                                                                                                                                                                                                                                                                                                                                                             |
| [组](/graph/api/resources/group)                                      | <li>[members](/graph/api/group-list-members) <li> [transitiveMembers](/graph/api/group-list-transitivemembers) <li> [memberOf](/graph/api/group-list-memberof) <li> [transitiveMemberOf](/graph/api/group-list-transitivememberof) <li> [所有者](/graph/api/group-list-owners) <li> [appRoleAssignments](/graph/api/group-list-approleassignments)                                                                                                                                                                                                                                                                       |
| [服务主体](/graph/api/resources/serviceprincipal)               | <li>[memberOf](/graph/api/serviceprincipal-list-memberof), <li>[transitiveMemberOf](/graph/api/serviceprincipal-list-transitivememberof) <li> [appRoleAssignments](/graph/api/serviceprincipal-list-approleassignments) <li> [appRoleAssignmentsTo](/graph/api/serviceprincipal-list-approleassignedto) <li> [oAuth2PermissionGrant](/graph/api/serviceprincipal-list-oauth2permissiongrants)                                                                                                                                                                                                                 |
| [用户](/graph/api/resources/user)                                         | <li>[memberOf](/graph/api/user-list-memberof) <li> [transitiveMemberOf](/graph/api/user-list-transitivememberof)<li> [ownedObjects](/graph/api/user-list-ownedobjects) <li> [registeredDevices](/graph/api/user-list-registereddevices) <li> [ownedDevices](/graph/api/user-list-owneddevices) <li> [transitiveManagers](/graph/api/user-list-manager) <li> [directReports](/graph/api/user-list-directreports) <li> [transitiveReports](/graph/api/user-get-transitivereports) <li> [appRoleAssignments](/graph/api/user-list-approleassignments) <li> [oAuth2PermissionGrant](/graph/api/user-list-oauth2permissiongrants) |

下表列出了仅在高级查询中支持的目录对象的查询方案：

| 说明                                                              | 示例                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :----------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 使用 `$count` 作为 URL 段                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                       |
| 使用 `$count` 作为查询字符串参数                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                     |
| 使用 `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                     |
| 对选择属性使用 `$orderby`                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                               |
| 将 `$filter` 与 `endsWith` 运算符结合使用                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                       |
| 在同一查询中使用`$filter`和`$orderby`                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                       |
| 对特定属性将 `$filter` 与 `startsWith` 运算符结合使用. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true` |
| 将 `$filter` 与 `ne` 和 `NOT` 运算符结合使用                           | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                           |
| 将 `$filter` 与 `NOT` 和 `startsWith` 运算符结合使用                   | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                      |
| 将 OData 强制转换与其他查询参数一起使用                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                             |

> [!NOTE]
>
> + 仅高级查询支持将 `$filter` 和 `$orderBy` 结合使用。
> + 高级查询当前不支持`$expand`。
> + 高级查询功能目前不适用于Azure AD B2C租户。

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>支持筛选 Azure AD 目录对象的属性

目录对象的属性对查询参数的支持行为各不相同。 以下是目录对象的常见应用场景:

+ 默认情况下支持的查询也适用于高级查询，但响应最终会保持一致。
+ 默认情况下，只要默认支持`eq`运算符，则默认支持`in`运算符。
+ 仅`mail`和`userPrincipalName`属性的高级查询支持 `endsWith` 运算符。
+ 仅高级查询支持 `not` 和 `ne` 求反运算符。
  + 支持 `eq` 运算符的所有属性也支持 `ne` 或 `not` 运算符。
  + 对于使用 `any` lambda 运算符的查询，请使用 `not` 运算符。 请参阅[使用 lambda 运算符的筛选器](/graph/query-parameters#filter-using-lambda-operators)。

下表汇总了对高级 `$filter` 查询功能支持的目录对象属性的操作器的支持。

### <a name="legend"></a>图例

+ ![默认情况下有效。 不需要高级查询参数。](../concepts/images/advanced-query-parameters/default.svg) 默认情况下， `$filter` 运算符适用于该属性。
+ ![需要高级查询参数。](../concepts/images/advanced-query-parameters/advanced.svg) `$filter`运算符 **需要***高级查询参数*，其中包括：
  + `ConsistencyLevel=eventual` 标头
  + `$count=true` 查询字符串
+ ![不支持。](../concepts/images/advanced-query-parameters/notSupported.svg) 该属性不支持 `$filter` 运算符。 [向我们发送反馈](https://aka.ms/MsGraphAADSurveyDocs) ，请求此属性支持 `$filter` 方案。
+ 空白单元格指示查询对该属性无效。
+ 列 **null 值** 指示该属性可为 null 且可使用 `null`筛选。
+ 此处未列出的属性完全不支持 `$filter`。

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

+ [使用查询参数自定义响应](/graph/query-parameters)
+ [查询参数限制](known-issues.md#query-parameter-limitations)
+ [使用$search查询参数匹配搜索条件](/graph/search-query-parameter)
