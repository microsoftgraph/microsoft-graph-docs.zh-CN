---
title: 列出事件
description: 检索事件对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 78142046858656d343295badcebf511120d1a647
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858449"
---
# <a name="list-events"></a><span data-ttu-id="4e6a4-103">列出事件</span><span class="sxs-lookup"><span data-stu-id="4e6a4-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6a4-104">检索 [event](../resources/event.md) 对象列表.</span><span class="sxs-lookup"><span data-stu-id="4e6a4-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e6a4-105">权限</span><span class="sxs-lookup"><span data-stu-id="4e6a4-105">Permissions</span></span>
<span data-ttu-id="4e6a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e6a4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e6a4-108">Permission type</span></span>      | <span data-ttu-id="4e6a4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e6a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e6a4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e6a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e6a4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e6a4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e6a4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e6a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e6a4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-113">Not supported.</span></span>    |
|<span data-ttu-id="4e6a4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e6a4-114">Application</span></span> | <span data-ttu-id="4e6a4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e6a4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e6a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e6a4-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4e6a4-117">Optional query parameters</span></span>
<span data-ttu-id="4e6a4-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e6a4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e6a4-119">Request headers</span></span>
| <span data-ttu-id="4e6a4-120">名称</span><span class="sxs-lookup"><span data-stu-id="4e6a4-120">Name</span></span>       | <span data-ttu-id="4e6a4-121">类型</span><span class="sxs-lookup"><span data-stu-id="4e6a4-121">Type</span></span> | <span data-ttu-id="4e6a4-122">说明</span><span class="sxs-lookup"><span data-stu-id="4e6a4-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="4e6a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e6a4-123">Authorization</span></span>  | <span data-ttu-id="4e6a4-124">string</span><span class="sxs-lookup"><span data-stu-id="4e6a4-124">string</span></span> | <span data-ttu-id="4e6a4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e6a4-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="4e6a4-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="4e6a4-128">string</span><span class="sxs-lookup"><span data-stu-id="4e6a4-128">string</span></span> | <span data-ttu-id="4e6a4-129">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="4e6a4-130">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="4e6a4-131">可选。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-131">Optional.</span></span> |
| <span data-ttu-id="4e6a4-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="4e6a4-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="4e6a4-133">string</span><span class="sxs-lookup"><span data-stu-id="4e6a4-133">string</span></span> | <span data-ttu-id="4e6a4-134">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="4e6a4-135">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-135">Values can be "text" or "html".</span></span> <span data-ttu-id="4e6a4-136">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="4e6a4-137">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="4e6a4-138">可选。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e6a4-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e6a4-139">Request body</span></span>
<span data-ttu-id="4e6a4-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e6a4-141">响应</span><span class="sxs-lookup"><span data-stu-id="4e6a4-141">Response</span></span>
<span data-ttu-id="4e6a4-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e6a4-143">示例</span><span class="sxs-lookup"><span data-stu-id="4e6a4-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4e6a4-144">请求</span><span class="sxs-lookup"><span data-stu-id="4e6a4-144">Request</span></span>
<span data-ttu-id="4e6a4-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e6a4-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4e6a4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e6a4-147">C#</span><span class="sxs-lookup"><span data-stu-id="4e6a4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e6a4-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="4e6a4-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e6a4-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="4e6a4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4e6a4-150">Java</span><span class="sxs-lookup"><span data-stu-id="4e6a4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e6a4-151">响应</span><span class="sxs-lookup"><span data-stu-id="4e6a4-151">Response</span></span>
<span data-ttu-id="4e6a4-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-152">The following is an example of the response.</span></span>
><span data-ttu-id="4e6a4-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4e6a4-154">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4e6a4-154">All the properties will be returned from an actual call.</span></span>
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
