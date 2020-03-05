---
title: 列出事件
description: 检索事件对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a8ff2621089214d30b9b7aa8d06c069312f3c6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419602"
---
# <a name="list-events"></a><span data-ttu-id="e2b31-103">列出事件</span><span class="sxs-lookup"><span data-stu-id="e2b31-103">List events</span></span>

<span data-ttu-id="e2b31-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e2b31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2b31-105">检索 [event](../resources/event.md) 对象列表.</span><span class="sxs-lookup"><span data-stu-id="e2b31-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2b31-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2b31-106">Permissions</span></span>
<span data-ttu-id="e2b31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2b31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2b31-109">Permission type</span></span>      | <span data-ttu-id="e2b31-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2b31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2b31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2b31-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b31-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2b31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2b31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2b31-114">Not supported.</span></span>    |
|<span data-ttu-id="e2b31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2b31-115">Application</span></span> | <span data-ttu-id="e2b31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2b31-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2b31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2b31-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2b31-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2b31-118">Optional query parameters</span></span>
<span data-ttu-id="e2b31-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2b31-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2b31-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2b31-120">Request headers</span></span>
| <span data-ttu-id="e2b31-121">名称</span><span class="sxs-lookup"><span data-stu-id="e2b31-121">Name</span></span>       | <span data-ttu-id="e2b31-122">类型</span><span class="sxs-lookup"><span data-stu-id="e2b31-122">Type</span></span> | <span data-ttu-id="e2b31-123">说明</span><span class="sxs-lookup"><span data-stu-id="e2b31-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e2b31-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b31-124">Authorization</span></span>  | <span data-ttu-id="e2b31-125">字符串</span><span class="sxs-lookup"><span data-stu-id="e2b31-125">string</span></span> | <span data-ttu-id="e2b31-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2b31-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2b31-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e2b31-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e2b31-129">string</span><span class="sxs-lookup"><span data-stu-id="e2b31-129">string</span></span> | <span data-ttu-id="e2b31-130">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="e2b31-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e2b31-131">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e2b31-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e2b31-132">可选。</span><span class="sxs-lookup"><span data-stu-id="e2b31-132">Optional.</span></span> |
| <span data-ttu-id="e2b31-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e2b31-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e2b31-134">string</span><span class="sxs-lookup"><span data-stu-id="e2b31-134">string</span></span> | <span data-ttu-id="e2b31-135">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="e2b31-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="e2b31-136">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="e2b31-136">Values can be "text" or "html".</span></span> <span data-ttu-id="e2b31-137">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="e2b31-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="e2b31-138">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="e2b31-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="e2b31-139">可选。</span><span class="sxs-lookup"><span data-stu-id="e2b31-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2b31-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2b31-140">Request body</span></span>
<span data-ttu-id="e2b31-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2b31-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2b31-142">响应</span><span class="sxs-lookup"><span data-stu-id="e2b31-142">Response</span></span>
<span data-ttu-id="e2b31-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e2b31-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b31-144">示例</span><span class="sxs-lookup"><span data-stu-id="e2b31-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e2b31-145">请求</span><span class="sxs-lookup"><span data-stu-id="e2b31-145">Request</span></span>
<span data-ttu-id="e2b31-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2b31-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2b31-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2b31-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="c"></a>[<span data-ttu-id="e2b31-148">C#</span><span class="sxs-lookup"><span data-stu-id="e2b31-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2b31-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2b31-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2b31-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2b31-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e2b31-151">响应</span><span class="sxs-lookup"><span data-stu-id="e2b31-151">Response</span></span>
<span data-ttu-id="e2b31-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2b31-152">The following is an example of the response.</span></span>
><span data-ttu-id="e2b31-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e2b31-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
