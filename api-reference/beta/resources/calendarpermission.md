---
title: calendarPermission 资源类型
description: 共享日历的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 80c704dbb3e50d3f4d0ba586a40f06f74f032321
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2020
ms.locfileid: "41651734"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="199df-103">calendarPermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="199df-103">calendarPermission resource type</span></span>

<span data-ttu-id="199df-104">在 Outlook 客户端中共享或委派了日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="199df-104">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="199df-105">仅代表日历所有者支持获取、更新和删除日历权限。</span><span class="sxs-lookup"><span data-stu-id="199df-105">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="199df-106">代表 sharee 或代理人获取日历的日历权限时，将返回一个空的日历权限集合。</span><span class="sxs-lookup"><span data-stu-id="199df-106">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="199df-107">为日历设置了 sharee 或委派后，您可以仅[更新](../api/calendarpermission-update.md) **role**属性来更改 sharee 或委派的权限。</span><span class="sxs-lookup"><span data-stu-id="199df-107">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="199df-108">您不\*\*\*\* 能更新**allowedRoles**、 **emailAddress**、 **isInsideOrganization**或**isRemovable**属性。</span><span class="sxs-lookup"><span data-stu-id="199df-108">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="199df-109">若要更改这些属性，应[删除](../api/calendarpermission-delete.md)相应的**calendarPermission**对象，并在 Outlook 客户端中创建另一个 sharee 或委派。</span><span class="sxs-lookup"><span data-stu-id="199df-109">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="199df-110">方法</span><span class="sxs-lookup"><span data-stu-id="199df-110">Methods</span></span>

| <span data-ttu-id="199df-111">方法</span><span class="sxs-lookup"><span data-stu-id="199df-111">Method</span></span>       | <span data-ttu-id="199df-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="199df-112">Return Type</span></span> | <span data-ttu-id="199df-113">说明</span><span class="sxs-lookup"><span data-stu-id="199df-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="199df-114">获取 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="199df-114">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="199df-115">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="199df-115">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="199df-116">读取 calendarPermission 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="199df-116">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="199df-117">更新</span><span class="sxs-lookup"><span data-stu-id="199df-117">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="199df-118">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="199df-118">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="199df-119">更新 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="199df-119">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="199df-120">删除</span><span class="sxs-lookup"><span data-stu-id="199df-120">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="199df-121">无</span><span class="sxs-lookup"><span data-stu-id="199df-121">None</span></span> | <span data-ttu-id="199df-122">删除 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="199df-122">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="199df-123">属性</span><span class="sxs-lookup"><span data-stu-id="199df-123">Properties</span></span>

