---
title: List messages
description: '获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 19cb2dc1dd1e86cd697319a0dc8a729cb712e463
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792186"
---
# <a name="list-messages"></a><span data-ttu-id="80905-103">List messages</span><span class="sxs-lookup"><span data-stu-id="80905-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80905-104">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="80905-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="80905-105">从邮箱中获取邮件可能会导致多个请求, 具体取决于页面大小和邮箱数据。</span><span class="sxs-lookup"><span data-stu-id="80905-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="80905-106">默认的页面大小为10封邮件。</span><span class="sxs-lookup"><span data-stu-id="80905-106">The default page size is 10 messages.</span></span> <span data-ttu-id="80905-107">若要获取下一页邮件, 只需将返回的整个 URL 应用`@odata.nextLink`到下一个消息获取请求。</span><span class="sxs-lookup"><span data-stu-id="80905-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="80905-108">此 URL 包括您在初始请求中可能指定的任何查询参数。</span><span class="sxs-lookup"><span data-stu-id="80905-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="80905-109">请勿尝试从`@odata.nextLink` URL 中提取`$skip`值来处理响应。</span><span class="sxs-lookup"><span data-stu-id="80905-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="80905-110">此 API 使用`$skip`值来保留它在用户邮箱中已有的所有项的计数, 以返回邮件类型项的页面。</span><span class="sxs-lookup"><span data-stu-id="80905-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="80905-111">因此, 即使在初始响应中, `$skip`该值也会大于页面大小。</span><span class="sxs-lookup"><span data-stu-id="80905-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="80905-112">有关详细信息, 请参阅[在应用中分页 Microsoft Graph 数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="80905-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="80905-113">您可以对邮件进行筛选, 并只获取那些包含已[](../resources/mention.md)登录用户的说明。</span><span class="sxs-lookup"><span data-stu-id="80905-113">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="80905-114">请注意, 默认情况下`GET /me/messages` , 该操作不会返回**提及**属性。</span><span class="sxs-lookup"><span data-stu-id="80905-114">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="80905-115">使用`$expand`查询参数[在邮件中查找每个提及的详细信息](../api/message-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="80905-115">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="80905-116">在以下两种情况下, 应用可以在其他用户的邮件文件夹中获取邮件:</span><span class="sxs-lookup"><span data-stu-id="80905-116">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="80905-117">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="80905-117">If the app has application permissions, or,</span></span>
* <span data-ttu-id="80905-118">如果应用程序具有来自一个用户的相应委派权限, 而另一个用户与该用户共享了一个邮件文件夹, 或者, 已向该用户授予了对该用户的委派访问[权限](#permissions)。</span><span class="sxs-lookup"><span data-stu-id="80905-118">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="80905-119">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="80905-119">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="80905-120">权限</span><span class="sxs-lookup"><span data-stu-id="80905-120">Permissions</span></span>
<span data-ttu-id="80905-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80905-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80905-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="80905-123">Permission type</span></span>      | <span data-ttu-id="80905-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80905-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80905-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80905-125">Delegated (work or school account)</span></span> | <span data-ttu-id="80905-126">user.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="80905-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="80905-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80905-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80905-128">user.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="80905-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="80905-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="80905-129">Application</span></span> | <span data-ttu-id="80905-130">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80905-130">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="80905-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80905-131">HTTP request</span></span>

<span data-ttu-id="80905-132">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="80905-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="80905-133">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="80905-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="80905-134">若要获取用户邮箱中包含用户**提及**的所有邮件, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="80905-134">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80905-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80905-135">Optional query parameters</span></span>
<span data-ttu-id="80905-136">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80905-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="80905-137">您可以使用`$filter` **mentionsPreview**属性上的查询参数来获取那些提及已登录用户的消息。</span><span class="sxs-lookup"><span data-stu-id="80905-137">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80905-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="80905-138">Request headers</span></span>
| <span data-ttu-id="80905-139">名称</span><span class="sxs-lookup"><span data-stu-id="80905-139">Name</span></span>       | <span data-ttu-id="80905-140">类型</span><span class="sxs-lookup"><span data-stu-id="80905-140">Type</span></span> | <span data-ttu-id="80905-141">说明</span><span class="sxs-lookup"><span data-stu-id="80905-141">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80905-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="80905-142">Authorization</span></span>  | <span data-ttu-id="80905-143">string</span><span class="sxs-lookup"><span data-stu-id="80905-143">string</span></span>  | <span data-ttu-id="80905-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80905-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80905-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="80905-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="80905-147">string</span><span class="sxs-lookup"><span data-stu-id="80905-147">string</span></span> | <span data-ttu-id="80905-148">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="80905-148">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="80905-149">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="80905-149">Values can be "text" or "html".</span></span> <span data-ttu-id="80905-150">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="80905-150">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="80905-151">可选。</span><span class="sxs-lookup"><span data-stu-id="80905-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80905-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="80905-152">Request body</span></span>
<span data-ttu-id="80905-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80905-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80905-154">响应</span><span class="sxs-lookup"><span data-stu-id="80905-154">Response</span></span>

<span data-ttu-id="80905-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[message](../resources/message.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="80905-155">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80905-156">示例</span><span class="sxs-lookup"><span data-stu-id="80905-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="80905-157">请求 1</span><span class="sxs-lookup"><span data-stu-id="80905-157">Request 1</span></span>
<span data-ttu-id="80905-158">第一个示例获取已登录用户的邮箱中的默认前10封邮件。</span><span class="sxs-lookup"><span data-stu-id="80905-158">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="80905-159">它使用`$select`返回响应中每个邮件的属性子集。</span><span class="sxs-lookup"><span data-stu-id="80905-159">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
##### <a name="response-1"></a><span data-ttu-id="80905-160">响应 1</span><span class="sxs-lookup"><span data-stu-id="80905-160">Response 1</span></span>
<span data-ttu-id="80905-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="80905-161">Here is an example of the response.</span></span> <span data-ttu-id="80905-162">若要获取下一页邮件, 请将返回`@odata.nextLink`的 URL 应用于后续的 get 请求。</span><span class="sxs-lookup"><span data-stu-id="80905-162">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/messages?$select=sender%2csubject&$skip=14",
    "value": [
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
            "id": "AAMkAGUAAAwTW09AAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D1e\"",
            "id": "AAMkAGUAAAq5QKlAAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D0v\"",
            "id": "AAMkAGUAAAq5QKkAAA=",
            "subject": "Your Azure AD Identity Protection Weekly Digest",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Azure",
                    "address": "azure-noreply@microsoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DsN\"",
            "id": "AAMkAGUAAAq5QKjAAA=",
            "subject": "Use attached file",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq9\"",
            "id": "AAMkAGUAAAq5QKiAAA=",
            "subject": "Original invitation",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq1\"",
            "id": "AAMkAGUAAAq5QKhAAA=",
            "subject": "Koala image",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dqp\"",
            "id": "AAMkAGUAAAq5QKgAAA=",
            "subject": "Sales invoice template",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessageRequest",
            "@odata.etag": "W/\"CwAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dfa\"",
            "id": "AAMkAGUAAAq5T8tAAA=",
            "subject": "Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="80905-163">请求 2</span><span class="sxs-lookup"><span data-stu-id="80905-163">Request 2</span></span>
<span data-ttu-id="80905-164">下一个示例将对登录用户邮箱中的所有邮件进行筛选, 以查找那些提及该用户的邮件。</span><span class="sxs-lookup"><span data-stu-id="80905-164">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="80905-165">它还`$select`用于在响应中返回每个邮件的属性子集。</span><span class="sxs-lookup"><span data-stu-id="80905-165">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="80905-166">该示例还合并了查询参数字符串中的空格字符的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="80905-166">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="80905-167">响应 2</span><span class="sxs-lookup"><span data-stu-id="80905-167">Response 2</span></span>
<span data-ttu-id="80905-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80905-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="80905-171">请求 3</span><span class="sxs-lookup"><span data-stu-id="80905-171">Request 3</span></span>
<span data-ttu-id="80905-172">第三个示例演示如何使用`Prefer: outlook.body-content-type="text"`标头以文本格式获取每个邮件的**body**和**uniqueBody**属性。</span><span class="sxs-lookup"><span data-stu-id="80905-172">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="80905-173">响应 3</span><span class="sxs-lookup"><span data-stu-id="80905-173">Response 3</span></span>
<span data-ttu-id="80905-174">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="80905-174">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
