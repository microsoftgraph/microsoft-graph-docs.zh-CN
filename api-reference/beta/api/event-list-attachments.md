---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 744ba1c0ab88afa2acf38f93b58cd01592504af4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43365444"
---
# <a name="list-attachments"></a><span data-ttu-id="01977-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="01977-103">List attachments</span></span>

<span data-ttu-id="01977-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01977-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01977-105">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="01977-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="01977-106">权限</span><span class="sxs-lookup"><span data-stu-id="01977-106">Permissions</span></span>

<span data-ttu-id="01977-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01977-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="01977-109">Permission type</span></span>      | <span data-ttu-id="01977-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01977-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01977-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01977-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01977-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01977-112">Calendars.Read</span></span>    |
|<span data-ttu-id="01977-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01977-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01977-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01977-114">Calendars.Read</span></span>    |
|<span data-ttu-id="01977-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="01977-115">Application</span></span> | <span data-ttu-id="01977-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01977-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="01977-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01977-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="01977-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01977-118">Optional query parameters</span></span>

<span data-ttu-id="01977-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01977-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="01977-120">特别是，您可以使用`$expand`查询参数将所有事件附件与其余事件属性一起包含在内联中。</span><span class="sxs-lookup"><span data-stu-id="01977-120">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="01977-121">例如：</span><span class="sxs-lookup"><span data-stu-id="01977-121">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="01977-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="01977-122">Request headers</span></span>

| <span data-ttu-id="01977-123">名称</span><span class="sxs-lookup"><span data-stu-id="01977-123">Name</span></span>       | <span data-ttu-id="01977-124">类型</span><span class="sxs-lookup"><span data-stu-id="01977-124">Type</span></span> | <span data-ttu-id="01977-125">说明</span><span class="sxs-lookup"><span data-stu-id="01977-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01977-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="01977-126">Authorization</span></span>  | <span data-ttu-id="01977-127">string</span><span class="sxs-lookup"><span data-stu-id="01977-127">string</span></span>  | <span data-ttu-id="01977-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01977-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01977-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="01977-130">Request body</span></span>

<span data-ttu-id="01977-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01977-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01977-132">响应</span><span class="sxs-lookup"><span data-stu-id="01977-132">Response</span></span>

<span data-ttu-id="01977-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="01977-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01977-134">示例</span><span class="sxs-lookup"><span data-stu-id="01977-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="01977-135">请求</span><span class="sxs-lookup"><span data-stu-id="01977-135">Request</span></span>

<span data-ttu-id="01977-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01977-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01977-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="01977-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="01977-138">C#</span><span class="sxs-lookup"><span data-stu-id="01977-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01977-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01977-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01977-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01977-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01977-141">响应</span><span class="sxs-lookup"><span data-stu-id="01977-141">Response</span></span>

<span data-ttu-id="01977-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01977-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
