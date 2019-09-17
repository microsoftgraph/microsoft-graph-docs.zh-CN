---
title: 通过导航 Microsoft Graph 访问数据和方法
description: 除了使用 Microsoft Graph API 读取和写入数据，还可以使用大量的请求模式遍历 Microsoft Graph 中的资源。元数据文档还可帮助你了解 Microsoft Grap 中资源和关系的数据模型。
localization_priority: Priority
scenarios: getting-started
ms.openlocfilehash: b2f9f5002b4743a61bbaf18af2408e10de12d463
ms.sourcegitcommit: c739cbfab42181adfcda409ca12514ab7f4832b1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982871"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a><span data-ttu-id="3515a-104">通过导航 Microsoft Graph 访问数据和方法</span><span class="sxs-lookup"><span data-stu-id="3515a-104">Access data and methods by navigating Microsoft Graph</span></span>

<span data-ttu-id="3515a-p102">除了使用 Microsoft Graph API 读取和写入数据，还可以使用大量的请求模式遍历 Microsoft Graph 中的资源。元数据文档还可帮助你了解 Microsoft Grap 中资源和关系的数据模型。</span><span class="sxs-lookup"><span data-stu-id="3515a-p102">In addition to using the Microsoft Graph API to read and write data, you can use a number of request patterns to traverse through the resources in Microsoft Graph. The metadata document also helps you to understand the data model of the resources and relationships in Microsoft Graph.</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="3515a-107">Microsoft Graph API 元数据</span><span class="sxs-lookup"><span data-stu-id="3515a-107">Microsoft Graph API metadata</span></span>

<span data-ttu-id="3515a-p103">在服务根处发布元数据文档 ($metadata)。可以通过以下 URL 查看 v1.0 和试用版的 Microsoft Graph API 服务文档。</span><span class="sxs-lookup"><span data-stu-id="3515a-p103">The metadata document ($metadata) is published at the service root. You can view the service document for the v1.0 and beta versions of the Microsoft Graph API via the following URLs.</span></span>

<span data-ttu-id="3515a-110">**Microsoft Graph API v1.0 元数据**</span><span class="sxs-lookup"><span data-stu-id="3515a-110">**Microsoft Graph API v1.0 metadata**</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```

<span data-ttu-id="3515a-111">**Microsoft Graph API beta 元数据**</span><span class="sxs-lookup"><span data-stu-id="3515a-111">**Microsoft Graph API beta metadata**</span></span>

```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="3515a-112">元数据允许你查看并了解 Microsoft Graph 数据模型，包括实体类型、复杂类型、组成在请求和响应数据包中表示的资源的枚举。</span><span class="sxs-lookup"><span data-stu-id="3515a-112">The metadata allows you to see and understand the Microsoft Graph data model, including the entity types, complex types, and enumerations that make up the resources represented in the request and response packets.</span></span>

<span data-ttu-id="3515a-113">可以使用元数据了解 Microsoft Graph 中实体之间的关系，并建立可在这些实体间导航的 URL。</span><span class="sxs-lookup"><span data-stu-id="3515a-113">You can use the metadata to learn the realtionships between entities in Microsoft Graph and establish URLs that navigate between those entities.</span></span>

> [!NOTE]
> - <span data-ttu-id="3515a-114">在使用资源 ID 时，应保持与其从 Microsoft Graph API 返回时相同的大小写。</span><span class="sxs-lookup"><span data-stu-id="3515a-114">Use resource IDs in the same case as they are returned from Microsoft Graph APIs.</span></span>
> - <span data-ttu-id="3515a-115">假设资源 ID、分配的值和其他 base-64 编码的值_区分大小写_。</span><span class="sxs-lookup"><span data-stu-id="3515a-115">Assume resource IDs, values you assign, and other base-64-encoded values are _case-sensitive_.</span></span>
> - <span data-ttu-id="3515a-116">假设路径 URL 资源名称、查询参数、操作、函数名称及其请求正文参数（包括任何 API 属性名称和值）均_不区分大小写_。</span><span class="sxs-lookup"><span data-stu-id="3515a-116">Assume path URL resource names, query parameters, action and function names, their request body parameters, including any API property names and values, are _not case-sensitive_.</span></span>

## <a name="view-a-collection-of-resources"></a><span data-ttu-id="3515a-117">查看资源集合</span><span class="sxs-lookup"><span data-stu-id="3515a-117">View a collection of resources</span></span>

<span data-ttu-id="3515a-118">Microsoft Graph 允许用户使用 HTTP `GET` 查询来查看租户中的资源。</span><span class="sxs-lookup"><span data-stu-id="3515a-118">Microsoft Graph lets you view resources in a tenant using HTTP `GET` queries.</span></span> <span data-ttu-id="3515a-119">查询响应包括每个资源的属性。</span><span class="sxs-lookup"><span data-stu-id="3515a-119">The query response includes properties of each resource.</span></span> <span data-ttu-id="3515a-120">实体资源均由其 ID 标识。</span><span class="sxs-lookup"><span data-stu-id="3515a-120">Entity resources are each identified by its ID.</span></span> <span data-ttu-id="3515a-121">资源 ID 的格式可以是 GUID，并且通常根据资源类型而变化。</span><span class="sxs-lookup"><span data-stu-id="3515a-121">The format of a resource ID can be a GUID, and generally varies according to the resource type.</span></span>

