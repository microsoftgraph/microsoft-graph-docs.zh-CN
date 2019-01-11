---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
ms.openlocfilehash: a03ec966f966df556ab0122958b0b8f5464cf4fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889717"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="eca32-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="eca32-104">directoryObject resource type</span></span>

> <span data-ttu-id="eca32-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eca32-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eca32-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eca32-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eca32-p103">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="eca32-p103">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="eca32-109">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="eca32-109">This resource supports:</span></span>

- <span data-ttu-id="eca32-110">通过提供 [delta](../api/directoryobject-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="eca32-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="eca32-111">方法</span><span class="sxs-lookup"><span data-stu-id="eca32-111">Methods</span></span>

| <span data-ttu-id="eca32-112">方法</span><span class="sxs-lookup"><span data-stu-id="eca32-112">Method</span></span>       | <span data-ttu-id="eca32-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="eca32-113">Return Type</span></span>  |<span data-ttu-id="eca32-114">说明</span><span class="sxs-lookup"><span data-stu-id="eca32-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eca32-115">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="eca32-115">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="eca32-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="eca32-116">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="eca32-117">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eca32-117">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="eca32-118">删除</span><span class="sxs-lookup"><span data-stu-id="eca32-118">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="eca32-119">无</span><span class="sxs-lookup"><span data-stu-id="eca32-119">None</span></span> |<span data-ttu-id="eca32-120">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="eca32-120">Delete a directory object.</span></span> |
|[<span data-ttu-id="eca32-121">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="eca32-121">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="eca32-122">String collection</span><span class="sxs-lookup"><span data-stu-id="eca32-122">String collection</span></span>|<span data-ttu-id="eca32-p104">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="eca32-p104">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="eca32-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="eca32-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="eca32-126">String collection</span><span class="sxs-lookup"><span data-stu-id="eca32-126">String collection</span></span>|<span data-ttu-id="eca32-p105">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="eca32-p105">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="eca32-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="eca32-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="eca32-130">String collection</span><span class="sxs-lookup"><span data-stu-id="eca32-130">String collection</span></span>| <span data-ttu-id="eca32-p106">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="eca32-p106">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="eca32-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="eca32-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="eca32-134">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eca32-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="eca32-135">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="eca32-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="eca32-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="eca32-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="eca32-137">JSON</span><span class="sxs-lookup"><span data-stu-id="eca32-137">JSON</span></span>| <span data-ttu-id="eca32-138">验证 Office 365 组的显示名称或邮件昵称符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="eca32-138">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="eca32-139">delta</span><span class="sxs-lookup"><span data-stu-id="eca32-139">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="eca32-140">directoryObject 集合</span><span class="sxs-lookup"><span data-stu-id="eca32-140">directoryObject collection</span></span>| <span data-ttu-id="eca32-141">获得目录对象的增量更改。</span><span class="sxs-lookup"><span data-stu-id="eca32-141">Get incremental changes for directory objects.</span></span> <span data-ttu-id="eca32-142">按 derrived 类型筛选的支持。</span><span class="sxs-lookup"><span data-stu-id="eca32-142">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="eca32-143">属性</span><span class="sxs-lookup"><span data-stu-id="eca32-143">Properties</span></span>

| <span data-ttu-id="eca32-144">属性</span><span class="sxs-lookup"><span data-stu-id="eca32-144">Property</span></span>   | <span data-ttu-id="eca32-145">类型</span><span class="sxs-lookup"><span data-stu-id="eca32-145">Type</span></span> |<span data-ttu-id="eca32-146">说明</span><span class="sxs-lookup"><span data-stu-id="eca32-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eca32-147">id</span><span class="sxs-lookup"><span data-stu-id="eca32-147">id</span></span>|<span data-ttu-id="eca32-148">字符串</span><span class="sxs-lookup"><span data-stu-id="eca32-148">String</span></span>|<span data-ttu-id="eca32-149">Guid 对象; 的唯一标识符例如，12345678-9abc-def0-1234年-56789abcde12。</span><span class="sxs-lookup"><span data-stu-id="eca32-149">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="eca32-150">键。</span><span class="sxs-lookup"><span data-stu-id="eca32-150">Key.</span></span> <span data-ttu-id="eca32-151">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="eca32-151">Not nullable.</span></span> <span data-ttu-id="eca32-152">只读。</span><span class="sxs-lookup"><span data-stu-id="eca32-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eca32-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="eca32-153">Relationships</span></span>

<span data-ttu-id="eca32-154">无</span><span class="sxs-lookup"><span data-stu-id="eca32-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eca32-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eca32-155">JSON representation</span></span>

<span data-ttu-id="eca32-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eca32-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
