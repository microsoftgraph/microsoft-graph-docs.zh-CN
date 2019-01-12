---
title: 调用 Microsoft Graph API
description: '若要访问和操纵 Microsoft Graph 资源，请使用以下一项操作来调用和指定资源 URL：   '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 627fb614f8084abe6980ed095a7a55adfa6a3f12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970414"
---
# <a name="calling-the-microsoft-graph-api"></a><span data-ttu-id="6e1a9-103">调用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="6e1a9-103">Calling the Microsoft Graph API</span></span>

<span data-ttu-id="6e1a9-104">若要访问和操纵 Microsoft Graph 资源，请使用以下一项操作来调用和指定资源 URL。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-104">To access and manipulate a Microsoft Graph resource, you call and specify the resource URLs using one of the following operations:</span></span>   

- <span data-ttu-id="6e1a9-105">GET</span><span class="sxs-lookup"><span data-stu-id="6e1a9-105">GET</span></span>
- <span data-ttu-id="6e1a9-106">POST</span><span class="sxs-lookup"><span data-stu-id="6e1a9-106">POST</span></span>
- <span data-ttu-id="6e1a9-107">PATCH</span><span class="sxs-lookup"><span data-stu-id="6e1a9-107">PATCH</span></span>
- <span data-ttu-id="6e1a9-108">PUT</span><span class="sxs-lookup"><span data-stu-id="6e1a9-108">PUT</span></span>
- <span data-ttu-id="6e1a9-109">DELETE</span><span class="sxs-lookup"><span data-stu-id="6e1a9-109">DELETE</span></span> 

<span data-ttu-id="6e1a9-110">所有 Microsoft Graph API 请求均使用下列基 URL 模式：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-110">All Microsoft Graph API requests use the following basic URL pattern:</span></span>

```
    https://graph.microsoft.com/{version}/{resource}?[query_parameters]
```

<span data-ttu-id="6e1a9-111">对于此 URL：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-111">For this URL:</span></span>

- <span data-ttu-id="6e1a9-112">`https://graph.microsoft.com` 是 Microsoft Graph API 终结点。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-112">`https://graph.microsoft.com` is the Microsoft Graph API endpoint.</span></span>
- <span data-ttu-id="6e1a9-113">`{version}` 是目标服务版本（例如 `v1.0` 或 `beta`）。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-113">`{version}` is the target service version, for example, `v1.0` or `beta`.</span></span>
- <span data-ttu-id="6e1a9-114">`{resource}` 是资源段或路径，如：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-114">`{resource}` is resource segment or path, such as:</span></span>
  - <span data-ttu-id="6e1a9-115">`users`, `groups`, `devices`, `organization`</span><span class="sxs-lookup"><span data-stu-id="6e1a9-115">`users`, `groups`, `devices`, `organization`</span></span>
  - <span data-ttu-id="6e1a9-116">解析为登录用户的别名 `me`</span><span class="sxs-lookup"><span data-stu-id="6e1a9-116">The alias `me`, which resolves to the signed-in user</span></span>
   - <span data-ttu-id="6e1a9-117">属于用户的资源（如 `me/events`、`me/drive` 或 `me/messages`）</span><span class="sxs-lookup"><span data-stu-id="6e1a9-117">The resources belonging to a user, such as `me/events`, `me/drive` or `me/messages`</span></span>
  - <span data-ttu-id="6e1a9-118">解析为登录用户所属组织的租户的别名 `myOrganization`</span><span class="sxs-lookup"><span data-stu-id="6e1a9-118">The alias `myOrganization`, which resolves to the tenant of the organization signed-in user</span></span>
- <span data-ttu-id="6e1a9-119">`[query_parameters]` 表示其他查询参数，例如 `$filter` 和 `$select`。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-119">`[query_parameters]` represents additional query parameters such as `$filter` and `$select`.</span></span>

<span data-ttu-id="6e1a9-p101">或者，也可以将租户指定为请求的一部分。使用 `me` 时，请勿指定租户。有关常见请求的列表，请参阅 [Microsoft Graph 概述](overview.md)。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p101">Optionally, you can also specify the tenant as part of your request. When using `me`, do not specify the tenant. For a list of common requests, see [Overview of Microsoft Graph](overview.md).</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="6e1a9-123">Microsoft Graph API 元数据</span><span class="sxs-lookup"><span data-stu-id="6e1a9-123">Microsoft Graph API metadata</span></span>
<span data-ttu-id="6e1a9-p102">元数据文档 ($metadata) 在服务根处发布。例如，可以通过以下 URL 查看 v1.0 和试用版的服务文档。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p102">The metadata document ($metadata) is published at the service root. For example, you can view the service document for the v1.0 and beta versions via the following URLs.</span></span>

