---
title: 更新 calendarpermission
description: 更新 calendarpermission 对象的属性。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e69a1b4cdc66e9c591d060bed6600c4383e14a63
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936788"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="7adbd-103">更新 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="7adbd-103">Update calendarPermission</span></span>

<span data-ttu-id="7adbd-104">更新 calendarPermission 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7adbd-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7adbd-105">权限</span><span class="sxs-lookup"><span data-stu-id="7adbd-105">Permissions</span></span>

<span data-ttu-id="7adbd-106">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7adbd-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="7adbd-107">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7adbd-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7adbd-108">日历</span><span class="sxs-lookup"><span data-stu-id="7adbd-108">Calendar</span></span> | <span data-ttu-id="7adbd-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7adbd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7adbd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7adbd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7adbd-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="7adbd-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="7adbd-112">用户日历</span><span class="sxs-lookup"><span data-stu-id="7adbd-112">user calendar</span></span> | <span data-ttu-id="7adbd-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7adbd-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="7adbd-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7adbd-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="7adbd-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7adbd-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="7adbd-116">组日历</span><span class="sxs-lookup"><span data-stu-id="7adbd-116">group calendar</span></span> | <span data-ttu-id="7adbd-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7adbd-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="7adbd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7adbd-118">Not supported.</span></span> | <span data-ttu-id="7adbd-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7adbd-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7adbd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7adbd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
PATCH /groups/{id}/calendar/calendarPermissions/{id}
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7adbd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7adbd-121">Request headers</span></span>

| <span data-ttu-id="7adbd-122">名称</span><span class="sxs-lookup"><span data-stu-id="7adbd-122">Name</span></span>       | <span data-ttu-id="7adbd-123">说明</span><span class="sxs-lookup"><span data-stu-id="7adbd-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7adbd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7adbd-124">Authorization</span></span> | <span data-ttu-id="7adbd-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7adbd-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7adbd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7adbd-126">Request body</span></span>

<span data-ttu-id="7adbd-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="7adbd-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7adbd-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="7adbd-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7adbd-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7adbd-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7adbd-130">属性</span><span class="sxs-lookup"><span data-stu-id="7adbd-130">Property</span></span>     | <span data-ttu-id="7adbd-131">类型</span><span class="sxs-lookup"><span data-stu-id="7adbd-131">Type</span></span>        | <span data-ttu-id="7adbd-132">描述</span><span class="sxs-lookup"><span data-stu-id="7adbd-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7adbd-133">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="7adbd-133">allowedRoles</span></span>|<span data-ttu-id="7adbd-134">string 集合</span><span class="sxs-lookup"><span data-stu-id="7adbd-134">string collection</span></span>| <span data-ttu-id="7adbd-135">日历的允许共享权限级别列表。</span><span class="sxs-lookup"><span data-stu-id="7adbd-135">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="7adbd-136">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="7adbd-136">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="7adbd-137">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7adbd-137">emailAddress</span></span>|[<span data-ttu-id="7adbd-138">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7adbd-138">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="7adbd-139">代表有权访问日历的 sharee。</span><span class="sxs-lookup"><span data-stu-id="7adbd-139">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="7adbd-140">对于 "My Organization" sharee， **address**属性为 null。</span><span class="sxs-lookup"><span data-stu-id="7adbd-140">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="7adbd-141">id</span><span class="sxs-lookup"><span data-stu-id="7adbd-141">id</span></span>|<span data-ttu-id="7adbd-142">字符串</span><span class="sxs-lookup"><span data-stu-id="7adbd-142">String</span></span>| <span data-ttu-id="7adbd-143">共享日历的用户（sharee）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7adbd-143">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="7adbd-144">只读。</span><span class="sxs-lookup"><span data-stu-id="7adbd-144">Read-only.</span></span>|
|<span data-ttu-id="7adbd-145">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="7adbd-145">isInsideOrganization</span></span>|<span data-ttu-id="7adbd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7adbd-146">Boolean</span></span>| <span data-ttu-id="7adbd-147">如此如果上下文中的用户（sharee）与日历所有者在同一个组织中。</span><span class="sxs-lookup"><span data-stu-id="7adbd-147">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="7adbd-148">isRemovable</span><span class="sxs-lookup"><span data-stu-id="7adbd-148">isRemovable</span></span>|<span data-ttu-id="7adbd-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7adbd-149">Boolean</span></span>| <span data-ttu-id="7adbd-150">`True`如果可以从指定日历的 sharees 列表中删除用户， `false`否则为。</span><span class="sxs-lookup"><span data-stu-id="7adbd-150">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="7adbd-151">"我的组织" 用户决定了贵组织内的其他人对给定日历的权限。</span><span class="sxs-lookup"><span data-stu-id="7adbd-151">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="7adbd-152">您无法将 "我的组织" 作为 sharee 删除到日历中。</span><span class="sxs-lookup"><span data-stu-id="7adbd-152">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="7adbd-153">role</span><span class="sxs-lookup"><span data-stu-id="7adbd-153">role</span></span>|<span data-ttu-id="7adbd-154">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="7adbd-154">calendarRoleType</span></span>| <span data-ttu-id="7adbd-155">日历 sharee 的当前权限级别。</span><span class="sxs-lookup"><span data-stu-id="7adbd-155">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="7adbd-156">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="7adbd-156">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="7adbd-157">响应</span><span class="sxs-lookup"><span data-stu-id="7adbd-157">Response</span></span>

<span data-ttu-id="7adbd-158">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[calendarPermission](../resources/calendarpermission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7adbd-158">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7adbd-159">示例</span><span class="sxs-lookup"><span data-stu-id="7adbd-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7adbd-160">请求</span><span class="sxs-lookup"><span data-stu-id="7adbd-160">Request</span></span>

<span data-ttu-id="7adbd-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7adbd-161">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7adbd-162">响应</span><span class="sxs-lookup"><span data-stu-id="7adbd-162">Response</span></span>

<span data-ttu-id="7adbd-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7adbd-163">The following is an example of the response.</span></span>

> <span data-ttu-id="7adbd-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7adbd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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