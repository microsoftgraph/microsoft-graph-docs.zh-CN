---
title: 列出邮件
description: 获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0e04715d011d2cb4217c73b7dc234d48f38d56cb
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612465"
---
# <a name="list-messages"></a><span data-ttu-id="8bae9-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="8bae9-103">List messages</span></span>

<span data-ttu-id="8bae9-104">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="8bae9-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bae9-105">权限</span><span class="sxs-lookup"><span data-stu-id="8bae9-105">Permissions</span></span>
<span data-ttu-id="8bae9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bae9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bae9-108">Permission type</span></span>      | <span data-ttu-id="8bae9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bae9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bae9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bae9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bae9-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bae9-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8bae9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bae9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bae9-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bae9-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8bae9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bae9-114">Application</span></span> | <span data-ttu-id="8bae9-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bae9-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bae9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bae9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8bae9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8bae9-117">Optional query parameters</span></span>
<span data-ttu-id="8bae9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8bae9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8bae9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bae9-119">Request headers</span></span>
| <span data-ttu-id="8bae9-120">名称</span><span class="sxs-lookup"><span data-stu-id="8bae9-120">Name</span></span>       | <span data-ttu-id="8bae9-121">类型</span><span class="sxs-lookup"><span data-stu-id="8bae9-121">Type</span></span> | <span data-ttu-id="8bae9-122">说明</span><span class="sxs-lookup"><span data-stu-id="8bae9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8bae9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bae9-123">Authorization</span></span>  | <span data-ttu-id="8bae9-124">string</span><span class="sxs-lookup"><span data-stu-id="8bae9-124">string</span></span>  | <span data-ttu-id="8bae9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bae9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bae9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bae9-127">Request body</span></span>
<span data-ttu-id="8bae9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8bae9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bae9-129">响应</span><span class="sxs-lookup"><span data-stu-id="8bae9-129">Response</span></span>

<span data-ttu-id="8bae9-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Message](../resources/message.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8bae9-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8bae9-131">示例</span><span class="sxs-lookup"><span data-stu-id="8bae9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bae9-132">请求</span><span class="sxs-lookup"><span data-stu-id="8bae9-132">Request</span></span>
<span data-ttu-id="8bae9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8bae9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="8bae9-134">响应</span><span class="sxs-lookup"><span data-stu-id="8bae9-134">Response</span></span>
<span data-ttu-id="8bae9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bae9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8bae9-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8bae9-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8bae9-139">C#</span><span class="sxs-lookup"><span data-stu-id="8bae9-139">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bae9-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="8bae9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
