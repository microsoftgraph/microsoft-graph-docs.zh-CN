---
title: 通过导航 Microsoft Graph 访问数据和方法
description: 除了使用 Microsoft Graph API 读取和写入数据，还可以使用大量的请求模式遍历 Microsoft Graph 中的资源。元数据文档还可帮助你了解 Microsoft Grap 中资源和关系的数据模型。
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 49d93659c17400aba84f1ed427648965856faef2
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896653"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a><span data-ttu-id="0f121-104">通过导航 Microsoft Graph 访问数据和方法</span><span class="sxs-lookup"><span data-stu-id="0f121-104">Access data and methods by navigating Microsoft Graph</span></span>

<span data-ttu-id="0f121-p102">除了使用 Microsoft Graph API 读取和写入数据，还可以使用大量的请求模式遍历 Microsoft Graph 中的资源。元数据文档还可帮助你了解 Microsoft Grap 中资源和关系的数据模型。</span><span class="sxs-lookup"><span data-stu-id="0f121-p102">In addition to using the Microsoft Graph API to read and write data, you can use a number of request patterns to traverse through the resources in Microsoft Graph. The metadata document also helps you to understand the data model of the resources and relationships in Microsoft Graph.</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="0f121-107">Microsoft Graph API 元数据</span><span class="sxs-lookup"><span data-stu-id="0f121-107">Microsoft Graph API metadata</span></span>

<span data-ttu-id="0f121-p103">在服务根处发布元数据文档 ($metadata)。可以通过以下 URL 查看 v1.0 和试用版的 Microsoft Graph API 服务文档。</span><span class="sxs-lookup"><span data-stu-id="0f121-p103">The metadata document ($metadata) is published at the service root. You can view the service document for the v1.0 and beta versions of the Microsoft Graph API via the following URLs.</span></span>

<span data-ttu-id="0f121-110">**Microsoft Graph API v1.0 元数据**</span><span class="sxs-lookup"><span data-stu-id="0f121-110">**Microsoft Graph API v1.0 metadata**</span></span>

```msgraph-interactive
https://graph.microsoft.com/v1.0/$metadata
```

<span data-ttu-id="0f121-111">**Microsoft Graph API beta 元数据**</span><span class="sxs-lookup"><span data-stu-id="0f121-111">**Microsoft Graph API beta metadata**</span></span>

```msgraph-interactive
https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="0f121-112">元数据允许你查看并了解 Microsoft Graph 数据模型，包括实体类型、复杂类型、组成在请求和响应数据包中表示的资源的枚举。</span><span class="sxs-lookup"><span data-stu-id="0f121-112">The metadata allows you to see and understand the Microsoft Graph data model, including the entity types, complex types, and enumerations that make up the resources represented in the request and response packets.</span></span> 

<span data-ttu-id="0f121-113">元数据还支持在相应的 OData 命名空间中定义类型、方法和枚举。</span><span class="sxs-lookup"><span data-stu-id="0f121-113">The metadata also supports defining types, methods, and enumerations in corresponding OData namespaces.</span></span> <span data-ttu-id="0f121-114">大多数 Microsoft Graph API 在 OData 命名空间 `microsoft.graph` 中定义。</span><span class="sxs-lookup"><span data-stu-id="0f121-114">The majority of the Microsoft Graph API is defined in the OData namespace, `microsoft.graph`.</span></span>

<span data-ttu-id="0f121-115">可以使用元数据了解 Microsoft Graph 中实体之间的关系，并建立可在这些实体间导航的 URL。</span><span class="sxs-lookup"><span data-stu-id="0f121-115">You can use the metadata to learn the relationships between entities in Microsoft Graph and establish URLs that navigate between those entities.</span></span>

> [!NOTE]
> - <span data-ttu-id="0f121-116">在使用资源 ID 时，应保持与其从 Microsoft Graph API 返回时相同的大小写。</span><span class="sxs-lookup"><span data-stu-id="0f121-116">Use resource IDs in the same case as they are returned from Microsoft Graph APIs.</span></span>
> - <span data-ttu-id="0f121-117">假设资源 ID、分配的值和其他 base-64 编码的值 _区分大小写_。</span><span class="sxs-lookup"><span data-stu-id="0f121-117">Assume resource IDs, values you assign, and other base-64-encoded values are _case-sensitive_.</span></span>
> - <span data-ttu-id="0f121-118">假设路径 URL 资源名称、查询参数、操作、函数名称及其请求正文参数（包括任何 API 属性名称和值）均 _不区分大小写_。</span><span class="sxs-lookup"><span data-stu-id="0f121-118">Assume path URL resource names, query parameters, action and function names, their request body parameters, including any API property names and values, are _not case-sensitive_.</span></span>

## <a name="view-a-collection-of-resources"></a><span data-ttu-id="0f121-119">查看资源集合</span><span class="sxs-lookup"><span data-stu-id="0f121-119">View a collection of resources</span></span>

<span data-ttu-id="0f121-p105">Microsoft Graph 让用户使用 HTTP `GET` 查询查看租户中的资源。查询响应包括每个资源的属性。实体资源是由其 ID 识别的。资源 ID 的格式可以是 GUID，通常根据资源类型而变化。</span><span class="sxs-lookup"><span data-stu-id="0f121-p105">Microsoft Graph lets you view resources in a tenant using HTTP `GET` queries. The query response includes properties of each resource. Entity resources are each identified by its ID. The format of a resource ID can be a GUID, and generally varies according to the resource type.</span></span>

<span data-ttu-id="0f121-124">例如，可以获取在租户中定义的[用户](/graph/api/resources/user)资源集合：</span><span class="sxs-lookup"><span data-stu-id="0f121-124">For example, you can get the collection of [user](/graph/api/resources/user) resources defined in a tenant:</span></span>

```
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="0f121-p106">如果成功，将会收到 200 OK 响应，其中包含有效负载中的 **user** 资源的集合。每个用户都由 **id** 属性标识，并附带其默认属性。为简单起见，下面所示的有效负载将被截断。</span><span class="sxs-lookup"><span data-stu-id="0f121-p106">If successful, you'll get a 200 OK response that contains the collection of **user** resources in the payload. Each user is identified by the **id** property and accompanied by its default properties. The payload shown below is truncated for brevity.</span></span>

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

