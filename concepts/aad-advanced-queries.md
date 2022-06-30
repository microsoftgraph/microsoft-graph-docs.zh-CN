---
title: Azure AD 目录对象的高级查询功能
description: Azure AD 目录对象支持高级查询功能以高效访问数据。
author: Licantrop0
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 629a1deacf94cb619fc4898fe9f4cacefc57cb6b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437098"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Azure AD 目录对象的高级查询功能

随着 Azure AD 在稳定性、可用性和性能方面不断提供更多功能和改进，Microsoft Graph 也在不断改进和扩展以便高效访问数据。 一个途径是 Microsoft Graph 对各种 Azure AD 对象及其属性的高级查询功能加强支持。 例如，在 `$filter` 查询参数上添加 **not** (`not`)，**不等于** (`ne`)，**以** (`endsWith`) 运算符结尾。

Microsoft Graph 查询引擎使用索引存储来满足查询请求。 为了添加对某些属性的其他查询功能的支持，这些属性现在在单独的存储中编制索引。 这种单独的索引使 Azure AD 可以增加支持并提高查询请求的性能。 但是，这些高级查询功能在默认情况下不可用，但是，请求者还必须将 **ConsistencyLevel** 标头设置为`eventual`*，*（`$search`除外）使用`$count`查询参数。 **ConsistencyLevel** 标头和`$count`被称为 *高级查询参数*。

例如，要仅检索非活动用户帐户，你可以运行使用 `$filter` 查询参数的查询之一。

<!-- markdownlint-disable MD023 MD024 MD025 -->
+ 选项 1：将 `$filter` 查询参数与 运算符 `eq` 一同使用。 默认情况下，此请求将起作用，即请求不需要高级查询参数。

    # <a name="http"></a>[HTTP](#tab/http)
    <!-- {
      "blockType": "request",
      "name": "get_users_enabled"
    } -->
    ```msgraph-interactive
    GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
    ```

    # <a name="c"></a>[C#](#tab/csharp)

    ```csharp
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=CS
    var user = await graphClient.Users.Request()
        .Filter("accountEnabled eq false")
        .GetAsync();
    ```

    # <a name="javascript"></a>[JavaScript](#tab/javascript)

    ```javascript
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Javascript
    let users = await client.api('/users')
      .filter('accountEnabled eq false')
      .get();
    ```

    # <a name="objective-c"></a>[Objective-C](#tab/objc)

    ```objectivec
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Objective-C
    NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$filter=accountEnabled eq false"]]];
    [urlRequest setHTTPMethod:@"GET"];

    MSURLSessionDataTask *usersDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

      NSError *jsonError = nil;
      MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
      MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

    }];

    [usersDataTask execute];
    ```

    # <a name="java"></a>[Java](#tab/java)

    ```java
    // See https://docs.microsoft.com/en-us/graph/sdks/create-client?tabs=Java
    UserCollectionPage users = graphClient.users()
        .buildRequest()
        .filter("accountEnabled eq false")
        .get();
    ```

    # <a name="go"></a>[转到](#tab/go)

    ```go
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Go
    requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
        Filter: "accountEnabled eq false",
    }

    options := &msgraphsdk.UsersRequestBuilderGetOptions{
        Q: requestParameters,
    }

    result, err := client.Users().Get(options)
    ```

    # <a name="powershell"></a>[PowerShell](#tab/powershell)

    ```powershell
    Import-Module Microsoft.Graph.Users

    Get-MgUser -Filter "accountEnabled eq false"
    ```

    ---

+ 选项 2：将 `$filter` 查询参数与 运算符 `ne` 一同使用。 默认情况下不支持此请求，因为仅在高级查询中支持 `ne` 运算符。 因此，必须将 **ConsistencyLevel** 标头设置为 `eventual` *并* 使用 `$count=true` 查询字符串。

    # <a name="http"></a>[HTTP](#tab/http)
    <!-- {
      "blockType": "request",
      "name": "get_users_not_enabled"
    } -->
    ```msgraph-interactive
    GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
    ConsistencyLevel: eventual
    ```

    # <a name="c"></a>[C#](#tab/csharp)

    ```csharp
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=CS
    var user = await graphClient.Users.Request()
        .Request(new Option[] { new QueryOption("$count", "true")})
        .Header("ConsistencyLevel", "eventual")
        .Filter("accountEnabled ne true")
        .GetAsync();
    ```

    # <a name="javascript"></a>[JavaScript](#tab/javascript)

    ```javascript
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Javascript
    let users = await client.api('/users')
      .header('ConsistencyLevel','eventual')
      .filter('accountEnabled ne true')
      .count(true)
      .get();
    ```

    # <a name="objective-c"></a>[Objective-C](#tab/objc)

    ```objectivec
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Objective-C
    NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$filter=accountEnabled ne true&$count=true"]]];
    [urlRequest setHTTPMethod:@"GET"];
    [urlRequest setValue:@"eventual" forHTTPHeaderField:@"ConsistencyLevel"];

    MSURLSessionDataTask *usersDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

      NSError *jsonError = nil;
      MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
      MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

    }];

    [usersDataTask execute];
    ```

    # <a name="java"></a>[Java](#tab/java)

    ```java
    // See https://docs.microsoft.com/en-us/graph/sdks/create-client?tabs=Java
    LinkedList<Option> requestOptions = new LinkedList<Option>();
    requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
    requestOptions.add(new QueryOption("$count", "true"))

    UserCollectionPage users = graphClient.users()
        .buildRequest(requestOptions)
        .filter("accountEnabled ne true")
        .get();
    ```

    # <a name="go"></a>[转到](#tab/go)

    ```go
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Go
    requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
        Filter: "accountEnabled ne true",
        Count: true,
    }

    headers := map[string]string{
        "ConsistencyLevel": "eventual"
    }

    options := &msgraphsdk.UsersRequestBuilderGetOptions{
        Q: requestParameters,
        H: headers,
    }

    result, err := client.Users().Get(options)
    ```

    # <a name="powershell"></a>[PowerShell](#tab/powershell)

    ```powershell
    Import-Module Microsoft.Graph.Users

    Get-MgUser -Filter "accountEnabled ne true" -CountVariable CountVar -ConsistencyLevel eventual
    ```

    ---

