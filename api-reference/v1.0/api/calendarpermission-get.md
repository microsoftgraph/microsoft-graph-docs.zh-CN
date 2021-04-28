---
title: 获取 calendarPermission
description: 获取 calendarpermission 对象的属性和关系。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4bfbf5fa07b0eb3ad61ceeb60572f229ba872617
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051618"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="b6157-103">获取 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="b6157-103">Get calendarPermission</span></span>

<span data-ttu-id="b6157-104">获取已共享的用户或组日历的指定 permissions 对象。</span><span class="sxs-lookup"><span data-stu-id="b6157-104">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6157-105">权限</span><span class="sxs-lookup"><span data-stu-id="b6157-105">Permissions</span></span>

<span data-ttu-id="b6157-106">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b6157-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="b6157-107">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6157-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6157-108">日历</span><span class="sxs-lookup"><span data-stu-id="b6157-108">Calendar</span></span> | <span data-ttu-id="b6157-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6157-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b6157-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6157-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6157-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6157-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="b6157-112">用户日历</span><span class="sxs-lookup"><span data-stu-id="b6157-112">user calendar</span></span> | <span data-ttu-id="b6157-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6157-113">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b6157-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6157-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b6157-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6157-115">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="b6157-116">组日历</span><span class="sxs-lookup"><span data-stu-id="b6157-116">group calendar</span></span> | <span data-ttu-id="b6157-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6157-117">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="b6157-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6157-118">Not supported.</span></span> | <span data-ttu-id="b6157-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6157-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6157-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6157-120">HTTP request</span></span>

<span data-ttu-id="b6157-121">获取用户的主日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="b6157-121">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b6157-122">获取组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="b6157-122">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b6157-123">获取包含已标识事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="b6157-123">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6157-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b6157-124">Optional query parameters</span></span>

<span data-ttu-id="b6157-125">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b6157-125">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b6157-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b6157-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6157-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6157-127">Request headers</span></span>

| <span data-ttu-id="b6157-128">名称</span><span class="sxs-lookup"><span data-stu-id="b6157-128">Name</span></span>      |<span data-ttu-id="b6157-129">说明</span><span class="sxs-lookup"><span data-stu-id="b6157-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6157-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6157-130">Authorization</span></span> | <span data-ttu-id="b6157-131">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b6157-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6157-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6157-132">Request body</span></span>

<span data-ttu-id="b6157-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6157-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6157-134">响应</span><span class="sxs-lookup"><span data-stu-id="b6157-134">Response</span></span>

<span data-ttu-id="b6157-135">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [calendarPermission](../resources/calendarpermission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6157-135">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6157-136">示例</span><span class="sxs-lookup"><span data-stu-id="b6157-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6157-137">请求</span><span class="sxs-lookup"><span data-stu-id="b6157-137">Request</span></span>

<span data-ttu-id="b6157-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b6157-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6157-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6157-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="b6157-140">C#</span><span class="sxs-lookup"><span data-stu-id="b6157-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6157-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6157-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6157-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6157-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6157-143">Java</span><span class="sxs-lookup"><span data-stu-id="b6157-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6157-144">响应</span><span class="sxs-lookup"><span data-stu-id="b6157-144">Response</span></span>

<span data-ttu-id="b6157-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b6157-145">The following is an example of the response.</span></span>

> <span data-ttu-id="b6157-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b6157-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

