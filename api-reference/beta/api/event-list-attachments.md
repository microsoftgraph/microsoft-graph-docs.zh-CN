---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: deb9ea49ef058f95fc6023c3f2a45c2fc919f9e6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326539"
---
# <a name="list-attachments"></a><span data-ttu-id="8f572-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="8f572-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f572-104">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8f572-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f572-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f572-105">Permissions</span></span>

<span data-ttu-id="8f572-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f572-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f572-108">Permission type</span></span>      | <span data-ttu-id="8f572-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f572-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f572-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f572-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f572-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f572-111">Calendars.Read</span></span>    |
|<span data-ttu-id="8f572-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f572-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f572-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f572-113">Calendars.Read</span></span>    |
|<span data-ttu-id="8f572-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f572-114">Application</span></span> | <span data-ttu-id="8f572-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f572-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f572-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f572-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="8f572-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8f572-117">Optional query parameters</span></span>

<span data-ttu-id="8f572-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8f572-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8f572-119">特别是, 您可以使用`$expand`查询参数将所有事件附件与其余事件属性一起包含在内联中。</span><span class="sxs-lookup"><span data-stu-id="8f572-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="8f572-120">例如：</span><span class="sxs-lookup"><span data-stu-id="8f572-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="8f572-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f572-121">Request headers</span></span>

| <span data-ttu-id="8f572-122">名称</span><span class="sxs-lookup"><span data-stu-id="8f572-122">Name</span></span>       | <span data-ttu-id="8f572-123">类型</span><span class="sxs-lookup"><span data-stu-id="8f572-123">Type</span></span> | <span data-ttu-id="8f572-124">说明</span><span class="sxs-lookup"><span data-stu-id="8f572-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f572-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f572-125">Authorization</span></span>  | <span data-ttu-id="8f572-126">string</span><span class="sxs-lookup"><span data-stu-id="8f572-126">string</span></span>  | <span data-ttu-id="8f572-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f572-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f572-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f572-129">Request body</span></span>

<span data-ttu-id="8f572-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f572-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f572-131">响应</span><span class="sxs-lookup"><span data-stu-id="8f572-131">Response</span></span>

<span data-ttu-id="8f572-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8f572-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f572-133">示例</span><span class="sxs-lookup"><span data-stu-id="8f572-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f572-134">请求</span><span class="sxs-lookup"><span data-stu-id="8f572-134">Request</span></span>

<span data-ttu-id="8f572-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f572-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f572-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8f572-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f572-137">C#</span><span class="sxs-lookup"><span data-stu-id="8f572-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f572-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f572-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f572-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="8f572-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f572-140">Java</span><span class="sxs-lookup"><span data-stu-id="8f572-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f572-141">响应</span><span class="sxs-lookup"><span data-stu-id="8f572-141">Response</span></span>

<span data-ttu-id="8f572-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f572-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