<span data-ttu-id="3515a-122">例如，可以获取在租户中定义的[用户](/graph/api/resources/user?view=graph-rest-1.0)资源集合：</span><span class="sxs-lookup"><span data-stu-id="3515a-122">For example, you can get the collection of users defined in a tenant:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="3515a-p105">如果成功，将会收到 200 OK 响应，其中包含有效负载中的 **user** 资源的集合。每个用户都由 **id** 属性标识，并附带其默认属性。为简单起见，下面所示的有效负载将被截断。</span><span class="sxs-lookup"><span data-stu-id="3515a-p105">If successful, you'll get a 200 OK response that contains the collection of **user** resources in the payload. Each user is identified by the **id** property and accompanied by its default properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight
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

<span data-ttu-id="3515a-p106">Microsoft Graph 还允许用户通过浏览不同资源之间的关系来查看集合。例如，通过用户的 **mailFolders** 导航属性，可以查询用户邮箱中的 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) 资源的集合：</span><span class="sxs-lookup"><span data-stu-id="3515a-p106">Microsoft Graph also lets you view collections by navigating the relationships of one resource with another. For example, through a user's **mailFolders** navigation property, you can query for the collection of [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resources in the user's mailbox:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="3515a-p107">如果成功，将会收到 200 OK 响应，其中包含有效负载中的 [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) 资源的集合。每个 **mailFolder** 都由 **id** 属性标识，并附带其属性。为简单起见，下面所示的有效负载将被截断。</span><span class="sxs-lookup"><span data-stu-id="3515a-p107">If successful, you'll get a 200 OK response that contains the collection of [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) resources in the payload. Each **mailFolder** is identified by the **id** property and accompanied by its properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight
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




## <a name="view-a-specific-resource-from-a-collection-by-id"></a><span data-ttu-id="3515a-131">按 ID 查看集合中的特定资源</span><span class="sxs-lookup"><span data-stu-id="3515a-131">View a specific resource from a collection by ID</span></span>

<span data-ttu-id="3515a-132">继续使用**用户**作为示例 - 要查看有关用户的信息，则使用 HTTP GET 请求根据用户 ID 获取特定用户。</span><span class="sxs-lookup"><span data-stu-id="3515a-132">Continuing with using **user** as an example - to view the information about a user, use an HTTPS GET request to get a specific user by the user's ID. For a user entity, you can use either the id or userPrincipalName property as the identifier. The following request example uses the userPrincipalName value as the user's ID.</span></span> <span data-ttu-id="3515a-133">对于**用户**实体，可以使用 **id** 或 **userPrincipalName** 属性作为标识符。</span><span class="sxs-lookup"><span data-stu-id="3515a-133">For a **user** entity, you can use either the **id** or **userPrincipalName** property as the identifier.</span></span>

<span data-ttu-id="3515a-134">以下请求示例使用 **userPrincipalName** 值作为用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3515a-134">The following example request uses the \*\*\*\* value as the user's id.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="3515a-135">如果成功，便会收到“200 正常”响应，其中包含有效负载中的用户资源表示，如下所示。</span><span class="sxs-lookup"><span data-stu-id="3515a-135">If successful, you'll get a 200 OK response that contains the user resource representation in the payload, as shown.</span></span>

```no-highlight
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

## <a name="read-specific-properties-of-a-resource"></a><span data-ttu-id="3515a-136">读取资源的特定属性</span><span class="sxs-lookup"><span data-stu-id="3515a-136">Read specific properties of a resource</span></span>
<span data-ttu-id="3515a-137">若要仅检索用户的传记数据（如用户提供的_本人简介_描述和技能集），则可以在上一个请求中添加 [$select](query-parameters.md) 查询参数，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="3515a-137">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the [$select](query-parameters.md) query parameter to the previous request, as shown in the following example.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="3515a-138">成功的响应返回 200 OK 状态和有效负载，如下所示。</span><span class="sxs-lookup"><span data-stu-id="3515a-138">The successful response returns the 200 OK status and a payload, as shown.</span></span>

```no-highlight
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
<span data-ttu-id="3515a-139">此时，仅返回 **aboutMe**、**displayName** 和 **skills** 基本属性（而不是 **user** 实体上的整个属性集）。</span><span class="sxs-lookup"><span data-stu-id="3515a-139">Here, instead of the entire property sets on the **user** entity, only the **aboutMe**, **displayName**, and **skills** basic properties are returned.</span></span>

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a><span data-ttu-id="3515a-140">读取集合中资源的特定属性</span><span class="sxs-lookup"><span data-stu-id="3515a-140">Read specific properties of the resources in a collection</span></span>
<span data-ttu-id="3515a-141">除了读取单个资源的特定属性，还可以将类似的 [$select](query-parameters.md) 查询参数应用于集合，只要使用返回到各自的特定属性即可返回集合中的所有资源。</span><span class="sxs-lookup"><span data-stu-id="3515a-141">In addition to reading specific properties of a single resource, you can also apply the similar [$select](query-parameters.md) query parameter to a collection to get back all resources in the collection with just the specific properties returned on each. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request.</span></span>

