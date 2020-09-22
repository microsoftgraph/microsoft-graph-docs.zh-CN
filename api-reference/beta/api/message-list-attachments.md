---
title: 列出附件
description: 检索附加到邮件的 attachment 对象列表。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 581bd98c47b24ce33508ca60b96612d93b2a3555
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067942"
---
# <a name="list-attachments"></a><span data-ttu-id="c1060-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="c1060-103">List attachments</span></span>

<span data-ttu-id="c1060-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1060-105">检索附加到邮件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="c1060-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1060-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1060-106">Permissions</span></span>
<span data-ttu-id="c1060-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1060-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1060-109">Permission type</span></span>      | <span data-ttu-id="c1060-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1060-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1060-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1060-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1060-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c1060-112">Mail.Read</span></span>    |
|<span data-ttu-id="c1060-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1060-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1060-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c1060-114">Mail.Read</span></span>    |
|<span data-ttu-id="c1060-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1060-115">Application</span></span> | <span data-ttu-id="c1060-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c1060-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1060-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1060-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c1060-118">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c1060-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="c1060-119">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c1060-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="c1060-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="c1060-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1060-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1060-122">Optional query parameters</span></span>
<span data-ttu-id="c1060-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1060-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c1060-124">特别是，您可以使用 $expand 查询参数将所有邮件附件嵌入到其余邮件属性中。</span><span class="sxs-lookup"><span data-stu-id="c1060-124">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="c1060-125">例如：</span><span class="sxs-lookup"><span data-stu-id="c1060-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="c1060-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1060-126">Request headers</span></span>
| <span data-ttu-id="c1060-127">名称</span><span class="sxs-lookup"><span data-stu-id="c1060-127">Name</span></span>       | <span data-ttu-id="c1060-128">类型</span><span class="sxs-lookup"><span data-stu-id="c1060-128">Type</span></span> | <span data-ttu-id="c1060-129">说明</span><span class="sxs-lookup"><span data-stu-id="c1060-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1060-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1060-130">Authorization</span></span>  | <span data-ttu-id="c1060-131">string</span><span class="sxs-lookup"><span data-stu-id="c1060-131">string</span></span>  | <span data-ttu-id="c1060-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1060-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1060-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1060-134">Request body</span></span>
<span data-ttu-id="c1060-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1060-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1060-136">响应</span><span class="sxs-lookup"><span data-stu-id="c1060-136">Response</span></span>

<span data-ttu-id="c1060-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1060-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1060-138">示例</span><span class="sxs-lookup"><span data-stu-id="c1060-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1060-139">请求</span><span class="sxs-lookup"><span data-stu-id="c1060-139">Request</span></span>
<span data-ttu-id="c1060-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1060-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1060-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1060-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="c1060-142">C#</span><span class="sxs-lookup"><span data-stu-id="c1060-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1060-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1060-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1060-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1060-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1060-145">响应</span><span class="sxs-lookup"><span data-stu-id="c1060-145">Response</span></span>
<span data-ttu-id="c1060-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1060-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "message_get_attachments_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
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


