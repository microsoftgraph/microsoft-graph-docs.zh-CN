---
title: 创建 CalendarGroup
description: 使用此 API 创建新的 CalendarGroup。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ddf26be745f22ca9ef98fb4949005b17d332e2cc
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107484"
---
# <a name="create-calendargroup"></a><span data-ttu-id="c1ca5-103">创建 CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="c1ca5-103">Create CalendarGroup</span></span>

<span data-ttu-id="c1ca5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1ca5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1ca5-105">使用此 API 创建新的 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1ca5-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1ca5-106">Permissions</span></span>
<span data-ttu-id="c1ca5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ca5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1ca5-109">Permission type</span></span>      | <span data-ttu-id="c1ca5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1ca5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1ca5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ca5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1ca5-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1ca5-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c1ca5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ca5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1ca5-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1ca5-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c1ca5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1ca5-115">Application</span></span> | <span data-ttu-id="c1ca5-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1ca5-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1ca5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1ca5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="c1ca5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1ca5-118">Request headers</span></span>
| <span data-ttu-id="c1ca5-119">标头</span><span class="sxs-lookup"><span data-stu-id="c1ca5-119">Header</span></span>       | <span data-ttu-id="c1ca5-120">值</span><span class="sxs-lookup"><span data-stu-id="c1ca5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1ca5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1ca5-121">Authorization</span></span>  | <span data-ttu-id="c1ca5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1ca5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1ca5-124">Content-Type</span></span>  | <span data-ttu-id="c1ca5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ca5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1ca5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1ca5-126">Request body</span></span>
<span data-ttu-id="c1ca5-127">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c1ca5-128">响应</span><span class="sxs-lookup"><span data-stu-id="c1ca5-128">Response</span></span>

<span data-ttu-id="c1ca5-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ca5-130">示例</span><span class="sxs-lookup"><span data-stu-id="c1ca5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1ca5-131">请求</span><span class="sxs-lookup"><span data-stu-id="c1ca5-131">Request</span></span>
<span data-ttu-id="c1ca5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1ca5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1ca5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c1ca5-134">C#</span><span class="sxs-lookup"><span data-stu-id="c1ca5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1ca5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1ca5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1ca5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1ca5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c1ca5-137">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-137">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c1ca5-138">响应</span><span class="sxs-lookup"><span data-stu-id="c1ca5-138">Response</span></span>
<span data-ttu-id="c1ca5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1ca5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