<!-- markdownlint-enable MD023 MD024 MD025 -->

这些高级查询功能仅在Azure AD目录对象及其关系（包括以下常用对象）上受支持：

| Object                                                                                            | 关系                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [administrativeUnit](/graph/api/resources/administrativeunit)                                     | <li>[members](/graph/api/administrativeunit-list-members)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [application](/graph/api/resources/application)                                                   | <li>[所有者](/graph/api/application-list-owners)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [appRoleAssignment](/graph/api/resources/approleassignment)                                       | -                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [设备](/graph/api/resources/device)                                                             | <li>[memberOf](/graph/api/device-list-memberof) <li>[transitiveMemberOf](/graph/api/device-list-transitivememberof) <li>[registeredUsers](/graph/api/device-list-registeredusers) <li>[registeredOwners](/graph/api/device-list-registeredowners)                                                                                                                                                                                                                                                                                                                                                                   |
| [group](/graph/api/resources/group)                                                               | <li>[members](/graph/api/group-list-members) <li>[transitiveMembers](/graph/api/group-list-transitivemembers) <li>[memberOf](/graph/api/group-list-memberof) <li>[transitiveMemberOf](/graph/api/group-list-transitivememberof) <li>[所有者](/graph/api/group-list-owners) <li>[appRoleAssignments](/graph/api/group-list-approleassignments)                                                                                                                                                                                                                                                                       |
| [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)（委派的权限授予） | -                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [orgContact](/graph/api/resources/orgContact)                                                     | <li>[memberOf](/graph/api/orgcontact-list-memberof) <li>[transitiveMemberOf](/graph/api/orgcontact-list-transitiveMemberOf)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [servicePrincipal](/graph/api/resources/serviceprincipal)                                         | <li>[memberOf](/graph/api/serviceprincipal-list-memberof) <li>[transitiveMemberOf](/graph/api/serviceprincipal-list-transitivememberof) <li>[appRoleAssignments](/graph/api/serviceprincipal-list-approleassignments) <li>[appRoleAssignmentsTo](/graph/api/serviceprincipal-list-approleassignedto) <li>[oAuth2PermissionGrant](/graph/api/serviceprincipal-list-oauth2permissiongrants)                                                                                                                                                                                                                           |
| [user](/graph/api/resources/user)                                                                 | <li>[memberOf](/graph/api/user-list-memberof) <li>[transitiveMemberOf](/graph/api/user-list-transitivememberof)<li>[ownedObjects](/graph/api/user-list-ownedobjects) <li>[registeredDevices](/graph/api/user-list-registereddevices) <li>[ownedDevices](/graph/api/user-list-owneddevices) <li>[transitiveManagers](/graph/api/user-list-manager) <li>[directReports](/graph/api/user-list-directreports) <li>[transitiveReports](/graph/api/user-get-transitivereports) <li>[appRoleAssignments](/graph/api/user-list-approleassignments) <li>[oAuth2PermissionGrant](/graph/api/user-list-oauth2permissiongrants) |

下表列出了仅在高级查询中支持的目录对象的查询方案：

