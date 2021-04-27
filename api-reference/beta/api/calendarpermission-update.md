---
title: 更新 calendarpermission
description: 更新 calendarpermission 对象的属性。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116352b351d66bdc2c413eb1aad9357407d25631
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047677"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="d509f-103">更新 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="d509f-103">Update calendarPermission</span></span>

<span data-ttu-id="d509f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d509f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d509f-105">通过日历的相应 [calendarPermission](../resources/calendarpermission.md) 对象更新分配给现有共享者或代理人的权限。</span><span class="sxs-lookup"><span data-stu-id="d509f-105">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="d509f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d509f-106">Permissions</span></span>

<span data-ttu-id="d509f-107">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d509f-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="d509f-108">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d509f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d509f-109">日历</span><span class="sxs-lookup"><span data-stu-id="d509f-109">Calendar</span></span> | <span data-ttu-id="d509f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d509f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d509f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d509f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d509f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d509f-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="d509f-113">用户日历</span><span class="sxs-lookup"><span data-stu-id="d509f-113">user calendar</span></span> | <span data-ttu-id="d509f-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d509f-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="d509f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d509f-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="d509f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d509f-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="d509f-117">组日历</span><span class="sxs-lookup"><span data-stu-id="d509f-117">group calendar</span></span> | <span data-ttu-id="d509f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d509f-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="d509f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d509f-119">Not supported.</span></span> | <span data-ttu-id="d509f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d509f-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d509f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d509f-121">HTTP request</span></span>

<span data-ttu-id="d509f-122">更新用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="d509f-122">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="d509f-123">更新组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="d509f-123">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="d509f-124">更新包含已标识事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="d509f-124">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d509f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d509f-125">Request headers</span></span>

| <span data-ttu-id="d509f-126">名称</span><span class="sxs-lookup"><span data-stu-id="d509f-126">Name</span></span>       | <span data-ttu-id="d509f-127">说明</span><span class="sxs-lookup"><span data-stu-id="d509f-127">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d509f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d509f-128">Authorization</span></span> | <span data-ttu-id="d509f-129">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d509f-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d509f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d509f-130">Request body</span></span>

<span data-ttu-id="d509f-131">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d509f-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d509f-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d509f-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d509f-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d509f-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d509f-134">属性</span><span class="sxs-lookup"><span data-stu-id="d509f-134">Property</span></span>     | <span data-ttu-id="d509f-135">类型</span><span class="sxs-lookup"><span data-stu-id="d509f-135">Type</span></span>        | <span data-ttu-id="d509f-136">说明</span><span class="sxs-lookup"><span data-stu-id="d509f-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d509f-137">role</span><span class="sxs-lookup"><span data-stu-id="d509f-137">role</span></span>|[<span data-ttu-id="d509f-138">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="d509f-138">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="d509f-139">要更改为日历共享者或代理人的权限级别。</span><span class="sxs-lookup"><span data-stu-id="d509f-139">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="d509f-140">响应</span><span class="sxs-lookup"><span data-stu-id="d509f-140">Response</span></span>

<span data-ttu-id="d509f-141">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [calendarPermission](../resources/calendarpermission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d509f-141">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d509f-142">示例</span><span class="sxs-lookup"><span data-stu-id="d509f-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d509f-143">请求</span><span class="sxs-lookup"><span data-stu-id="d509f-143">Request</span></span>

<span data-ttu-id="d509f-144">以下示例将共享者 Adele 的权限级别更改为 `write` 。</span><span class="sxs-lookup"><span data-stu-id="d509f-144">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

# <a name="http"></a>[<span data-ttu-id="d509f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d509f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[<span data-ttu-id="d509f-146">C#</span><span class="sxs-lookup"><span data-stu-id="d509f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d509f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d509f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d509f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d509f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d509f-149">Java</span><span class="sxs-lookup"><span data-stu-id="d509f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d509f-150">响应</span><span class="sxs-lookup"><span data-stu-id="d509f-150">Response</span></span>

<span data-ttu-id="d509f-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d509f-151">The following is an example of the response.</span></span>

> <span data-ttu-id="d509f-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d509f-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "update_calendarpermission",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "L289RXhlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


