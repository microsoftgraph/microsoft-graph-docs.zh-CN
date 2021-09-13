---
title: 通过导航 Microsoft Graph 访问数据和方法
description: 除了使用 Microsoft Graph API 读取和写入数据，还可以使用大量的请求模式遍历 Microsoft Graph 中的资源。元数据文档还可帮助你了解 Microsoft Grap 中资源和关系的数据模型。
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 0fb759c39eb33dcd7bce16dffa0e39494938e597
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117639"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a>通过导航 Microsoft Graph 访问数据和方法

除了使用 Microsoft Graph API 读取和写入数据，还可以使用大量的请求模式遍历 Microsoft Graph 中的资源。元数据文档还可帮助你了解 Microsoft Grap 中资源和关系的数据模型。

## <a name="microsoft-graph-api-metadata"></a>Microsoft Graph API 元数据

在服务根处发布元数据文档 ($metadata)。可以通过以下 URL 查看 v1.0 和试用版的 Microsoft Graph API 服务文档。

**Microsoft Graph API v1.0 元数据**

```msgraph-interactive
https://graph.microsoft.com/v1.0/$metadata
```

**Microsoft Graph API beta 元数据**

```msgraph-interactive
https://graph.microsoft.com/beta/$metadata
```

元数据允许你查看并了解 Microsoft Graph 数据模型，包括实体类型、复杂类型、组成在请求和响应数据包中表示的资源的枚举。 

元数据还支持在相应的 OData 命名空间中定义类型、方法和枚举。 大多数 Microsoft Graph API 在 OData 命名空间 `microsoft.graph` 中定义。

可以使用元数据了解 Microsoft Graph 中实体之间的关系，并建立可在这些实体间导航的 URL。

> [!NOTE]
> - 在使用资源 ID 时，应保持与其从 Microsoft Graph API 返回时相同的大小写。
> - 假设资源 ID、分配的值和其他 base-64 编码的值 _区分大小写_。
> - 假设路径 URL 资源名称、查询参数、操作、函数名称及其请求正文参数（包括任何 API 属性名称和值）均 _不区分大小写_。

## <a name="view-a-collection-of-resources"></a>查看资源集合

Microsoft Graph 让用户使用 HTTP `GET` 查询查看租户中的资源。查询响应包括每个资源的属性。实体资源是由其 ID 识别的。资源 ID 的格式可以是 GUID，通常根据资源类型而变化。

例如，可以获取在租户中定义的[用户](/graph/api/resources/user)资源集合：

```
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

如果成功，将会收到 200 OK 响应，其中包含有效负载中的 **user** 资源的集合。每个用户都由 **id** 属性标识，并附带其默认属性。为简单起见，下面所示的有效负载将被截断。

```
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

Microsoft Graph 还允许用户通过浏览不同资源之间的关系来查看集合。例如，通过用户的 **mailFolders** 导航属性，可以查询用户邮箱中的 [mailFolder](/graph/api/resources/mailfolder) 资源的集合：

```
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

如果成功，将会收到 200 OK 响应，其中包含有效负载中的 [mailFolder](/graph/api/resources/user) 资源的集合。每个 **mailFolder** 都由 **id** 属性标识，并附带其属性。为简单起见，下面所示的有效负载将被截断。

```
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a>按 ID 查看集合中的特定资源

继续以 **用户** 为例 - 若要查看用户的信息，请使用 HTTPS GET 请求，通过用户的 ID 来获取特定的用户。对于 **用户** 实体，则可以使用 **id** 或 **userPrincipalName** 属性作为标识。

以下请求示例使用 **userPrincipalName** 值作为用户 ID。

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

如果成功，便会收到“200 正常”响应，其中包含有效负载中的用户资源表示，如下所示。

```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ...
}
```

## <a name="read-specific-properties-of-a-resource"></a>读取资源的特定属性
若要仅检索用户的传记数据（如用户提供的 _本人简介_ 描述和技能集），则可以在上一个请求中添加 [$select](query-parameters.md) 查询参数，如以下示例所示。

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

成功的响应返回 200 OK 状态和有效负载，如下所示。

```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
此时，仅返回 **aboutMe**、**displayName** 和 **skills** 基本属性（而不是 **user** 实体上的整个属性集）。

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>读取集合中资源的特定属性
除了读取单个资源的特定属性，还可以将类似的 [$select](query-parameters.md) 查询参数应用于集合，只要使用返回到各自的特定属性即可返回集合中的所有资源。

例如，要查询已登录用户的驱动器项目姓名，你可以提交以下 HTTPS GET 请求：

```
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

成功的响应返回 200 OK 状态代码，以及仅包含共享文件名称的有效负载，如以下示例所示。

```
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>通过关系从某个资源遍历到其他资源
经理与向其报告的其他用户保持 **directReports** 关系。若要查询用户的直接下属列表，则你可以使用以下 HTTPS GET 请求，通过关系遍历，导航到预期目标。

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

成功响应返回“200 正常”状态和有效负载，如下所示。

```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

同样地，可以根据关系导航至相关资源。例如，借助 user-messages 关系，可以从 Azure Active Directory (Azure AD) 用户遍历到 Outlook 邮件集。下面的示例显示如何在 REST API 调用中执行此操作：


```
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


成功响应返回“200 正常”状态和有效负载，如下所示。


```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",

       ...
    }
  ]
}
```
通过转到元数据、查找 `EntityType`，并查看该 `EntityType` 的每个 `NavigationProperty`，可以查看给定资源上的所有关系。

## <a name="call-actions-and-functions"></a>调用操作和函数
Microsoft Graph 还支持 _操作_ 和 _函数_，以操作资源的方式，而不是简单的创建、读取、更新和删除 (CRUD) 操作。它们通常以 HTTPS POST 请求的形式出现，以便为操作或函数接收参数。例如，以下操作让登录的用户 (`me`) 发送电子邮件。

```
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@contoso.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

你可以查看元数据中可用的全部功能。它们显示为函数或操作。

## <a name="use-the-microsoft-graph-sdks"></a>使用 Microsoft Graph SDK

喜欢 SDK 的强大功能和易用性吗？虽然你可以随时使用 REST API 调用 Microsoft Graph，但我们还提供了适用于许多常用平台的 SDK。要研究可用的 SDK，请参阅[代码示例和 SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)。

## <a name="see-also"></a>另请参阅

- [使用 Microsoft Graph API](use-the-api.md)
- [获取身份验证令牌](./auth/index.yml)