| 说明                                                              | 示例                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| :----------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 使用 `$count` 作为 URL 段                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                                                                           |
| 使用 `$count` 作为查询字符串参数                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                                                                         |
| 在 `$filter` 表达式中使用 `$count`                                | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedLicenses%2F%24count%2Bne%2B0%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedLicenses/$count eq 0&$count=true`                                                                                                                                   |
| 使用 `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                                                                         |
| 对选择属性使用 `$orderby`                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                                                                                   |
| 将 `$filter` 与 `endsWith` 运算符结合使用                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                                                                           |
| 在同一查询中使用`$filter`和`$orderby`                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                                                                           |
| 对特定属性将 `$filter` 与 `startsWith` 运算符结合使用. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`                                                     |
| 将 `$filter` 与 `ne` 和 `not` 运算符结合使用                           | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                                                                               |
| 将 `$filter` 与 `not` 和 `startsWith` 运算符结合使用                   | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                                                                          |
| 在带有 `endsWith` 运算符的集合上使用 `$filter`                | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DproxyAddresses%2Fany(p%3AendsWith(p%2C%2B'OnMicrosoft.com'))%26select%3Did%2CdisplayName%2Cproxyaddresses&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=proxyAddresses/any(p:endsWith(p,+'OnMicrosoft.com'))&select=id,displayName,proxyaddresses` |
| 将 OData 强制转换与可传递成员列表配合使用                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                                                                                 |
    
> [!NOTE]
>
> + 仅高级查询支持将 `$filter` 和 `$orderBy` 结合使用。
> + 高级查询当前不支持`$expand`。
> + 高级查询功能目前不适用于Azure AD B2C租户。
> + 若要在 [批处理请求](json-batching.md) 中使用高级查询功能，请在 `POST` 请求的 JSON 正文中指定 **ConsistencyLevel** 标头。

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>支持筛选 Azure AD 目录对象的属性

目录对象的属性对查询参数的支持行为各不相同。 以下是目录对象的常见应用场景:

+ 默认情况下支持的查询也适用于高级查询，但响应最终会保持一致。
+ 默认情况下，只要默认支持`eq`运算符，则默认支持`in`运算符。
+ 仅对 **mail**、**otherMails**、**userPrincipalName** 和 **proxyAddresses** 属性的高级查询支持 `endsWith` 运算符。
+ 仅高级查询支持 `not` 和 `ne` 求反运算符。
  + 支持 `eq` 运算符的所有属性也支持 `ne` 或 `not` 运算符。
  + 对于使用 `any` lambda 运算符的查询，请使用 `not` 运算符。 请参阅[使用 lambda 运算符的筛选器](/graph/query-parameters#filter-using-lambda-operators)。

下表汇总了对高级 `$filter` 查询功能支持的目录对象属性的操作器的支持。

### <a name="legend"></a>图例

+ ![默认情况下有效。 不需要高级查询参数。](../concepts/images/yesandnosymbols/greencheck.svg) 默认情况下， `$filter` 运算符适用于该属性。
+ ![需要高级查询参数。](../concepts/images/yesandnosymbols/whitecheck-in-greencircle.svg) `$filter`运算符 **需要***高级查询参数*，其中包括：
  + `ConsistencyLevel=eventual` 标头
  + `$count=true` 查询字符串
+ ![不支持。](../concepts/images/yesandnosymbols/no.svg) 该属性不支持 `$filter` 运算符。 [向我们发送反馈](https://aka.ms/MsGraphAADSurveyDocs) ，请求此属性支持 `$filter` 方案。
+ 空白单元格指示查询对该属性无效。
+ 列 **null 值** 指示该属性可为 null 且可使用 `null`筛选。
+ 此处未列出的属性完全不支持 `$filter`。

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]

## <a name="error-handling-for-advanced-queries-on-directory-objects"></a>针对目录对象的高级查询的错误处理

仅支持使用高级查询参数对目录对象进行计数。如果未指定 `ConsistencyLevel=eventual` 标头，则当 `$count` URL 段被使用时，请求将返回错误；如果使用了 `$count` 查询参数 (`?$count=true`)，则会无提示地忽略该参数。

<!-- {
  "blockType": "request",
  "name": "get_users_count_bad"
} -->
```http
https://graph.microsoft.com/v1.0/users/$count
```

<!-- {
  "blockType": "response",
  "@odata.type": "odata.error",
  "expectError": true
} -->
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

<!-- {
  "blockType": "request",
  "name": "get_applications_search_displayName"
} -->
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

<!-- {
  "blockType": "request",
  "name": "get_users_filer_endsWith"
} -->
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

<!-- {
  "blockType": "request",
  "name": "get_groups_unindexed_bad"
} -->
```http
https://graph.microsoft.com/beta/groups?$filter=createdDateTime ge 2021-11-01&$count=true
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

但是，值得注意的是请求中指定的查询参数可能会自行失败。
不支持的查询参数以及不支持的查询参数组合的情况就是如此。
在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。 例如，在下面的示例中，即使查询成功， `@odata.count` 参数也缺失。

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
+ [查询参数限制](known-issues.md#some-limitations-apply-to-query-parameters)
+ [使用$search查询参数匹配搜索条件](/graph/search-query-parameter#using-search-on-directory-object-collections)
+ [使用 .NET SDK 探索 Azure AD Directory 对象的高级查询功能](https://github.com/microsoftgraph/dotnet-aad-query-sample/)
