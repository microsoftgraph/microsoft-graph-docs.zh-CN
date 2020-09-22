---
title: calendarPermission 资源类型
description: 共享日历的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5ba8b0021a815f6c1ae329523741b7d536994ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071610"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="b69e0-103">calendarPermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="b69e0-103">calendarPermission resource type</span></span>

<span data-ttu-id="b69e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b69e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b69e0-105">在 Outlook 客户端中共享或委派了日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="b69e0-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="b69e0-106">仅代表日历所有者支持获取、更新和删除日历权限。</span><span class="sxs-lookup"><span data-stu-id="b69e0-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="b69e0-107">代表 sharee 或代理人获取日历的日历权限时，将返回一个空的日历权限集合。</span><span class="sxs-lookup"><span data-stu-id="b69e0-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="b69e0-108">为日历设置了 sharee 或委派后，您可以仅 [更新](../api/calendarpermission-update.md) **role** 属性来更改 sharee 或委派的权限。</span><span class="sxs-lookup"><span data-stu-id="b69e0-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="b69e0-109">您不**update**能更新**allowedRoles**、 **emailAddress**、 **isInsideOrganization**或**isRemovable**属性。</span><span class="sxs-lookup"><span data-stu-id="b69e0-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="b69e0-110">若要更改这些属性，应 [删除](../api/calendarpermission-delete.md) 相应的 **calendarPermission** 对象，并在 Outlook 客户端中创建另一个 sharee 或委派。</span><span class="sxs-lookup"><span data-stu-id="b69e0-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="b69e0-111">方法</span><span class="sxs-lookup"><span data-stu-id="b69e0-111">Methods</span></span>

| <span data-ttu-id="b69e0-112">方法</span><span class="sxs-lookup"><span data-stu-id="b69e0-112">Method</span></span>       | <span data-ttu-id="b69e0-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="b69e0-113">Return Type</span></span> | <span data-ttu-id="b69e0-114">说明</span><span class="sxs-lookup"><span data-stu-id="b69e0-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b69e0-115">获取 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="b69e0-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="b69e0-116">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="b69e0-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="b69e0-117">读取 calendarPermission 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b69e0-117">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="b69e0-118">更新</span><span class="sxs-lookup"><span data-stu-id="b69e0-118">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="b69e0-119">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="b69e0-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="b69e0-120">更新 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="b69e0-120">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="b69e0-121">删除</span><span class="sxs-lookup"><span data-stu-id="b69e0-121">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="b69e0-122">无</span><span class="sxs-lookup"><span data-stu-id="b69e0-122">None</span></span> | <span data-ttu-id="b69e0-123">删除 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="b69e0-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b69e0-124">属性</span><span class="sxs-lookup"><span data-stu-id="b69e0-124">Properties</span></span>

