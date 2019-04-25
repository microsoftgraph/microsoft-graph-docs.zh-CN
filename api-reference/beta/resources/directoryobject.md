---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87fb1c21e2fa1e9788890d97f6afbd0b494c555e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507803"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="742a6-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="742a6-104">directoryObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="742a6-p102">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="742a6-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="742a6-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="742a6-107">This resource supports:</span></span>

- <span data-ttu-id="742a6-108">通过提供 [delta](../api/directoryobject-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="742a6-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="742a6-109">方法</span><span class="sxs-lookup"><span data-stu-id="742a6-109">Methods</span></span>

| <span data-ttu-id="742a6-110">方法</span><span class="sxs-lookup"><span data-stu-id="742a6-110">Method</span></span>       | <span data-ttu-id="742a6-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="742a6-111">Return Type</span></span>  |<span data-ttu-id="742a6-112">说明</span><span class="sxs-lookup"><span data-stu-id="742a6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="742a6-113">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="742a6-113">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="742a6-114">directoryObject</span><span class="sxs-lookup"><span data-stu-id="742a6-114">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="742a6-115">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="742a6-115">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="742a6-116">删除</span><span class="sxs-lookup"><span data-stu-id="742a6-116">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="742a6-117">无</span><span class="sxs-lookup"><span data-stu-id="742a6-117">None</span></span> |<span data-ttu-id="742a6-118">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="742a6-118">Delete a directory object.</span></span> |
|[<span data-ttu-id="742a6-119">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="742a6-119">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="742a6-120">String collection</span><span class="sxs-lookup"><span data-stu-id="742a6-120">String collection</span></span>|<span data-ttu-id="742a6-p103">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="742a6-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="742a6-123">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="742a6-123">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="742a6-124">String collection</span><span class="sxs-lookup"><span data-stu-id="742a6-124">String collection</span></span>|<span data-ttu-id="742a6-p104">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="742a6-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="742a6-127">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="742a6-127">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="742a6-128">String collection</span><span class="sxs-lookup"><span data-stu-id="742a6-128">String collection</span></span>| <span data-ttu-id="742a6-p105">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="742a6-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="742a6-131">getByIds</span><span class="sxs-lookup"><span data-stu-id="742a6-131">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="742a6-132">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="742a6-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="742a6-133">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="742a6-133">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="742a6-134">validateProperties</span><span class="sxs-lookup"><span data-stu-id="742a6-134">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="742a6-135">JSON</span><span class="sxs-lookup"><span data-stu-id="742a6-135">JSON</span></span>| <span data-ttu-id="742a6-136">验证 Office 365 组的显示名称或邮件别名是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="742a6-136">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="742a6-137">delta</span><span class="sxs-lookup"><span data-stu-id="742a6-137">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="742a6-138">directoryObject 集合</span><span class="sxs-lookup"><span data-stu-id="742a6-138">directoryObject collection</span></span>| <span data-ttu-id="742a6-139">获取目录对象的增量更改。</span><span class="sxs-lookup"><span data-stu-id="742a6-139">Get incremental changes for directory objects.</span></span> <span data-ttu-id="742a6-140">支持按派生类型筛选。</span><span class="sxs-lookup"><span data-stu-id="742a6-140">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="742a6-141">属性</span><span class="sxs-lookup"><span data-stu-id="742a6-141">Properties</span></span>

| <span data-ttu-id="742a6-142">属性</span><span class="sxs-lookup"><span data-stu-id="742a6-142">Property</span></span>   | <span data-ttu-id="742a6-143">类型</span><span class="sxs-lookup"><span data-stu-id="742a6-143">Type</span></span> |<span data-ttu-id="742a6-144">说明</span><span class="sxs-lookup"><span data-stu-id="742a6-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="742a6-145">id</span><span class="sxs-lookup"><span data-stu-id="742a6-145">id</span></span>|<span data-ttu-id="742a6-146">String</span><span class="sxs-lookup"><span data-stu-id="742a6-146">String</span></span>|<span data-ttu-id="742a6-147">用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde12。</span><span class="sxs-lookup"><span data-stu-id="742a6-147">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="742a6-148">密钥。</span><span class="sxs-lookup"><span data-stu-id="742a6-148">Key.</span></span> <span data-ttu-id="742a6-149">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="742a6-149">Not nullable.</span></span> <span data-ttu-id="742a6-150">只读。</span><span class="sxs-lookup"><span data-stu-id="742a6-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="742a6-151">关系</span><span class="sxs-lookup"><span data-stu-id="742a6-151">Relationships</span></span>

<span data-ttu-id="742a6-152">无</span><span class="sxs-lookup"><span data-stu-id="742a6-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="742a6-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="742a6-153">JSON representation</span></span>

<span data-ttu-id="742a6-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="742a6-154">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
