---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5084407b6927172f5d1ef956bd696952e1b551b7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440470"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="41acf-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="41acf-104">directoryObject resource type</span></span>

<span data-ttu-id="41acf-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41acf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41acf-p102">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="41acf-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="41acf-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="41acf-108">This resource supports:</span></span>

- <span data-ttu-id="41acf-109">通过提供 [delta](../api/directoryobject-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="41acf-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="41acf-110">方法</span><span class="sxs-lookup"><span data-stu-id="41acf-110">Methods</span></span>

| <span data-ttu-id="41acf-111">方法</span><span class="sxs-lookup"><span data-stu-id="41acf-111">Method</span></span>       | <span data-ttu-id="41acf-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="41acf-112">Return Type</span></span>  |<span data-ttu-id="41acf-113">说明</span><span class="sxs-lookup"><span data-stu-id="41acf-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41acf-114">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="41acf-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="41acf-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="41acf-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="41acf-116">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41acf-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="41acf-117">删除</span><span class="sxs-lookup"><span data-stu-id="41acf-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="41acf-118">无</span><span class="sxs-lookup"><span data-stu-id="41acf-118">None</span></span> |<span data-ttu-id="41acf-119">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="41acf-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="41acf-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="41acf-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="41acf-121">字符串集合</span><span class="sxs-lookup"><span data-stu-id="41acf-121">String collection</span></span>|<span data-ttu-id="41acf-p103">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="41acf-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="41acf-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="41acf-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="41acf-125">String collection</span><span class="sxs-lookup"><span data-stu-id="41acf-125">String collection</span></span>|<span data-ttu-id="41acf-p104">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="41acf-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="41acf-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="41acf-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="41acf-129">String collection</span><span class="sxs-lookup"><span data-stu-id="41acf-129">String collection</span></span>| <span data-ttu-id="41acf-p105">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="41acf-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="41acf-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="41acf-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="41acf-133">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41acf-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="41acf-134">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="41acf-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="41acf-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="41acf-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="41acf-136">Json</span><span class="sxs-lookup"><span data-stu-id="41acf-136">Json</span></span>| <span data-ttu-id="41acf-137">验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="41acf-137">Validate a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="41acf-138">delta</span><span class="sxs-lookup"><span data-stu-id="41acf-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="41acf-139">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="41acf-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="41acf-140">获取目录对象的增量更改。</span><span class="sxs-lookup"><span data-stu-id="41acf-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="41acf-141">支持按派生类型筛选。</span><span class="sxs-lookup"><span data-stu-id="41acf-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="41acf-142">属性</span><span class="sxs-lookup"><span data-stu-id="41acf-142">Properties</span></span>

| <span data-ttu-id="41acf-143">属性</span><span class="sxs-lookup"><span data-stu-id="41acf-143">Property</span></span>   | <span data-ttu-id="41acf-144">类型</span><span class="sxs-lookup"><span data-stu-id="41acf-144">Type</span></span> |<span data-ttu-id="41acf-145">说明</span><span class="sxs-lookup"><span data-stu-id="41acf-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41acf-146">id</span><span class="sxs-lookup"><span data-stu-id="41acf-146">id</span></span>|<span data-ttu-id="41acf-147">String</span><span class="sxs-lookup"><span data-stu-id="41acf-147">String</span></span>|<span data-ttu-id="41acf-148">对象的全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="41acf-148">The unique identifier for the object.</span></span> <span data-ttu-id="41acf-149">例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="41acf-149">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="41acf-150">**id** 属性的值通常（但不总是）用 GUID 表示；将它视为不透明标识符，不要总将它视为 GUID。</span><span class="sxs-lookup"><span data-stu-id="41acf-150">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="41acf-151">键。</span><span class="sxs-lookup"><span data-stu-id="41acf-151">Key.</span></span> <span data-ttu-id="41acf-152">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="41acf-152">Not nullable.</span></span> <span data-ttu-id="41acf-153">只读。</span><span class="sxs-lookup"><span data-stu-id="41acf-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41acf-154">关系</span><span class="sxs-lookup"><span data-stu-id="41acf-154">Relationships</span></span>

<span data-ttu-id="41acf-155">无</span><span class="sxs-lookup"><span data-stu-id="41acf-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41acf-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41acf-156">JSON representation</span></span>

<span data-ttu-id="41acf-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41acf-157">Here is a JSON representation of the resource</span></span>

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


