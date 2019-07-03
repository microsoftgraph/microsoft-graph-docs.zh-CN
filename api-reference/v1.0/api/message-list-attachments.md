---
title: 列出附件
description: 检索附加到邮件的 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6cae690ce030a149dffe03536c6b8d918a6040eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444167"
---
# <a name="list-attachments"></a><span data-ttu-id="c89e7-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="c89e7-103">List attachments</span></span>

<span data-ttu-id="c89e7-104">检索附加到邮件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="c89e7-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="c89e7-105">权限</span><span class="sxs-lookup"><span data-stu-id="c89e7-105">Permissions</span></span>
<span data-ttu-id="c89e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c89e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89e7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c89e7-108">Permission type</span></span>      | <span data-ttu-id="c89e7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c89e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c89e7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c89e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c89e7-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c89e7-111">Mail.Read</span></span>    |
|<span data-ttu-id="c89e7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c89e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c89e7-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c89e7-113">Mail.Read</span></span>    |
|<span data-ttu-id="c89e7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c89e7-114">Application</span></span> | <span data-ttu-id="c89e7-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c89e7-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c89e7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c89e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c89e7-117">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c89e7-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="c89e7-118">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c89e7-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="c89e7-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="c89e7-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c89e7-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c89e7-121">Optional query parameters</span></span>
<span data-ttu-id="c89e7-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c89e7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c89e7-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c89e7-123">Request headers</span></span>
| <span data-ttu-id="c89e7-124">名称</span><span class="sxs-lookup"><span data-stu-id="c89e7-124">Name</span></span>       | <span data-ttu-id="c89e7-125">类型</span><span class="sxs-lookup"><span data-stu-id="c89e7-125">Type</span></span> | <span data-ttu-id="c89e7-126">说明</span><span class="sxs-lookup"><span data-stu-id="c89e7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c89e7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c89e7-127">Authorization</span></span>  | <span data-ttu-id="c89e7-128">string</span><span class="sxs-lookup"><span data-stu-id="c89e7-128">string</span></span>  | <span data-ttu-id="c89e7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c89e7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c89e7-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c89e7-131">Request body</span></span>
<span data-ttu-id="c89e7-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c89e7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c89e7-133">响应</span><span class="sxs-lookup"><span data-stu-id="c89e7-133">Response</span></span>

<span data-ttu-id="c89e7-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c89e7-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c89e7-135">示例</span><span class="sxs-lookup"><span data-stu-id="c89e7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c89e7-136">请求</span><span class="sxs-lookup"><span data-stu-id="c89e7-136">Request</span></span>
<span data-ttu-id="c89e7-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c89e7-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c89e7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c89e7-138">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c89e7-139">C#</span><span class="sxs-lookup"><span data-stu-id="c89e7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c89e7-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c89e7-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c89e7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c89e7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c89e7-142">响应</span><span class="sxs-lookup"><span data-stu-id="c89e7-142">Response</span></span>
<span data-ttu-id="c89e7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c89e7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
