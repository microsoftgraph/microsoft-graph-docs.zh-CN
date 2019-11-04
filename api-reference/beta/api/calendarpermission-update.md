---
title: 更新 calendarpermission
description: 更新 calendarpermission 对象的属性。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1cd959c4ee083ff6ec26914c5f99ccd3d8c3c8f
ms.sourcegitcommit: 1a3ca53422fc9a8254e78af7c058e876fc9f9ef8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2019
ms.locfileid: "37942635"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="35565-103">更新 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="35565-103">Update calendarPermission</span></span>

<span data-ttu-id="35565-104">更新 calendarPermission 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35565-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="35565-105">权限</span><span class="sxs-lookup"><span data-stu-id="35565-105">Permissions</span></span>

<span data-ttu-id="35565-106">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="35565-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="35565-107">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35565-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35565-108">日历</span><span class="sxs-lookup"><span data-stu-id="35565-108">Calendar</span></span> | <span data-ttu-id="35565-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35565-109">Delegated (work or school account)</span></span> | <span data-ttu-id="35565-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35565-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35565-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="35565-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="35565-112">用户日历</span><span class="sxs-lookup"><span data-stu-id="35565-112">user calendar</span></span> | <span data-ttu-id="35565-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35565-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="35565-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35565-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="35565-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35565-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="35565-116">组日历</span><span class="sxs-lookup"><span data-stu-id="35565-116">group calendar</span></span> | <span data-ttu-id="35565-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35565-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="35565-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="35565-118">Not supported.</span></span> | <span data-ttu-id="35565-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="35565-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35565-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35565-120">HTTP request</span></span>

<span data-ttu-id="35565-121">更新用户的主日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="35565-121">Update the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="35565-122">更新组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="35565-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="35565-123">更新包含已标识事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="35565-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35565-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="35565-124">Request headers</span></span>

| <span data-ttu-id="35565-125">名称</span><span class="sxs-lookup"><span data-stu-id="35565-125">Name</span></span>       | <span data-ttu-id="35565-126">说明</span><span class="sxs-lookup"><span data-stu-id="35565-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="35565-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="35565-127">Authorization</span></span> | <span data-ttu-id="35565-128">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="35565-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="35565-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="35565-129">Request body</span></span>

<span data-ttu-id="35565-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="35565-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="35565-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="35565-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="35565-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="35565-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="35565-133">属性</span><span class="sxs-lookup"><span data-stu-id="35565-133">Property</span></span>     | <span data-ttu-id="35565-134">类型</span><span class="sxs-lookup"><span data-stu-id="35565-134">Type</span></span>        | <span data-ttu-id="35565-135">描述</span><span class="sxs-lookup"><span data-stu-id="35565-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="35565-136">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="35565-136">allowedRoles</span></span>|<span data-ttu-id="35565-137">string 集合</span><span class="sxs-lookup"><span data-stu-id="35565-137">string collection</span></span>| <span data-ttu-id="35565-138">日历的允许共享权限级别列表。</span><span class="sxs-lookup"><span data-stu-id="35565-138">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="35565-139">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="35565-139">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="35565-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="35565-140">emailAddress</span></span>|[<span data-ttu-id="35565-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="35565-141">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="35565-142">代表有权访问日历的 sharee。</span><span class="sxs-lookup"><span data-stu-id="35565-142">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="35565-143">对于 "My Organization" sharee， **address**属性为 null。</span><span class="sxs-lookup"><span data-stu-id="35565-143">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="35565-144">id</span><span class="sxs-lookup"><span data-stu-id="35565-144">id</span></span>|<span data-ttu-id="35565-145">String</span><span class="sxs-lookup"><span data-stu-id="35565-145">String</span></span>| <span data-ttu-id="35565-146">共享日历的用户（sharee）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="35565-146">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="35565-147">只读。</span><span class="sxs-lookup"><span data-stu-id="35565-147">Read-only.</span></span>|
|<span data-ttu-id="35565-148">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="35565-148">isInsideOrganization</span></span>|<span data-ttu-id="35565-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="35565-149">Boolean</span></span>| <span data-ttu-id="35565-150">如此如果上下文中的用户（sharee）与日历所有者在同一个组织中。</span><span class="sxs-lookup"><span data-stu-id="35565-150">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="35565-151">isRemovable</span><span class="sxs-lookup"><span data-stu-id="35565-151">isRemovable</span></span>|<span data-ttu-id="35565-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="35565-152">Boolean</span></span>| <span data-ttu-id="35565-153">`True`如果可以从指定日历的 sharees 列表中删除用户， `false`否则为。</span><span class="sxs-lookup"><span data-stu-id="35565-153">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="35565-154">"我的组织" 用户决定了贵组织内的其他人对给定日历的权限。</span><span class="sxs-lookup"><span data-stu-id="35565-154">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="35565-155">您无法将 "我的组织" 作为 sharee 删除到日历中。</span><span class="sxs-lookup"><span data-stu-id="35565-155">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="35565-156">role</span><span class="sxs-lookup"><span data-stu-id="35565-156">role</span></span>|<span data-ttu-id="35565-157">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="35565-157">calendarRoleType</span></span>| <span data-ttu-id="35565-158">日历 sharee 的当前权限级别。</span><span class="sxs-lookup"><span data-stu-id="35565-158">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="35565-159">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="35565-159">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="35565-160">响应</span><span class="sxs-lookup"><span data-stu-id="35565-160">Response</span></span>

<span data-ttu-id="35565-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[calendarPermission](../resources/calendarpermission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35565-161">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35565-162">示例</span><span class="sxs-lookup"><span data-stu-id="35565-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35565-163">请求</span><span class="sxs-lookup"><span data-stu-id="35565-163">Request</span></span>

<span data-ttu-id="35565-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="35565-164">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
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

### <a name="response"></a><span data-ttu-id="35565-165">响应</span><span class="sxs-lookup"><span data-stu-id="35565-165">Response</span></span>

<span data-ttu-id="35565-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="35565-166">The following is an example of the response.</span></span>

> <span data-ttu-id="35565-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35565-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->