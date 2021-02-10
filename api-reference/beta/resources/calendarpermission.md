---
title: calendarPermission 资源类型
description: 与日历共享的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c8cf612827819370a43b02dbb7064d03530a5d1
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177093"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="9fd40-103">calendarPermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fd40-103">calendarPermission resource type</span></span>

<span data-ttu-id="9fd40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fd40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fd40-105">已在 Outlook 客户端中共享或委派日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="9fd40-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="9fd40-106">仅代表日历所有者获取、更新和删除日历权限。</span><span class="sxs-lookup"><span data-stu-id="9fd40-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="9fd40-107">代表共享者或代理人获取日历的日历权限将返回一个空的日历权限集合。</span><span class="sxs-lookup"><span data-stu-id="9fd40-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="9fd40-108">为日历设置共享者或代理人后，只能更新角色属性以更改共享[](../api/calendarpermission-update.md)者或代理人的权限。</span><span class="sxs-lookup"><span data-stu-id="9fd40-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="9fd40-109">不能更新 **allowedRoles** **、emailAddress、isInsideOrganization** 或 **isRemovable** 属性。 </span><span class="sxs-lookup"><span data-stu-id="9fd40-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="9fd40-110">若要更改这些属性，您应删除相应的 [](../api/calendarpermission-delete.md) **calendarPermission** 对象，在 Outlook 客户端中创建另一个共享或委托。</span><span class="sxs-lookup"><span data-stu-id="9fd40-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="9fd40-111">方法</span><span class="sxs-lookup"><span data-stu-id="9fd40-111">Methods</span></span>

| <span data-ttu-id="9fd40-112">方法</span><span class="sxs-lookup"><span data-stu-id="9fd40-112">Method</span></span>       | <span data-ttu-id="9fd40-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="9fd40-113">Return Type</span></span> | <span data-ttu-id="9fd40-114">说明</span><span class="sxs-lookup"><span data-stu-id="9fd40-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9fd40-115">获取 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9fd40-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="9fd40-116">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9fd40-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="9fd40-117">读取 calendarPermission 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fd40-117">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="9fd40-118">更新</span><span class="sxs-lookup"><span data-stu-id="9fd40-118">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="9fd40-119">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9fd40-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="9fd40-120">更新 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="9fd40-120">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="9fd40-121">删除</span><span class="sxs-lookup"><span data-stu-id="9fd40-121">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="9fd40-122">无</span><span class="sxs-lookup"><span data-stu-id="9fd40-122">None</span></span> | <span data-ttu-id="9fd40-123">删除 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="9fd40-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fd40-124">属性</span><span class="sxs-lookup"><span data-stu-id="9fd40-124">Properties</span></span>