<span data-ttu-id="0f121-p107">Microsoft Graph 还允许用户通过浏览不同资源之间的关系来查看集合。例如，通过用户的 **mailFolders** 导航属性，可以查询用户邮箱中的 [mailFolder](/graph/api/resources/mailfolder) 资源的集合：</span><span class="sxs-lookup"><span data-stu-id="0f121-p107">Microsoft Graph also lets you view collections by navigating the relationships of one resource with another. For example, through a user's **mailFolders** navigation property, you can query for the collection of [mailFolder](/graph/api/resources/mailfolder) resources in the user's mailbox:</span></span>

```
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="0f121-p108">如果成功，将会收到 200 OK 响应，其中包含有效负载中的 [mailFolder](/graph/api/resources/user) 资源的集合。每个 **mailFolder** 都由 **id** 属性标识，并附带其属性。为简单起见，下面所示的有效负载将被截断。</span><span class="sxs-lookup"><span data-stu-id="0f121-p108">If successful, you'll get a 200 OK response that contains the collection of [mailFolder](/graph/api/resources/user) resources in the payload. Each **mailFolder** is identified by the **id** property and accompanied by its properties. The payload shown below is truncated for brevity.</span></span>

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




## <a name="view-a-specific-resource-from-a-collection-by-id"></a><span data-ttu-id="0f121-133">按 ID 查看集合中的特定资源</span><span class="sxs-lookup"><span data-stu-id="0f121-133">View a specific resource from a collection by ID</span></span>

<span data-ttu-id="0f121-p109">继续以 **用户** 为例 - 若要查看用户的信息，请使用 HTTPS GET 请求，通过用户的 ID 来获取特定的用户。对于 **用户** 实体，则可以使用 **id** 或 **userPrincipalName** 属性作为标识。</span><span class="sxs-lookup"><span data-stu-id="0f121-p109">Continuing with using **user** as an example - to view the information about a user, use an HTTPS GET request to get a specific user by the user's ID. For a **user** entity, you can use either the **id** or **userPrincipalName** property as the identifier.</span></span>

<span data-ttu-id="0f121-136">以下请求示例使用 **userPrincipalName** 值作为用户 ID。</span><span class="sxs-lookup"><span data-stu-id="0f121-136">The following request example uses the **userPrincipalName** value as the user's ID.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="0f121-137">如果成功，便会收到“200 正常”响应，其中包含有效负载中的用户资源表示，如下所示。</span><span class="sxs-lookup"><span data-stu-id="0f121-137">If successful, you'll get a 200 OK response that contains the user resource representation in the payload, as shown.</span></span>

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

## <a name="read-specific-properties-of-a-resource"></a><span data-ttu-id="0f121-138">读取资源的特定属性</span><span class="sxs-lookup"><span data-stu-id="0f121-138">Read specific properties of a resource</span></span>
<span data-ttu-id="0f121-139">若要仅检索用户的传记数据（如用户提供的 _本人简介_ 描述和技能集），则可以在上一个请求中添加 [$select](query-parameters.md) 查询参数，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="0f121-139">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the [$select](query-parameters.md) query parameter to the previous request, as shown in the following example.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="0f121-140">成功的响应返回 200 OK 状态和有效负载，如下所示。</span><span class="sxs-lookup"><span data-stu-id="0f121-140">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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
<span data-ttu-id="0f121-141">此时，仅返回 **aboutMe**、**displayName** 和 **skills** 基本属性（而不是 **user** 实体上的整个属性集）。</span><span class="sxs-lookup"><span data-stu-id="0f121-141">Here, instead of the entire property sets on the **user** entity, only the **aboutMe**, **displayName**, and **skills** basic properties are returned.</span></span>

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a><span data-ttu-id="0f121-142">读取集合中资源的特定属性</span><span class="sxs-lookup"><span data-stu-id="0f121-142">Read specific properties of the resources in a collection</span></span>
<span data-ttu-id="0f121-143">除了读取单个资源的特定属性，还可以将类似的 [$select](query-parameters.md) 查询参数应用于集合，只要使用返回到各自的特定属性即可返回集合中的所有资源。</span><span class="sxs-lookup"><span data-stu-id="0f121-143">In addition to reading specific properties of a single resource, you can also apply the similar [$select](query-parameters.md) query parameter to a collection to get back all resources in the collection with just the specific properties returned on each.</span></span>

<span data-ttu-id="0f121-144">例如，要查询已登录用户的驱动器项目姓名，你可以提交以下 HTTPS GET 请求：</span><span class="sxs-lookup"><span data-stu-id="0f121-144">For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="0f121-145">成功的响应返回 200 OK 状态代码，以及仅包含共享文件名称的有效负载，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="0f121-145">The successful response returns a 200 OK status code and a payload that contains only the names of the shared files, as shown in the following example.</span></span>

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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a><span data-ttu-id="0f121-146">通过关系从某个资源遍历到其他资源</span><span class="sxs-lookup"><span data-stu-id="0f121-146">Traverse from one resource to another via relationship</span></span>
<span data-ttu-id="0f121-p110">经理与向其报告的其他用户保持 **directReports** 关系。若要查询用户的直接下属列表，则你可以使用以下 HTTPS GET 请求，通过关系遍历，导航到预期目标。</span><span class="sxs-lookup"><span data-stu-id="0f121-p110">A manager holds a **directReports** relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="0f121-149">成功响应返回“200 正常”状态和有效负载，如下所示。</span><span class="sxs-lookup"><span data-stu-id="0f121-149">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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

<span data-ttu-id="0f121-p111">同样地，可以根据关系导航至相关资源。例如，借助 user-messages 关系，可以从 Azure Active Directory (Azure AD) 用户遍历到 Outlook 邮件集。下面的示例显示如何在 REST API 调用中执行此操作：</span><span class="sxs-lookup"><span data-stu-id="0f121-p111">Similarly, you can follow a relationship to navigate to related resources. For example, the user-messages relationship enables traversal from an Azure Active Directory (Azure AD) User to a set of Outlook mail messages. The following example shows how to do this in a REST API call.</span></span>


```
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


