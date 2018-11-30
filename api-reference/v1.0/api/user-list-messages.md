---
title: List messages
description: 获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。
ms.openlocfilehash: 861d56850a8a4a4a167540b221bd94b7b8e62ae0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007766"
---
# <a name="list-messages"></a><span data-ttu-id="a0567-103">List messages</span><span class="sxs-lookup"><span data-stu-id="a0567-103">List messages</span></span>

<span data-ttu-id="a0567-104">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="a0567-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="a0567-105">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="a0567-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="a0567-106">有两种应用程序，另一个用户的邮件文件夹中收到消息的情况：</span><span class="sxs-lookup"><span data-stu-id="a0567-106">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="a0567-107">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="a0567-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a0567-108">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享邮件文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="a0567-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a0567-109">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="a0567-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0567-110">权限</span><span class="sxs-lookup"><span data-stu-id="a0567-110">Permissions</span></span>
<span data-ttu-id="a0567-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0567-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0567-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0567-113">Permission type</span></span>      | <span data-ttu-id="a0567-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0567-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0567-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0567-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a0567-116">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0567-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a0567-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0567-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0567-118">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0567-118">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a0567-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0567-119">Application</span></span> | <span data-ttu-id="a0567-120">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0567-120">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0567-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0567-121">HTTP request</span></span>

<span data-ttu-id="a0567-122">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a0567-122">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="a0567-123">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a0567-123">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0567-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0567-124">Optional query parameters</span></span>
<span data-ttu-id="a0567-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0567-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a0567-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0567-126">Request headers</span></span>
| <span data-ttu-id="a0567-127">名称</span><span class="sxs-lookup"><span data-stu-id="a0567-127">Name</span></span>       | <span data-ttu-id="a0567-128">类型</span><span class="sxs-lookup"><span data-stu-id="a0567-128">Type</span></span> | <span data-ttu-id="a0567-129">说明</span><span class="sxs-lookup"><span data-stu-id="a0567-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a0567-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0567-130">Authorization</span></span>  | <span data-ttu-id="a0567-131">string</span><span class="sxs-lookup"><span data-stu-id="a0567-131">string</span></span>  | <span data-ttu-id="a0567-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0567-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0567-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a0567-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a0567-135">string</span><span class="sxs-lookup"><span data-stu-id="a0567-135">string</span></span> | <span data-ttu-id="a0567-136">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="a0567-136">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="a0567-137">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="a0567-137">Values can be "text" or "html".</span></span> <span data-ttu-id="a0567-138">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="a0567-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="a0567-139">可选。</span><span class="sxs-lookup"><span data-stu-id="a0567-139">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a0567-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0567-140">Request body</span></span>
<span data-ttu-id="a0567-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0567-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0567-142">响应</span><span class="sxs-lookup"><span data-stu-id="a0567-142">Response</span></span>

<span data-ttu-id="a0567-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0567-143">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="a0567-144">此请求的默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="a0567-144">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="a0567-145">示例</span><span class="sxs-lookup"><span data-stu-id="a0567-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0567-146">请求</span><span class="sxs-lookup"><span data-stu-id="a0567-146">Request</span></span>
<span data-ttu-id="a0567-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0567-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="a0567-148">响应</span><span class="sxs-lookup"><span data-stu-id="a0567-148">Response</span></span>
<span data-ttu-id="a0567-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0567-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