| <span data-ttu-id="199df-124">属性</span><span class="sxs-lookup"><span data-stu-id="199df-124">Property</span></span>     | <span data-ttu-id="199df-125">类型</span><span class="sxs-lookup"><span data-stu-id="199df-125">Type</span></span>        | <span data-ttu-id="199df-126">描述</span><span class="sxs-lookup"><span data-stu-id="199df-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="199df-127">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="199df-127">allowedRoles</span></span>|<span data-ttu-id="199df-128">[calendarRoleType](#calendarroletype-values)集合</span><span class="sxs-lookup"><span data-stu-id="199df-128">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="199df-129">允许共享或委派日历权限级别的列表。</span><span class="sxs-lookup"><span data-stu-id="199df-129">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="199df-130">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="199df-130">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="199df-131">emailAddress</span><span class="sxs-lookup"><span data-stu-id="199df-131">emailAddress</span></span>|[<span data-ttu-id="199df-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="199df-132">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="199df-133">代表有权访问日历的 sharee 或代理人。</span><span class="sxs-lookup"><span data-stu-id="199df-133">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="199df-134">对于 "My Organization" sharee， **address**属性为 null。</span><span class="sxs-lookup"><span data-stu-id="199df-134">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="199df-135">只读。</span><span class="sxs-lookup"><span data-stu-id="199df-135">Read-only.</span></span> |
|<span data-ttu-id="199df-136">id</span><span class="sxs-lookup"><span data-stu-id="199df-136">id</span></span>|<span data-ttu-id="199df-137">字符串</span><span class="sxs-lookup"><span data-stu-id="199df-137">String</span></span>| <span data-ttu-id="199df-138">为其共享日历的用户（sharee 或代理人）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="199df-138">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="199df-139">只读。</span><span class="sxs-lookup"><span data-stu-id="199df-139">Read-only.</span></span>|
|<span data-ttu-id="199df-140">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="199df-140">isInsideOrganization</span></span>|<span data-ttu-id="199df-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="199df-141">Boolean</span></span>| <span data-ttu-id="199df-142">如此如果上下文中的用户（sharee 或代理人）与日历所有者在同一个组织中。</span><span class="sxs-lookup"><span data-stu-id="199df-142">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="199df-143">isRemovable</span><span class="sxs-lookup"><span data-stu-id="199df-143">isRemovable</span></span>|<span data-ttu-id="199df-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="199df-144">Boolean</span></span>| <span data-ttu-id="199df-145">`True`如果可以从指定日历的 sharees 或代理列表中删除用户， `false`否则为。</span><span class="sxs-lookup"><span data-stu-id="199df-145">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="199df-146">"我的组织" 用户决定了贵组织内的其他人对给定日历的权限。</span><span class="sxs-lookup"><span data-stu-id="199df-146">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="199df-147">您无法将 "我的组织" 作为 sharee 删除到日历中。</span><span class="sxs-lookup"><span data-stu-id="199df-147">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="199df-148">role</span><span class="sxs-lookup"><span data-stu-id="199df-148">role</span></span>|[<span data-ttu-id="199df-149">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="199df-149">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="199df-150">日历 sharee 或代理人的当前权限级别。</span><span class="sxs-lookup"><span data-stu-id="199df-150">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="199df-151">calendarRoleType 值</span><span class="sxs-lookup"><span data-stu-id="199df-151">calendarRoleType values</span></span>

| <span data-ttu-id="199df-152">值</span><span class="sxs-lookup"><span data-stu-id="199df-152">Values</span></span>        | <span data-ttu-id="199df-153">说明</span><span class="sxs-lookup"><span data-stu-id="199df-153">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="199df-154">无</span><span class="sxs-lookup"><span data-stu-id="199df-154">none</span></span> | <span data-ttu-id="199df-155">日历不与用户共享。</span><span class="sxs-lookup"><span data-stu-id="199df-155">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="199df-156">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="199df-156">freeBusyRead</span></span> | <span data-ttu-id="199df-157">用户是可以查看日历上的所有者的忙/闲状态的 sharee。</span><span class="sxs-lookup"><span data-stu-id="199df-157">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="199df-158">limitedRead</span><span class="sxs-lookup"><span data-stu-id="199df-158">limitedRead</span></span> | <span data-ttu-id="199df-159">用户是可以查看忙/闲状态以及日历上的事件的标题和位置的 sharee。</span><span class="sxs-lookup"><span data-stu-id="199df-159">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="199df-160">自述</span><span class="sxs-lookup"><span data-stu-id="199df-160">read</span></span> | <span data-ttu-id="199df-161">用户是可以查看日历上的事件的所有详细信息的 sharee，所有者的私人活动除外。</span><span class="sxs-lookup"><span data-stu-id="199df-161">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="199df-162">销帐</span><span class="sxs-lookup"><span data-stu-id="199df-162">write</span></span> | <span data-ttu-id="199df-163">用户是可以查看所有详细信息（私有事件除外）和编辑日历上的事件的 sharee。</span><span class="sxs-lookup"><span data-stu-id="199df-163">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="199df-164">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="199df-164">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="199df-165">用户是具有写入权限的代理，但无法查看日历上所有者的私人活动的信息。</span><span class="sxs-lookup"><span data-stu-id="199df-165">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="199df-166">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="199df-166">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="199df-167">用户是具有写访问权限的代理，可以在日历上查看所有者的私人活动的信息。</span><span class="sxs-lookup"><span data-stu-id="199df-167">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="199df-168">自</span><span class="sxs-lookup"><span data-stu-id="199df-168">custom</span></span> | <span data-ttu-id="199df-169">用户对日历具有自定义权限。</span><span class="sxs-lookup"><span data-stu-id="199df-169">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="199df-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="199df-170">JSON representation</span></span>

<span data-ttu-id="199df-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="199df-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->