---
title: 列出附件
description: 检索附加到邮件的 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 964e822c5f66dc53390c8aa11bc288e81a7ad01a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992918"
---
# <a name="list-attachments"></a><span data-ttu-id="65804-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="65804-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65804-104">检索附加到邮件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="65804-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="65804-105">权限</span><span class="sxs-lookup"><span data-stu-id="65804-105">Permissions</span></span>
<span data-ttu-id="65804-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65804-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="65804-108">Permission type</span></span>      | <span data-ttu-id="65804-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65804-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65804-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65804-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65804-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="65804-111">Mail.Read</span></span>    |
|<span data-ttu-id="65804-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65804-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65804-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="65804-113">Mail.Read</span></span>    |
|<span data-ttu-id="65804-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="65804-114">Application</span></span> | <span data-ttu-id="65804-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="65804-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="65804-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65804-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="65804-117">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="65804-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="65804-118">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="65804-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="65804-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="65804-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65804-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="65804-121">Optional query parameters</span></span>
<span data-ttu-id="65804-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="65804-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="65804-123">特别是, 您可以使用 $expand 查询参数将所有邮件附件嵌入到其余邮件属性中。</span><span class="sxs-lookup"><span data-stu-id="65804-123">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="65804-124">例如：</span><span class="sxs-lookup"><span data-stu-id="65804-124">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="65804-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="65804-125">Request headers</span></span>
| <span data-ttu-id="65804-126">名称</span><span class="sxs-lookup"><span data-stu-id="65804-126">Name</span></span>       | <span data-ttu-id="65804-127">类型</span><span class="sxs-lookup"><span data-stu-id="65804-127">Type</span></span> | <span data-ttu-id="65804-128">说明</span><span class="sxs-lookup"><span data-stu-id="65804-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65804-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="65804-129">Authorization</span></span>  | <span data-ttu-id="65804-130">string</span><span class="sxs-lookup"><span data-stu-id="65804-130">string</span></span>  | <span data-ttu-id="65804-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65804-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65804-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="65804-133">Request body</span></span>
<span data-ttu-id="65804-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65804-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65804-135">响应</span><span class="sxs-lookup"><span data-stu-id="65804-135">Response</span></span>

<span data-ttu-id="65804-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="65804-136">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65804-137">示例</span><span class="sxs-lookup"><span data-stu-id="65804-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65804-138">请求</span><span class="sxs-lookup"><span data-stu-id="65804-138">Request</span></span>
<span data-ttu-id="65804-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65804-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65804-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="65804-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65804-141">C#</span><span class="sxs-lookup"><span data-stu-id="65804-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65804-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="65804-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65804-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="65804-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65804-144">Java</span><span class="sxs-lookup"><span data-stu-id="65804-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="65804-145">响应</span><span class="sxs-lookup"><span data-stu-id="65804-145">Response</span></span>
<span data-ttu-id="65804-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65804-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
