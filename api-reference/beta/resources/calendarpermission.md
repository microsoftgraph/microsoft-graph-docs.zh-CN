---
title: calendarPermission 资源类型
description: 共享日历的用户的权限。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5d19a1738d3369f2d910dd590062016acf3047ab
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950449"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="3bcdf-103">calendarPermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bcdf-103">calendarPermission resource type</span></span>

<span data-ttu-id="3bcdf-104">共享日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-104">The permissions of a user with whom the calendar is shared.</span></span> 

## <a name="methods"></a><span data-ttu-id="3bcdf-105">方法</span><span class="sxs-lookup"><span data-stu-id="3bcdf-105">Methods</span></span>

| <span data-ttu-id="3bcdf-106">方法</span><span class="sxs-lookup"><span data-stu-id="3bcdf-106">Method</span></span>       | <span data-ttu-id="3bcdf-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3bcdf-107">Return Type</span></span> | <span data-ttu-id="3bcdf-108">说明</span><span class="sxs-lookup"><span data-stu-id="3bcdf-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3bcdf-109">获取 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="3bcdf-109">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="3bcdf-110">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="3bcdf-110">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="3bcdf-111">读取 calendarPermission 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-111">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="3bcdf-112">Update</span><span class="sxs-lookup"><span data-stu-id="3bcdf-112">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="3bcdf-113">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="3bcdf-113">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="3bcdf-114">更新 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-114">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="3bcdf-115">删除</span><span class="sxs-lookup"><span data-stu-id="3bcdf-115">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="3bcdf-116">无</span><span class="sxs-lookup"><span data-stu-id="3bcdf-116">None</span></span> | <span data-ttu-id="3bcdf-117">删除 calendarPermission 对象。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-117">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3bcdf-118">属性</span><span class="sxs-lookup"><span data-stu-id="3bcdf-118">Properties</span></span>

| <span data-ttu-id="3bcdf-119">属性</span><span class="sxs-lookup"><span data-stu-id="3bcdf-119">Property</span></span>     | <span data-ttu-id="3bcdf-120">类型</span><span class="sxs-lookup"><span data-stu-id="3bcdf-120">Type</span></span>        | <span data-ttu-id="3bcdf-121">描述</span><span class="sxs-lookup"><span data-stu-id="3bcdf-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3bcdf-122">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="3bcdf-122">allowedRoles</span></span>|<span data-ttu-id="3bcdf-123">string 集合</span><span class="sxs-lookup"><span data-stu-id="3bcdf-123">string collection</span></span>| <span data-ttu-id="3bcdf-124">日历的允许共享权限级别列表。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-124">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="3bcdf-125">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-125">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="3bcdf-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3bcdf-126">emailAddress</span></span>|[<span data-ttu-id="3bcdf-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3bcdf-127">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="3bcdf-128">代表有权访问日历的 sharee。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-128">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="3bcdf-129">对于 "My Organization" sharee， **address**属性为 null。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-129">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="3bcdf-130">id</span><span class="sxs-lookup"><span data-stu-id="3bcdf-130">id</span></span>|<span data-ttu-id="3bcdf-131">String</span><span class="sxs-lookup"><span data-stu-id="3bcdf-131">String</span></span>| <span data-ttu-id="3bcdf-132">共享日历的用户（sharee）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-132">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="3bcdf-133">只读。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-133">Read-only.</span></span>|
|<span data-ttu-id="3bcdf-134">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="3bcdf-134">isInsideOrganization</span></span>|<span data-ttu-id="3bcdf-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bcdf-135">Boolean</span></span>| <span data-ttu-id="3bcdf-136">如此如果上下文中的用户（sharee）与日历所有者在同一个组织中。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-136">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="3bcdf-137">isRemovable</span><span class="sxs-lookup"><span data-stu-id="3bcdf-137">isRemovable</span></span>|<span data-ttu-id="3bcdf-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bcdf-138">Boolean</span></span>| <span data-ttu-id="3bcdf-139">`True`如果可以从指定日历的 sharees 列表中删除用户， `false`否则为。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-139">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="3bcdf-140">"我的组织" 用户决定了贵组织内的其他人对给定日历的权限。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-140">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="3bcdf-141">您无法将 "我的组织" 作为 sharee 删除到日历中。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-141">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="3bcdf-142">role</span><span class="sxs-lookup"><span data-stu-id="3bcdf-142">role</span></span>|<span data-ttu-id="3bcdf-143">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="3bcdf-143">calendarRoleType</span></span>| <span data-ttu-id="3bcdf-144">日历 sharee 的当前权限级别。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-144">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="3bcdf-145">可取值为：`none`、`freeBusyRead`、`limitedRead`、`read`、`write`、`delegateWithoutPrivateEventAccess`、`delegateWithPrivateEventAccess`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-145">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bcdf-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bcdf-146">JSON representation</span></span>

<span data-ttu-id="3bcdf-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bcdf-147">The following is a JSON representation of the resource.</span></span>

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