<span data-ttu-id="6e1a9-126">Microsoft Graph API `v1.0` 元数据。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-126">Microsoft Graph API `v1.0` metadata.</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```
<span data-ttu-id="6e1a9-127">Microsoft Graph API `beta` 元数据。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-127">Microsoft Graph API `beta` metadata.</span></span>
```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="6e1a9-128">元数据允许你查看并了解 Microsoft Graph 的数据模型，包括实体类型和集、复杂类型、组成请求的枚举以及发送到和发送自 Microsoft Graph 的响应数据包。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-128">The metadata allows you to see and understand the data model of Microsoft Graph, including the entity types and sets, complex types, and enums that make up the request and response packets sent to and from Microsoft Graph.</span></span>
<span data-ttu-id="6e1a9-129">可以使用元数据了解 Microsoft Graph 中实体之间的关系，并建立可在实体导航的 URL。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-129">You can use the metadata to understand the realtionships between entities in Microsoft Graph and establish URLs that navigate between entities.</span></span>
<span data-ttu-id="6e1a9-130">此基于导航的相互联系为 Microsoft Graph 提供了唯一的字符。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-130">This navigation-based interconnectedness gives Microsoft Graph its unique character.</span></span>

<span data-ttu-id="6e1a9-131">路径 URL 资源名称、查询参数，以及操作参数和值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-131">Path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span> <span data-ttu-id="6e1a9-132">不过，分配的值、实体 ID 和其他 base64 编码的值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-132">However, values you assign, entity IDs, and other base64-encoded values are case-sensitive.</span></span>

<span data-ttu-id="6e1a9-133">以下部分介绍了几个对 Microsoft Graph API 的基本编程模式调用。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-133">The following sections show a few basic programming pattern calls to the Microsoft Graph API.</span></span>

## <a name="navigate-from-a-set-to-a-member"></a><span data-ttu-id="6e1a9-134">从集导航至成员</span><span class="sxs-lookup"><span data-stu-id="6e1a9-134">Navigate from a set to a member</span></span>

<span data-ttu-id="6e1a9-p105">若要查看用户相关信息，可以使用一个 HTTPS GET 请求从 `users` 集合至标识符标识的指定用户获取 `User` 实体。对于 `User` 实体，可以将 `id` 或 `userPrincipalName` 属性用作标识符。以下示例请求使用 `userPrincipalName` 值作为用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p105">To view the information about a user, you get the `User` entity from the `users` collection to the specific user identified by its identifier, using an HTTPS GET request. For a `User` entity, either the `id` or `userPrincipalName` property can be used as the identifier. The following example request uses the `userPrincipalName` value as the user's id.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="6e1a9-138">如果成功，应该会收到 200 OK 响应，其中包含有效负载中的用户资源声明，如下所示：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-138">If successful, you should get a 200 OK response containing the user resource representation in the payload, as shown as follows:</span></span>

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


## <a name="project-from-an-entity-to-properties"></a><span data-ttu-id="6e1a9-139">从一个实体投影至属性</span><span class="sxs-lookup"><span data-stu-id="6e1a9-139">Project from an entity to properties</span></span>
<span data-ttu-id="6e1a9-140">若要仅检索用户的传记数据（如用户提供的_本人简介_描述和技能集），则可以在上一个请求中添加 _select_ 查询参数。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-140">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the _select_ query parameter to the previous request.</span></span>
<span data-ttu-id="6e1a9-141">例如：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-141">For example:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="6e1a9-142">成功的响应返回 200 OK 状态，以及具有如下格式的有效负载：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-142">The successful response returns the 200 OK status and a payload of the following format:</span></span>

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

<span data-ttu-id="6e1a9-143">此时，仅返回 `user`、`aboutMe` 和 `displayName` 属性（而不是 `skills` 实体上的整个属性集）。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-143">Here, instead of the entire property sets on the `user` entity, only the `aboutMe`, `displayName`, and `skills` properties are returned.</span></span>

## <a name="traverse-to-another-resource-via-relationship"></a><span data-ttu-id="6e1a9-144">通过关系遍历到其他资源</span><span class="sxs-lookup"><span data-stu-id="6e1a9-144">Traverse to another resource via relationship</span></span>
<span data-ttu-id="6e1a9-p107">经理与向其报告的其他用户保持 `directReports` 关系。若要查询用户的直接下属列表，则你可以使用以下 HTTPS GET 请求，通过关系遍历，导航到预期目标。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p107">A manager holds a `directReports` relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="6e1a9-147">成功的响应返回 200 OK 状态，以及具有如下格式的有效负载：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-147">The successful response returns the 200 OK status and a payload of the following format:</span></span>

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

<span data-ttu-id="6e1a9-p108">同样地，可以根据关系导航至相关资源。例如，借助 `user => messages` 关系，可以从 Azure AD 用户遍历到 Outlook 邮件集。下面的示例显示如何在 REST API 调用中执行此操作：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p108">Similarly, you can follow a relationship to navigate to related resources. For example, the `user => messages` relationship enables traversal from an Azure AD User to a set of Outlook mail messages. The following example shows how to do this in a REST API call:</span></span>


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
<span data-ttu-id="6e1a9-151">成功的响应返回 200 OK 状态，以及具有如下格式的有效负载：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-151">The successful response returns the 200 OK status and a payload of the following format:</span></span>


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

## <a name="project-from-entities-to-properties"></a><span data-ttu-id="6e1a9-152">从多个实体投影至属性</span><span class="sxs-lookup"><span data-stu-id="6e1a9-152">Project from entities to properties</span></span>
<span data-ttu-id="6e1a9-p109">除了能从一个实体投影至其属性之外，您还可以将类似的 `select` 查询选项应用于实体集合，以便将它们投影至其一些属性的集合。例如，若要查询登录用户的驱动器项目名称，则您可以提交以下 HTTPS GET 请求：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p109">In addition to projection from a single entity to its properties, you can also apply the similar `select` query option to an entity collection to project them to a collection of some of their properties. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="6e1a9-155">成功的响应返回 200 OK 状态代码，以及包含共享文件的名称和类型的有效负载，如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-155">The successful response returns a 200 OK status code and a payload containing the names and types of the shared files, as shown in the following example:</span></span>

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

## <a name="query-a-subset-of-users-with-the-filtering-query-option"></a><span data-ttu-id="6e1a9-156">使用筛选查询选项查询用户子集</span><span class="sxs-lookup"><span data-stu-id="6e1a9-156">Query a subset of users with the filtering query option</span></span>
<span data-ttu-id="6e1a9-p110">要查找组织中指定工作头衔的员工，可以从用户集合中导航，然后指定一个 _filter_ 查询选项。一个示例如下所示：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p110">To find the employees of a specific job title within an organization, you can navigate from the users collection and then specify a _filter_ query option. An example is shown as follows:</span></span>

    
```no-highlight 
GET https://graph.microsoft.com/v1.0/users/?$filter=jobTitle+eq+%27Helper%27 HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="6e1a9-159">成功的响应返回 200 OK 状态代码，以及担任特定职务 (`'Helper'`) 的用户列表，如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-159">The successful response returns the 200 OK status code and a list of users with the specified job title (`'Helper'`), as shown in the following example:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
odata-version: 4.0
content-length: 986