<span data-ttu-id="0f121-153">成功响应返回“200 正常”状态和有效负载，如下所示。</span><span class="sxs-lookup"><span data-stu-id="0f121-153">The successful response returns the 200 OK status and a payload, as shown.</span></span>


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
<span data-ttu-id="0f121-154">通过转到元数据、查找 `EntityType`，并查看该 `EntityType` 的每个 `NavigationProperty`，可以查看给定资源上的所有关系。</span><span class="sxs-lookup"><span data-stu-id="0f121-154">You can see all the relationships on a given resource by going to the metadata, finding the `EntityType`, and looking at each `NavigationProperty` for that `EntityType`.</span></span>

## <a name="call-actions-and-functions"></a><span data-ttu-id="0f121-155">调用操作和函数</span><span class="sxs-lookup"><span data-stu-id="0f121-155">Call actions and functions</span></span>
<span data-ttu-id="0f121-p112">Microsoft Graph 还支持 _操作_ 和 _函数_，以操作资源的方式，而不是简单的创建、读取、更新和删除 (CRUD) 操作。它们通常以 HTTPS POST 请求的形式出现，以便为操作或函数接收参数。例如，以下操作让登录的用户 (`me`) 发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="0f121-p112">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not simply create, read, update, and delete (CRUD) operations. They are often in the shape of HTTPS POST requests in order to intake arguments for the action or function. For example, the following action lets the signed-in user (`me`) send an email message.</span></span>

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

<span data-ttu-id="0f121-p113">你可以查看元数据中可用的全部功能。它们显示为函数或操作。</span><span class="sxs-lookup"><span data-stu-id="0f121-p113">You can see all the functions that are available in the metadata. They appear as Functions or Actions.</span></span>

## <a name="use-the-microsoft-graph-sdks"></a><span data-ttu-id="0f121-161">使用 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="0f121-161">Use the Microsoft Graph SDKs</span></span>

<span data-ttu-id="0f121-p114">喜欢 SDK 的强大功能和易用性吗？虽然你可以随时使用 REST API 调用 Microsoft Graph，但我们还提供了适用于许多常用平台的 SDK。要研究可用的 SDK，请参阅[代码示例和 SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)。</span><span class="sxs-lookup"><span data-stu-id="0f121-p114">Like the power and ease of SDKs? While you can always use REST APIs to call Microsoft Graph, we also provide SDKs for many popular platforms. To explore the SDKs that are available, see [Code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>

## <a name="see-also"></a><span data-ttu-id="0f121-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0f121-165">See also</span></span>

- [<span data-ttu-id="0f121-166">使用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="0f121-166">Use the Microsoft Graph API</span></span>](use-the-api.md)
- [<span data-ttu-id="0f121-167">获取身份验证令牌</span><span class="sxs-lookup"><span data-stu-id="0f121-167">Get auth tokens</span></span>](./auth/index.yml)