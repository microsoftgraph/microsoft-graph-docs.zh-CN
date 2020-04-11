---
title: 更新 calendarpermission
description: 更新 calendarpermission 对象的属性。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b990b038960a97eb8ba8e86d6a338cebe4339fbb
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227779"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="fb426-103">更新 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="fb426-103">Update calendarPermission</span></span>

<span data-ttu-id="fb426-104">通过日历的相应[calendarPermission](../resources/calendarpermission.md)对象更新分配给现有 sharee 或代理的权限。</span><span class="sxs-lookup"><span data-stu-id="fb426-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb426-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb426-105">Permissions</span></span>

<span data-ttu-id="fb426-106">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="fb426-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="fb426-107">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb426-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb426-108">日历</span><span class="sxs-lookup"><span data-stu-id="fb426-108">Calendar</span></span> | <span data-ttu-id="fb426-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb426-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fb426-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb426-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb426-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb426-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="fb426-112">用户日历</span><span class="sxs-lookup"><span data-stu-id="fb426-112">user calendar</span></span> | <span data-ttu-id="fb426-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb426-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="fb426-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb426-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="fb426-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb426-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="fb426-116">组日历</span><span class="sxs-lookup"><span data-stu-id="fb426-116">group calendar</span></span> | <span data-ttu-id="fb426-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb426-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="fb426-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb426-118">Not supported.</span></span> | <span data-ttu-id="fb426-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb426-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb426-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb426-120">HTTP request</span></span>

<span data-ttu-id="fb426-121">更新用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="fb426-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="fb426-122">更新组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="fb426-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="fb426-123">更新包含已标识事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="fb426-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb426-124">请求头</span><span class="sxs-lookup"><span data-stu-id="fb426-124">Request headers</span></span>

| <span data-ttu-id="fb426-125">名称</span><span class="sxs-lookup"><span data-stu-id="fb426-125">Name</span></span>       | <span data-ttu-id="fb426-126">说明</span><span class="sxs-lookup"><span data-stu-id="fb426-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fb426-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb426-127">Authorization</span></span> | <span data-ttu-id="fb426-128">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fb426-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb426-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb426-129">Request body</span></span>

<span data-ttu-id="fb426-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="fb426-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="fb426-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="fb426-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fb426-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fb426-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fb426-133">属性</span><span class="sxs-lookup"><span data-stu-id="fb426-133">Property</span></span>     | <span data-ttu-id="fb426-134">类型</span><span class="sxs-lookup"><span data-stu-id="fb426-134">Type</span></span>        | <span data-ttu-id="fb426-135">说明</span><span class="sxs-lookup"><span data-stu-id="fb426-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb426-136">role</span><span class="sxs-lookup"><span data-stu-id="fb426-136">role</span></span>|[<span data-ttu-id="fb426-137">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="fb426-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="fb426-138">为日历 sharee 或代理人更改的权限级别。</span><span class="sxs-lookup"><span data-stu-id="fb426-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="fb426-139">响应</span><span class="sxs-lookup"><span data-stu-id="fb426-139">Response</span></span>

<span data-ttu-id="fb426-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[calendarPermission](../resources/calendarpermission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb426-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb426-141">示例</span><span class="sxs-lookup"><span data-stu-id="fb426-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb426-142">请求</span><span class="sxs-lookup"><span data-stu-id="fb426-142">Request</span></span>

<span data-ttu-id="fb426-143">下面的示例将 sharee、Adele、的权限级别更改为`write`。</span><span class="sxs-lookup"><span data-stu-id="fb426-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```

### <a name="response"></a><span data-ttu-id="fb426-144">响应</span><span class="sxs-lookup"><span data-stu-id="fb426-144">Response</span></span>

<span data-ttu-id="fb426-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb426-145">The following is an example of the response.</span></span>

> <span data-ttu-id="fb426-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fb426-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