| <span data-ttu-id="9fd40-125">属性</span><span class="sxs-lookup"><span data-stu-id="9fd40-125">Property</span></span>     | <span data-ttu-id="9fd40-126">类型</span><span class="sxs-lookup"><span data-stu-id="9fd40-126">Type</span></span>        | <span data-ttu-id="9fd40-127">说明</span><span class="sxs-lookup"><span data-stu-id="9fd40-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fd40-128">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="9fd40-128">allowedRoles</span></span>|<span data-ttu-id="9fd40-129">[calendarRoleType](#calendarroletype-values) 集合</span><span class="sxs-lookup"><span data-stu-id="9fd40-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="9fd40-130">日历允许的共享或委派权限级别列表。</span><span class="sxs-lookup"><span data-stu-id="9fd40-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="9fd40-131">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="9fd40-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="9fd40-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9fd40-132">emailAddress</span></span>|[<span data-ttu-id="9fd40-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9fd40-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="9fd40-134">表示有权访问日历的共享者或代理人。</span><span class="sxs-lookup"><span data-stu-id="9fd40-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="9fd40-135">对于"我的组织"共享， **地址** 属性为 null。</span><span class="sxs-lookup"><span data-stu-id="9fd40-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="9fd40-136">只读。</span><span class="sxs-lookup"><span data-stu-id="9fd40-136">Read-only.</span></span> |
|<span data-ttu-id="9fd40-137">id</span><span class="sxs-lookup"><span data-stu-id="9fd40-137">id</span></span>|<span data-ttu-id="9fd40-138">String</span><span class="sxs-lookup"><span data-stu-id="9fd40-138">String</span></span>| <span data-ttu-id="9fd40-139">已共享日历 (或) 用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9fd40-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="9fd40-140">只读。</span><span class="sxs-lookup"><span data-stu-id="9fd40-140">Read-only.</span></span>|
|<span data-ttu-id="9fd40-141">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="9fd40-141">isInsideOrganization</span></span>|<span data-ttu-id="9fd40-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="9fd40-142">Boolean</span></span>| <span data-ttu-id="9fd40-143">如此 如果上下文中的用户 (共享或委派) 与日历所有者位于同一组织内部。</span><span class="sxs-lookup"><span data-stu-id="9fd40-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="9fd40-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="9fd40-144">isRemovable</span></span>|<span data-ttu-id="9fd40-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fd40-145">Boolean</span></span>| <span data-ttu-id="9fd40-146">`True` 如果可以从指定日历的共享或委派列表中删除用户， `false` 否则。</span><span class="sxs-lookup"><span data-stu-id="9fd40-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="9fd40-147">"我的组织"用户确定组织中其他人对给定日历拥有的权限。</span><span class="sxs-lookup"><span data-stu-id="9fd40-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="9fd40-148">不能删除"我的组织"作为日历共享者。</span><span class="sxs-lookup"><span data-stu-id="9fd40-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="9fd40-149">role</span><span class="sxs-lookup"><span data-stu-id="9fd40-149">role</span></span>|[<span data-ttu-id="9fd40-150">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="9fd40-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="9fd40-151">日历共享者或代理人的当前权限级别。</span><span class="sxs-lookup"><span data-stu-id="9fd40-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="9fd40-152">calendarRoleType 值</span><span class="sxs-lookup"><span data-stu-id="9fd40-152">calendarRoleType values</span></span>

| <span data-ttu-id="9fd40-153">成员</span><span class="sxs-lookup"><span data-stu-id="9fd40-153">Member</span></span>        | <span data-ttu-id="9fd40-154">说明</span><span class="sxs-lookup"><span data-stu-id="9fd40-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="9fd40-155">无</span><span class="sxs-lookup"><span data-stu-id="9fd40-155">none</span></span> | <span data-ttu-id="9fd40-156">日历不与用户共享。</span><span class="sxs-lookup"><span data-stu-id="9fd40-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="9fd40-157">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="9fd40-157">freeBusyRead</span></span> | <span data-ttu-id="9fd40-158">用户是共享者，可以查看日历上所有者的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="9fd40-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="9fd40-159">limitedRead</span><span class="sxs-lookup"><span data-stu-id="9fd40-159">limitedRead</span></span> | <span data-ttu-id="9fd40-160">用户是可以查看忙/闲状态以及日历上事件的标题和位置的共享者。</span><span class="sxs-lookup"><span data-stu-id="9fd40-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="9fd40-161">阅读</span><span class="sxs-lookup"><span data-stu-id="9fd40-161">read</span></span> | <span data-ttu-id="9fd40-162">用户是一个共享者，可以查看日历上事件的所有详细信息，所有者的私人事件除外。</span><span class="sxs-lookup"><span data-stu-id="9fd40-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="9fd40-163">写入</span><span class="sxs-lookup"><span data-stu-id="9fd40-163">write</span></span> | <span data-ttu-id="9fd40-164">用户是一个共享者，可以查看所有详细信息 (日历上的私人事件) 和编辑事件除外。</span><span class="sxs-lookup"><span data-stu-id="9fd40-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="9fd40-165">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="9fd40-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="9fd40-166">用户是具有写入访问权限但无法在日历上查看所有者私人事件信息的代理人。</span><span class="sxs-lookup"><span data-stu-id="9fd40-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="9fd40-167">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="9fd40-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="9fd40-168">用户是具有写入访问权限的代理人，可以查看日历上所有者私人事件的信息。</span><span class="sxs-lookup"><span data-stu-id="9fd40-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="9fd40-169">custom</span><span class="sxs-lookup"><span data-stu-id="9fd40-169">custom</span></span> | <span data-ttu-id="9fd40-170">用户对日历具有自定义权限。</span><span class="sxs-lookup"><span data-stu-id="9fd40-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9fd40-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fd40-171">JSON representation</span></span>

<span data-ttu-id="9fd40-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fd40-172">The following is a JSON representation of the resource.</span></span>

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

