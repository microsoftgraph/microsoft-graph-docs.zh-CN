---
title: 列出事件
description: 检索 event 对象列表。
author: dkershaw10
ms.openlocfilehash: fdb996f9be5193c5f18e6adb7de0b16938221e58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355543"
---
# <a name="list-events"></a><span data-ttu-id="3ab1b-103">列出事件</span><span class="sxs-lookup"><span data-stu-id="3ab1b-103">List events</span></span>

> <span data-ttu-id="3ab1b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ab1b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ab1b-106">检索 [event](../resources/event.md) 对象列表.</span><span class="sxs-lookup"><span data-stu-id="3ab1b-106">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ab1b-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ab1b-107">Permissions</span></span>
<span data-ttu-id="3ab1b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ab1b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ab1b-110">Permission type</span></span>      | <span data-ttu-id="3ab1b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ab1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ab1b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ab1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ab1b-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ab1b-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ab1b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ab1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ab1b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-115">Not supported.</span></span>    |
|<span data-ttu-id="3ab1b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ab1b-116">Application</span></span> | <span data-ttu-id="3ab1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ab1b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ab1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ab1b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ab1b-119">Optional query parameters</span></span>
<span data-ttu-id="3ab1b-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ab1b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ab1b-121">Request headers</span></span>
| <span data-ttu-id="3ab1b-122">Name</span><span class="sxs-lookup"><span data-stu-id="3ab1b-122">Name</span></span>       | <span data-ttu-id="3ab1b-123">类型</span><span class="sxs-lookup"><span data-stu-id="3ab1b-123">Type</span></span> | <span data-ttu-id="3ab1b-124">说明</span><span class="sxs-lookup"><span data-stu-id="3ab1b-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="3ab1b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ab1b-125">Authorization</span></span>  | <span data-ttu-id="3ab1b-126">string</span><span class="sxs-lookup"><span data-stu-id="3ab1b-126">string</span></span> | <span data-ttu-id="3ab1b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ab1b-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3ab1b-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="3ab1b-130">string</span><span class="sxs-lookup"><span data-stu-id="3ab1b-130">string</span></span> | <span data-ttu-id="3ab1b-131">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="3ab1b-132">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="3ab1b-133">可选。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-133">Optional.</span></span> |
| <span data-ttu-id="3ab1b-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="3ab1b-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="3ab1b-135">string</span><span class="sxs-lookup"><span data-stu-id="3ab1b-135">string</span></span> | <span data-ttu-id="3ab1b-136">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="3ab1b-137">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-137">Values can be "text" or "html".</span></span> <span data-ttu-id="3ab1b-138">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="3ab1b-139">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="3ab1b-140">可选。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ab1b-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ab1b-141">Request body</span></span>
<span data-ttu-id="3ab1b-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ab1b-143">响应</span><span class="sxs-lookup"><span data-stu-id="3ab1b-143">Response</span></span>
<span data-ttu-id="3ab1b-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-144">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ab1b-145">示例</span><span class="sxs-lookup"><span data-stu-id="3ab1b-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3ab1b-146">请求</span><span class="sxs-lookup"><span data-stu-id="3ab1b-146">Request</span></span>
<span data-ttu-id="3ab1b-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="3ab1b-148">响应</span><span class="sxs-lookup"><span data-stu-id="3ab1b-148">Response</span></span>
<span data-ttu-id="3ab1b-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-149">The following is an example of the response.</span></span>
><span data-ttu-id="3ab1b-150">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ab1b-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ab1b-151">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