{
    "@odata.context": "https://graph.microsoft.com/v1.0/contoso.onmicrosoft.com/$metadata#users",
    "value": [
        {
            "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
            "city": "Redmond",
            "country": "USA",
            "department": "Help Center",
            "displayName": "Jane Doe",
            "givenName": "Jane",
            "jobTitle": "Helper",
            ......
            "mailNickname": "Jane",
            "mobile": null,
            "otherMails": [
                "jane.doe@contoso.onmicrosoft.com"
            ],
            ......
            "surname": "Doe",
            "usageLocation": "US",
            "userPrincipalName": "help@contoso.onmicrosoft.com",
            "userType": "Member"
        },
        
        ...
    ]
}
```

## <a name="call-actions-or-functions"></a><span data-ttu-id="6e1a9-160">调用操作或函数</span><span class="sxs-lookup"><span data-stu-id="6e1a9-160">Call actions or functions</span></span>
<span data-ttu-id="6e1a9-161">Microsoft Graph 还支持_操作_和_函数_，以并非简单符合标准 HTTP 方法的方式操作资源。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-161">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not a simple fit with standard HTTP methods.</span></span> <span data-ttu-id="6e1a9-162">例如，以下 HTTPS POST 请求允许登录用户 (`me`) 发送电子邮件：</span><span class="sxs-lookup"><span data-stu-id="6e1a9-162">For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>
```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
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
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
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

<span data-ttu-id="6e1a9-163">请求有效负载中包含对 `sendMail` 操作的输入（$metadata 中也对此进行了定义）。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-163">The request payload contains the input to the `sendMail` action, which is also defined in the $metadata.</span></span>

## <a name="use-microsoft-graph-client-libraries"></a><span data-ttu-id="6e1a9-164">使用 Microsoft Graph 客户端库</span><span class="sxs-lookup"><span data-stu-id="6e1a9-164">Use Microsoft Graph client libraries</span></span>
<span data-ttu-id="6e1a9-p112">喜欢 SDK 的强大功能和易用性吗？虽然你可以随时使用 REST API 调用 Microsoft Graph，但我们还提供了适用于许多常用平台的 SDK。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-p112">Like the power and ease of SDKs? While you can always call Microsoft Graph using the REST API, we also provide SDKs for many popular platforms.</span></span>

<span data-ttu-id="6e1a9-167">浏览[代码示例和 SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)。</span><span class="sxs-lookup"><span data-stu-id="6e1a9-167">Explore our [code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