<span data-ttu-id="3515a-142">例如，要查询已登录用户的驱动器项目姓名，你可以提交以下 HTTPS GET 请求：</span><span class="sxs-lookup"><span data-stu-id="3515a-142">For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="3515a-143">成功的响应返回 200 OK 状态代码，以及仅包含共享文件名称的有效负载，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="3515a-143">The successful response returns a 200 OK status code and a payload that contains only the names of the shared files, as shown in the following example.</span></span>

```no-highlight
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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a><span data-ttu-id="3515a-144">通过关系从某个资源遍历到其他资源</span><span class="sxs-lookup"><span data-stu-id="3515a-144">Traverse from one resource to another via relationship</span></span>
<span data-ttu-id="3515a-p109">经理与向其报告的其他用户保持 **directReports** 关系。若要查询用户的直接下属列表，则你可以使用以下 HTTPS GET 请求，通过关系遍历，导航到预期目标。</span><span class="sxs-lookup"><span data-stu-id="3515a-p109">A manager holds a **directReports** relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="3515a-147">成功响应返回“200 正常”状态和有效负载，如下所示。</span><span class="sxs-lookup"><span data-stu-id="3515a-147">The successful response returns the 200 OK status and a payload, as shown.</span></span>

```no-highlight
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

<span data-ttu-id="3515a-p110">同样地，可以根据关系导航至相关资源。例如，借助 user-messages 关系，可以从 Azure Active Directory (Azure AD) 用户遍历到 Outlook 邮件集。下面的示例显示如何在 REST API 调用中执行此操作：</span><span class="sxs-lookup"><span data-stu-id="3515a-p110">Similarly, you can follow a relationship to navigate to related resources. For example, the user-messages relationship enables traversal from an Azure Active Directory (Azure AD) User to a set of Outlook mail messages. The following example shows how to do this in a REST API call.</span></span>


```no-highlight
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


<span data-ttu-id="3515a-151">成功响应返回“200 正常”状态和有效负载，如下所示。</span><span class="sxs-lookup"><span data-stu-id="3515a-151">The successful response returns the 200 OK status and a payload, as shown.</span></span>


```no-highlight
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
<span data-ttu-id="3515a-152">通过转到元数据、查找 `EntityType`，并查看该 `EntityType` 的每个 `NavigationProperty`，可以查看给定资源上的所有关系。</span><span class="sxs-lookup"><span data-stu-id="3515a-152">You can see all the relationships on a given resource by going to the metadata, finding the EntityType, and looking at all NavigationProperties for that EntityType.</span></span>

## <a name="call-actions-and-functions"></a><span data-ttu-id="3515a-153">调用操作和函数</span><span class="sxs-lookup"><span data-stu-id="3515a-153">Call actions or functions</span></span>
<span data-ttu-id="3515a-154">Microsoft Graph 还支持_操作_和_函数_以并不仅仅是创建、读取、更新和删除 (CRUD) 操作的方式来操作资源。</span><span class="sxs-lookup"><span data-stu-id="3515a-154">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not simply create, read, update, and delete (CRUD) operations.</span></span> <span data-ttu-id="3515a-155">它们通常采用 HTTPS POST 请求的形式以便输入操作或函数参数。</span><span class="sxs-lookup"><span data-stu-id="3515a-155">They are often in the shape of HTTPS POST requests in order to intake arguments for the action or function.</span></span> <span data-ttu-id="3515a-156">例如，以下操作允许已登录用户 (`me`) 发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3515a-156">For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>

```no-highlight
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

<span data-ttu-id="3515a-p112">你可以查看元数据中可用的全部功能。它们显示为函数或操作。</span><span class="sxs-lookup"><span data-stu-id="3515a-p112">You can see all the functions that are available in the metadata. They appear as Functions or Actions.</span></span>

## <a name="use-the-microsoft-graph-sdks"></a><span data-ttu-id="3515a-159">使用 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="3515a-159">Use the Microsoft Graph SDKs</span></span>

<span data-ttu-id="3515a-p113">喜欢 SDK 的强大功能和易用性吗？虽然你可以随时使用 REST API 调用 Microsoft Graph，但我们还提供了适用于许多常用平台的 SDK。要研究可用的 SDK，请参阅[代码示例和 SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)。</span><span class="sxs-lookup"><span data-stu-id="3515a-p113">Like the power and ease of SDKs? While you can always use REST APIs to call Microsoft Graph, we also provide SDKs for many popular platforms. To explore the SDKs that are available, see [Code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>

## <a name="see-also"></a><span data-ttu-id="3515a-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3515a-163">See also</span></span>

- [<span data-ttu-id="3515a-164">使用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="3515a-164">Use the Microsoft Graph API</span></span>](use-the-api.md)
- [<span data-ttu-id="3515a-165">获取身份验证令牌</span><span class="sxs-lookup"><span data-stu-id="3515a-165">Get auth tokens</span></span>](/graph/auth)
