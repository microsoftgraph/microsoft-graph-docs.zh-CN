---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: angelgolfer-ms
ms.openlocfilehash: 57545b89adc5cbb3c20ab782de04438b7b5ba9bf
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771798"
---
# <a name="list-attachments"></a><span data-ttu-id="9984e-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="9984e-103">List attachments</span></span>

> <span data-ttu-id="9984e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9984e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9984e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9984e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9984e-106">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9984e-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="9984e-107">权限</span><span class="sxs-lookup"><span data-stu-id="9984e-107">Permissions</span></span>

<span data-ttu-id="9984e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9984e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9984e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9984e-110">Permission type</span></span>      | <span data-ttu-id="9984e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9984e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9984e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9984e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9984e-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9984e-113">Calendars.Read</span></span>    |
|<span data-ttu-id="9984e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9984e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9984e-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9984e-115">Calendars.Read</span></span>    |
|<span data-ttu-id="9984e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9984e-116">Application</span></span> | <span data-ttu-id="9984e-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9984e-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9984e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9984e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="9984e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9984e-119">Optional query parameters</span></span>

<span data-ttu-id="9984e-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9984e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9984e-121">具体而言，您可以使用`$expand`查询参数来包含所有事件附件内嵌与事件属性的其余部分。</span><span class="sxs-lookup"><span data-stu-id="9984e-121">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="9984e-122">例如：</span><span class="sxs-lookup"><span data-stu-id="9984e-122">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="9984e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9984e-123">Request headers</span></span>

| <span data-ttu-id="9984e-124">名称</span><span class="sxs-lookup"><span data-stu-id="9984e-124">Name</span></span>       | <span data-ttu-id="9984e-125">类型</span><span class="sxs-lookup"><span data-stu-id="9984e-125">Type</span></span> | <span data-ttu-id="9984e-126">说明</span><span class="sxs-lookup"><span data-stu-id="9984e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9984e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9984e-127">Authorization</span></span>  | <span data-ttu-id="9984e-128">string</span><span class="sxs-lookup"><span data-stu-id="9984e-128">string</span></span>  | <span data-ttu-id="9984e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9984e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9984e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9984e-131">Request body</span></span>

<span data-ttu-id="9984e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9984e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9984e-133">响应</span><span class="sxs-lookup"><span data-stu-id="9984e-133">Response</span></span>

<span data-ttu-id="9984e-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9984e-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9984e-135">示例</span><span class="sxs-lookup"><span data-stu-id="9984e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="9984e-136">请求</span><span class="sxs-lookup"><span data-stu-id="9984e-136">Request</span></span>

<span data-ttu-id="9984e-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9984e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="9984e-138">响应</span><span class="sxs-lookup"><span data-stu-id="9984e-138">Response</span></span>

<span data-ttu-id="9984e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9984e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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