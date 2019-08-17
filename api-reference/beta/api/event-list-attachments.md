---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: edfe7b8eec63109df19ca8d1997fce4799db85a6
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453132"
---
# <a name="list-attachments"></a><span data-ttu-id="3b87d-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="3b87d-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b87d-104">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="3b87d-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b87d-105">权限</span><span class="sxs-lookup"><span data-stu-id="3b87d-105">Permissions</span></span>

<span data-ttu-id="3b87d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b87d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b87d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b87d-108">Permission type</span></span>      | <span data-ttu-id="3b87d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b87d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b87d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b87d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b87d-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3b87d-111">Calendars.Read</span></span>    |
|<span data-ttu-id="3b87d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b87d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b87d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3b87d-113">Calendars.Read</span></span>    |
|<span data-ttu-id="3b87d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b87d-114">Application</span></span> | <span data-ttu-id="3b87d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3b87d-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b87d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b87d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="3b87d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3b87d-117">Optional query parameters</span></span>

<span data-ttu-id="3b87d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3b87d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3b87d-119">特别是, 您可以使用`$expand`查询参数将所有事件附件与其余事件属性一起包含在内联中。</span><span class="sxs-lookup"><span data-stu-id="3b87d-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="3b87d-120">例如：</span><span class="sxs-lookup"><span data-stu-id="3b87d-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="3b87d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b87d-121">Request headers</span></span>

| <span data-ttu-id="3b87d-122">名称</span><span class="sxs-lookup"><span data-stu-id="3b87d-122">Name</span></span>       | <span data-ttu-id="3b87d-123">类型</span><span class="sxs-lookup"><span data-stu-id="3b87d-123">Type</span></span> | <span data-ttu-id="3b87d-124">说明</span><span class="sxs-lookup"><span data-stu-id="3b87d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b87d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b87d-125">Authorization</span></span>  | <span data-ttu-id="3b87d-126">string</span><span class="sxs-lookup"><span data-stu-id="3b87d-126">string</span></span>  | <span data-ttu-id="3b87d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b87d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b87d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b87d-129">Request body</span></span>

<span data-ttu-id="3b87d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b87d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b87d-131">响应</span><span class="sxs-lookup"><span data-stu-id="3b87d-131">Response</span></span>

<span data-ttu-id="3b87d-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3b87d-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b87d-133">示例</span><span class="sxs-lookup"><span data-stu-id="3b87d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b87d-134">请求</span><span class="sxs-lookup"><span data-stu-id="3b87d-134">Request</span></span>

<span data-ttu-id="3b87d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b87d-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3b87d-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3b87d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b87d-137">C#</span><span class="sxs-lookup"><span data-stu-id="3b87d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b87d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b87d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b87d-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="3b87d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3b87d-140">响应</span><span class="sxs-lookup"><span data-stu-id="3b87d-140">Response</span></span>

<span data-ttu-id="3b87d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b87d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_get_attachments_beta",
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
      "@odata.type":"#microsoft.graph.fileAttachment",
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
