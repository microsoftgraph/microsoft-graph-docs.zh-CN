---
title: 列出附件
description: 检索附加到邮件的 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 584b01114f22466673568d991c824a94c6d73dd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983481"
---
# <a name="list-attachments"></a><span data-ttu-id="cbc6c-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="cbc6c-103">List attachments</span></span>

> <span data-ttu-id="cbc6c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbc6c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbc6c-106">检索附加到邮件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbc6c-107">权限</span><span class="sxs-lookup"><span data-stu-id="cbc6c-107">Permissions</span></span>
<span data-ttu-id="cbc6c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbc6c-110">Permission type</span></span>      | <span data-ttu-id="cbc6c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cbc6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbc6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbc6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cbc6c-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbc6c-113">Mail.Read</span></span>    |
|<span data-ttu-id="cbc6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbc6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbc6c-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbc6c-115">Mail.Read</span></span>    |
|<span data-ttu-id="cbc6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbc6c-116">Application</span></span> | <span data-ttu-id="cbc6c-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbc6c-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbc6c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbc6c-118">HTTP request</span></span>
<span data-ttu-id="cbc6c-119"><!-- { "blockType": "ignored" } -->[邮件](../resources/message.md)用户的邮箱中的附件。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-119"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="cbc6c-120">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-120">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="cbc6c-p103">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cbc6c-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cbc6c-123">Optional query parameters</span></span>
<span data-ttu-id="cbc6c-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cbc6c-125">具体而言，您可以使用 $展开查询参数，包括所有与邮件属性的其余部分内联邮件附件。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-125">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="cbc6c-126">例如：</span><span class="sxs-lookup"><span data-stu-id="cbc6c-126">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="cbc6c-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbc6c-127">Request headers</span></span>
| <span data-ttu-id="cbc6c-128">名称</span><span class="sxs-lookup"><span data-stu-id="cbc6c-128">Name</span></span>       | <span data-ttu-id="cbc6c-129">类型</span><span class="sxs-lookup"><span data-stu-id="cbc6c-129">Type</span></span> | <span data-ttu-id="cbc6c-130">说明</span><span class="sxs-lookup"><span data-stu-id="cbc6c-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cbc6c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbc6c-131">Authorization</span></span>  | <span data-ttu-id="cbc6c-132">string</span><span class="sxs-lookup"><span data-stu-id="cbc6c-132">string</span></span>  | <span data-ttu-id="cbc6c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbc6c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbc6c-135">Request body</span></span>
<span data-ttu-id="cbc6c-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbc6c-137">响应</span><span class="sxs-lookup"><span data-stu-id="cbc6c-137">Response</span></span>

<span data-ttu-id="cbc6c-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-138">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbc6c-139">示例</span><span class="sxs-lookup"><span data-stu-id="cbc6c-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbc6c-140">请求</span><span class="sxs-lookup"><span data-stu-id="cbc6c-140">Request</span></span>
<span data-ttu-id="cbc6c-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="cbc6c-142">响应</span><span class="sxs-lookup"><span data-stu-id="cbc6c-142">Response</span></span>
<span data-ttu-id="cbc6c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbc6c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
