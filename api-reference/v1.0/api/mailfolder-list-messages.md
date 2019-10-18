---
title: 列出邮件
description: 获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b57766a9b8aa756e2d198f0f2358827006c1b455
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728697"
---
# <a name="list-messages"></a><span data-ttu-id="96a24-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="96a24-103">List messages</span></span>

<span data-ttu-id="96a24-104">获取已指定用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="96a24-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="96a24-105">权限</span><span class="sxs-lookup"><span data-stu-id="96a24-105">Permissions</span></span>
<span data-ttu-id="96a24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96a24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96a24-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="96a24-108">Permission type</span></span>      | <span data-ttu-id="96a24-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96a24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96a24-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96a24-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96a24-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96a24-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="96a24-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96a24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96a24-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96a24-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="96a24-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="96a24-114">Application</span></span> | <span data-ttu-id="96a24-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96a24-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96a24-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96a24-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96a24-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96a24-117">Optional query parameters</span></span>
<span data-ttu-id="96a24-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96a24-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96a24-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96a24-119">Request headers</span></span>
| <span data-ttu-id="96a24-120">名称</span><span class="sxs-lookup"><span data-stu-id="96a24-120">Name</span></span>       | <span data-ttu-id="96a24-121">类型</span><span class="sxs-lookup"><span data-stu-id="96a24-121">Type</span></span> | <span data-ttu-id="96a24-122">说明</span><span class="sxs-lookup"><span data-stu-id="96a24-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96a24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96a24-123">Authorization</span></span>  | <span data-ttu-id="96a24-124">string</span><span class="sxs-lookup"><span data-stu-id="96a24-124">string</span></span>  | <span data-ttu-id="96a24-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96a24-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96a24-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="96a24-127">Request body</span></span>
<span data-ttu-id="96a24-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96a24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96a24-129">响应</span><span class="sxs-lookup"><span data-stu-id="96a24-129">Response</span></span>

<span data-ttu-id="96a24-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Message](../resources/message.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96a24-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96a24-131">示例</span><span class="sxs-lookup"><span data-stu-id="96a24-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96a24-132">请求</span><span class="sxs-lookup"><span data-stu-id="96a24-132">Request</span></span>
<span data-ttu-id="96a24-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96a24-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96a24-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96a24-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96a24-135">C#</span><span class="sxs-lookup"><span data-stu-id="96a24-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96a24-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96a24-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96a24-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96a24-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96a24-138">Java</span><span class="sxs-lookup"><span data-stu-id="96a24-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96a24-139">响应</span><span class="sxs-lookup"><span data-stu-id="96a24-139">Response</span></span>
<span data-ttu-id="96a24-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96a24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