| <span data-ttu-id="b69e0-125">属性</span><span class="sxs-lookup"><span data-stu-id="b69e0-125">Property</span></span>     | <span data-ttu-id="b69e0-126">类型</span><span class="sxs-lookup"><span data-stu-id="b69e0-126">Type</span></span>        | <span data-ttu-id="b69e0-127">说明</span><span class="sxs-lookup"><span data-stu-id="b69e0-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b69e0-128">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="b69e0-128">allowedRoles</span></span>|<span data-ttu-id="b69e0-129">[calendarRoleType](#calendarroletype-values) 集合</span><span class="sxs-lookup"><span data-stu-id="b69e0-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="b69e0-130">允许共享或委派日历权限级别的列表。</span><span class="sxs-lookup"><span data-stu-id="b69e0-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="b69e0-131">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="b69e0-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="b69e0-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b69e0-132">emailAddress</span></span>|[<span data-ttu-id="b69e0-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b69e0-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="b69e0-134">代表有权访问日历的 sharee 或代理人。</span><span class="sxs-lookup"><span data-stu-id="b69e0-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="b69e0-135">对于 "My Organization" sharee， **address** 属性为 null。</span><span class="sxs-lookup"><span data-stu-id="b69e0-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="b69e0-136">只读。</span><span class="sxs-lookup"><span data-stu-id="b69e0-136">Read-only.</span></span> |
|<span data-ttu-id="b69e0-137">id</span><span class="sxs-lookup"><span data-stu-id="b69e0-137">id</span></span>|<span data-ttu-id="b69e0-138">String</span><span class="sxs-lookup"><span data-stu-id="b69e0-138">String</span></span>| <span data-ttu-id="b69e0-139">用户 (sharee 或委派) 与其共享日历的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b69e0-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="b69e0-140">只读。</span><span class="sxs-lookup"><span data-stu-id="b69e0-140">Read-only.</span></span>|
|<span data-ttu-id="b69e0-141">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="b69e0-141">isInsideOrganization</span></span>|<span data-ttu-id="b69e0-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b69e0-142">Boolean</span></span>| <span data-ttu-id="b69e0-143">如此如果上下文中的用户 (sharee 或委派) 与日历所有者在同一个组织中。</span><span class="sxs-lookup"><span data-stu-id="b69e0-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="b69e0-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="b69e0-144">isRemovable</span></span>|<span data-ttu-id="b69e0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b69e0-145">Boolean</span></span>| <span data-ttu-id="b69e0-146">`True` 如果可以从指定日历的 sharees 或代理列表中删除用户， `false` 否则为。</span><span class="sxs-lookup"><span data-stu-id="b69e0-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="b69e0-147">"我的组织" 用户决定了贵组织内的其他人对给定日历的权限。</span><span class="sxs-lookup"><span data-stu-id="b69e0-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="b69e0-148">您无法将 "我的组织" 作为 sharee 删除到日历中。</span><span class="sxs-lookup"><span data-stu-id="b69e0-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="b69e0-149">role</span><span class="sxs-lookup"><span data-stu-id="b69e0-149">role</span></span>|[<span data-ttu-id="b69e0-150">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="b69e0-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="b69e0-151">日历 sharee 或代理人的当前权限级别。</span><span class="sxs-lookup"><span data-stu-id="b69e0-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="b69e0-152">calendarRoleType 值</span><span class="sxs-lookup"><span data-stu-id="b69e0-152">calendarRoleType values</span></span>

| <span data-ttu-id="b69e0-153">值</span><span class="sxs-lookup"><span data-stu-id="b69e0-153">Values</span></span>        | <span data-ttu-id="b69e0-154">说明</span><span class="sxs-lookup"><span data-stu-id="b69e0-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="b69e0-155">无</span><span class="sxs-lookup"><span data-stu-id="b69e0-155">none</span></span> | <span data-ttu-id="b69e0-156">日历不与用户共享。</span><span class="sxs-lookup"><span data-stu-id="b69e0-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="b69e0-157">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="b69e0-157">freeBusyRead</span></span> | <span data-ttu-id="b69e0-158">用户是可以查看日历上的所有者的忙/闲状态的 sharee。</span><span class="sxs-lookup"><span data-stu-id="b69e0-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="b69e0-159">limitedRead</span><span class="sxs-lookup"><span data-stu-id="b69e0-159">limitedRead</span></span> | <span data-ttu-id="b69e0-160">用户是可以查看忙/闲状态以及日历上的事件的标题和位置的 sharee。</span><span class="sxs-lookup"><span data-stu-id="b69e0-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="b69e0-161">阅读</span><span class="sxs-lookup"><span data-stu-id="b69e0-161">read</span></span> | <span data-ttu-id="b69e0-162">用户是可以查看日历上的事件的所有详细信息的 sharee，所有者的私人活动除外。</span><span class="sxs-lookup"><span data-stu-id="b69e0-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="b69e0-163">写入</span><span class="sxs-lookup"><span data-stu-id="b69e0-163">write</span></span> | <span data-ttu-id="b69e0-164">User 是一个 sharee，可以查看除) 和编辑日历上的事件之外的所有详细信息 (。</span><span class="sxs-lookup"><span data-stu-id="b69e0-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="b69e0-165">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="b69e0-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="b69e0-166">用户是具有写入权限的代理，但无法查看日历上所有者的私人活动的信息。</span><span class="sxs-lookup"><span data-stu-id="b69e0-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="b69e0-167">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="b69e0-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="b69e0-168">用户是具有写访问权限的代理，可以在日历上查看所有者的私人活动的信息。</span><span class="sxs-lookup"><span data-stu-id="b69e0-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="b69e0-169">自</span><span class="sxs-lookup"><span data-stu-id="b69e0-169">custom</span></span> | <span data-ttu-id="b69e0-170">用户对日历具有自定义权限。</span><span class="sxs-lookup"><span data-stu-id="b69e0-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b69e0-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b69e0-171">JSON representation</span></span>

<span data-ttu-id="b69e0-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b69e0-172">The following is a JSON representation of the resource.</span></span>

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

