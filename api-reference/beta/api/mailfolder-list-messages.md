---
title: 列出邮件
description: 列出已登录用户的邮箱中的所有邮件，或邮箱或驱动器中指定文件夹中的邮件。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4dbad3f465091828b718c8467a5b6e75356f7eee
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049259"
---
# <a name="list-messages"></a><span data-ttu-id="602a2-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="602a2-103">List messages</span></span>

<span data-ttu-id="602a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="602a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="602a2-105">列出指定用户的邮箱中的所有邮件，或邮箱中指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="602a2-105">List all the messages in the specified user's mailbox, or those messages in a specified folder in the mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="602a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="602a2-106">Permissions</span></span>
<span data-ttu-id="602a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="602a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="602a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="602a2-109">Permission type</span></span>      | <span data-ttu-id="602a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="602a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="602a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="602a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="602a2-112">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602a2-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="602a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="602a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="602a2-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602a2-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="602a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="602a2-115">Application</span></span> | <span data-ttu-id="602a2-116">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602a2-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="602a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="602a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="602a2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="602a2-118">Optional query parameters</span></span>
<span data-ttu-id="602a2-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="602a2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="602a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="602a2-120">Request headers</span></span>
| <span data-ttu-id="602a2-121">名称</span><span class="sxs-lookup"><span data-stu-id="602a2-121">Name</span></span>       | <span data-ttu-id="602a2-122">类型</span><span class="sxs-lookup"><span data-stu-id="602a2-122">Type</span></span> | <span data-ttu-id="602a2-123">说明</span><span class="sxs-lookup"><span data-stu-id="602a2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="602a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="602a2-124">Authorization</span></span>  | <span data-ttu-id="602a2-125">string</span><span class="sxs-lookup"><span data-stu-id="602a2-125">string</span></span>  | <span data-ttu-id="602a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="602a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="602a2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="602a2-128">Request body</span></span>
<span data-ttu-id="602a2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="602a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="602a2-130">响应</span><span class="sxs-lookup"><span data-stu-id="602a2-130">Response</span></span>
<span data-ttu-id="602a2-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Message](../resources/message.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="602a2-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="602a2-132">示例</span><span class="sxs-lookup"><span data-stu-id="602a2-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="602a2-133">请求</span><span class="sxs-lookup"><span data-stu-id="602a2-133">Request</span></span>
<span data-ttu-id="602a2-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="602a2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="602a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="602a2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/messages
```
# <a name="c"></a>[<span data-ttu-id="602a2-136">C#</span><span class="sxs-lookup"><span data-stu-id="602a2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="602a2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="602a2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="602a2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="602a2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="602a2-139">Java</span><span class="sxs-lookup"><span data-stu-id="602a2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="602a2-140">响应</span><span class="sxs-lookup"><span data-stu-id="602a2-140">Response</span></span>
<span data-ttu-id="602a2-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="602a2-141">The following is an example of the response.</span></span>
><span data-ttu-id="602a2-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="602a2-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "id": "AAMkAGVmMDEzK",
      "createdDateTime": "2018-02-13T03:53:55Z",
      "lastModifiedDateTime": "2018-02-13T03:53:55Z",
      "changeKey": "CQAAABYAAAAiIsqMbYjsT5e/T7KzowPTAACB/CZh",
      "categories": [],
      "receivedDateTime": "2018-02-13T03:53:55Z",
      "sentDateTime": "2018-02-13T03:53:55Z",
      "hasAttachments": false,
      "internetMessageId": "<DM5PR1501MB2117E943C78792608769840ECDF60@DM5PR1501MB2117.namprd15.prod.outlook.com>",
      "subject": "MyAnalytics | Your past week",
      "bodyPreview": "February 4-10, 2018\r\n\r\n\r\nHi Megan Bowen,\r\n\r\nWe've got your highlights from last week\r\n\r\n\r\n\r\nYour time\r\n\r\n\r\nEmail hours\r\n\r\n\r\n\r\n\r\n0 hrs\r\n\r\n\r\n\r\nMeeting hours\r\n\r\n\r\n\r\n\r\n12 hrs\r\n\r\n\r\n\r\n\r\nFocus hours\r\n\r\n\r\n\r\n\r\n30 hrs\r\n\r\n\r\n\r\n\r\n\r\nGoals keep you motivated. Set them",
      "importance": "normal",
      "parentFolderId": "AAMkAGVmMDEzM",
      "conversationId": "AAQkAGVmMDEzE",
      "conversationIndex": "AQHTpH5EZfLlhf/DnUK56FDP+qUfcQ==",
      "isDeliveryReceiptRequested": false,
      "isReadReceiptRequested": false,
      "isRead": false,
      "isDraft": false,
      "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGVmMDEzK&exvsurl=1&viewmodel=ReadMessageItem",
      "inferenceClassification": "other",
      "unsubscribeData": [],
      "unsubscribeEnabled": false,
      "body": {
          "contentType": "html",
          "content": "<html lang=\"en\">\r\n<head></head>\r\n<body> </body>\r\n</html>\r\n"
      },
      "sender": {
          "emailAddress": {
              "name": "MyAnalytics",
              "address": "no-reply@contoso.com"
          }
      },
      "from": {
          "emailAddress": {
              "name": "MyAnalytics",
              "address": "no-reply@contoso.com"
          }
      },
      "toRecipients": [
          {
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.com"
              }
          }
      ],
      "ccRecipients": [],
      "bccRecipients": [],
      "replyTo": [],
      "mentionsPreview": null,
      "flag": {
          "flagStatus": "notFlagged"
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
  ]
}
-->


