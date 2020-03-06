---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b90e81a9337cef51af4bfded50eaaf494e4ebca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507028"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="13fe0-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="13fe0-104">directoryObject resource type</span></span>

<span data-ttu-id="13fe0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13fe0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13fe0-p102">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="13fe0-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="13fe0-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="13fe0-108">This resource supports:</span></span>

- <span data-ttu-id="13fe0-109">通过提供 [delta](../api/directoryobject-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="13fe0-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="13fe0-110">方法</span><span class="sxs-lookup"><span data-stu-id="13fe0-110">Methods</span></span>

| <span data-ttu-id="13fe0-111">方法</span><span class="sxs-lookup"><span data-stu-id="13fe0-111">Method</span></span>       | <span data-ttu-id="13fe0-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="13fe0-112">Return Type</span></span>  |<span data-ttu-id="13fe0-113">说明</span><span class="sxs-lookup"><span data-stu-id="13fe0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13fe0-114">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="13fe0-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="13fe0-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="13fe0-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="13fe0-116">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13fe0-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="13fe0-117">删除</span><span class="sxs-lookup"><span data-stu-id="13fe0-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="13fe0-118">无</span><span class="sxs-lookup"><span data-stu-id="13fe0-118">None</span></span> |<span data-ttu-id="13fe0-119">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="13fe0-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="13fe0-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="13fe0-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="13fe0-121">String collection</span><span class="sxs-lookup"><span data-stu-id="13fe0-121">String collection</span></span>|<span data-ttu-id="13fe0-p103">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="13fe0-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="13fe0-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="13fe0-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="13fe0-125">String collection</span><span class="sxs-lookup"><span data-stu-id="13fe0-125">String collection</span></span>|<span data-ttu-id="13fe0-p104">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="13fe0-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="13fe0-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="13fe0-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="13fe0-129">String collection</span><span class="sxs-lookup"><span data-stu-id="13fe0-129">String collection</span></span>| <span data-ttu-id="13fe0-p105">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="13fe0-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="13fe0-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="13fe0-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="13fe0-133">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13fe0-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="13fe0-134">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="13fe0-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="13fe0-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="13fe0-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="13fe0-136">Json</span><span class="sxs-lookup"><span data-stu-id="13fe0-136">Json</span></span>| <span data-ttu-id="13fe0-137">验证 Office 365 组的显示名称或邮件别名是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="13fe0-137">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="13fe0-138">delta</span><span class="sxs-lookup"><span data-stu-id="13fe0-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="13fe0-139">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="13fe0-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="13fe0-140">获取目录对象的增量更改。</span><span class="sxs-lookup"><span data-stu-id="13fe0-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="13fe0-141">支持按派生类型筛选。</span><span class="sxs-lookup"><span data-stu-id="13fe0-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="13fe0-142">属性</span><span class="sxs-lookup"><span data-stu-id="13fe0-142">Properties</span></span>

| <span data-ttu-id="13fe0-143">属性</span><span class="sxs-lookup"><span data-stu-id="13fe0-143">Property</span></span>   | <span data-ttu-id="13fe0-144">类型</span><span class="sxs-lookup"><span data-stu-id="13fe0-144">Type</span></span> |<span data-ttu-id="13fe0-145">说明</span><span class="sxs-lookup"><span data-stu-id="13fe0-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13fe0-146">id</span><span class="sxs-lookup"><span data-stu-id="13fe0-146">id</span></span>|<span data-ttu-id="13fe0-147">String</span><span class="sxs-lookup"><span data-stu-id="13fe0-147">String</span></span>|<span data-ttu-id="13fe0-148">用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde12。</span><span class="sxs-lookup"><span data-stu-id="13fe0-148">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="13fe0-149">密钥。</span><span class="sxs-lookup"><span data-stu-id="13fe0-149">Key.</span></span> <span data-ttu-id="13fe0-150">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="13fe0-150">Not nullable.</span></span> <span data-ttu-id="13fe0-151">只读。</span><span class="sxs-lookup"><span data-stu-id="13fe0-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13fe0-152">关系</span><span class="sxs-lookup"><span data-stu-id="13fe0-152">Relationships</span></span>

<span data-ttu-id="13fe0-153">无</span><span class="sxs-lookup"><span data-stu-id="13fe0-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13fe0-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13fe0-154">JSON representation</span></span>

<span data-ttu-id="13fe0-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13fe0-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
