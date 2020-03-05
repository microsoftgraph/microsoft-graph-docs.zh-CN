---
title: 获取 calendarPermission
description: 获取 calendarpermission 对象的属性和关系。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8481cecf256d9cd85f9c444f0550ea7c43d37d0b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440897"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="d0b40-103">获取 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="d0b40-103">Get calendarPermission</span></span>

<span data-ttu-id="d0b40-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d0b40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0b40-105">获取已共享的用户或组日历的指定权限对象。</span><span class="sxs-lookup"><span data-stu-id="d0b40-105">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0b40-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0b40-106">Permissions</span></span>

<span data-ttu-id="d0b40-107">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d0b40-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="d0b40-108">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0b40-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0b40-109">日历</span><span class="sxs-lookup"><span data-stu-id="d0b40-109">Calendar</span></span> | <span data-ttu-id="d0b40-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0b40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0b40-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0b40-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0b40-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0b40-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="d0b40-113">用户日历</span><span class="sxs-lookup"><span data-stu-id="d0b40-113">user calendar</span></span> | <span data-ttu-id="d0b40-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0b40-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d0b40-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0b40-115">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d0b40-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0b40-116">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="d0b40-117">组日历</span><span class="sxs-lookup"><span data-stu-id="d0b40-117">group calendar</span></span> | <span data-ttu-id="d0b40-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b40-118">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="d0b40-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0b40-119">Not supported.</span></span> | <span data-ttu-id="d0b40-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0b40-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0b40-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0b40-121">HTTP request</span></span>

<span data-ttu-id="d0b40-122">获取用户的主日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="d0b40-122">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="d0b40-123">获取组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="d0b40-123">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="d0b40-124">获取包含标识的事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="d0b40-124">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0b40-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d0b40-125">Optional query parameters</span></span>

<span data-ttu-id="d0b40-126">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d0b40-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d0b40-127">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d0b40-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0b40-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0b40-128">Request headers</span></span>

| <span data-ttu-id="d0b40-129">名称</span><span class="sxs-lookup"><span data-stu-id="d0b40-129">Name</span></span>      |<span data-ttu-id="d0b40-130">说明</span><span class="sxs-lookup"><span data-stu-id="d0b40-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0b40-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0b40-131">Authorization</span></span> | <span data-ttu-id="d0b40-132">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d0b40-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0b40-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0b40-133">Request body</span></span>

<span data-ttu-id="d0b40-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0b40-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0b40-135">响应</span><span class="sxs-lookup"><span data-stu-id="d0b40-135">Response</span></span>

<span data-ttu-id="d0b40-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[calendarPermission](../resources/calendarpermission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0b40-136">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0b40-137">示例</span><span class="sxs-lookup"><span data-stu-id="d0b40-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0b40-138">请求</span><span class="sxs-lookup"><span data-stu-id="d0b40-138">Request</span></span>

<span data-ttu-id="d0b40-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d0b40-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0b40-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0b40-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="d0b40-141">C#</span><span class="sxs-lookup"><span data-stu-id="d0b40-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0b40-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0b40-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0b40-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0b40-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0b40-144">响应</span><span class="sxs-lookup"><span data-stu-id="d0b40-144">Response</span></span>

<span data-ttu-id="d0b40-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d0b40-145">The following is an example of the response.</span></span>

> <span data-ttu-id="d0b40-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d0b40-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
