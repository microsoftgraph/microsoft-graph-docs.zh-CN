---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8014c238487d5ada0f05f1a6edfed0402b25ae1a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181865"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="02143-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="02143-104">directoryObject resource type</span></span>

<span data-ttu-id="02143-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02143-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02143-p102">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="02143-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="02143-108">方法</span><span class="sxs-lookup"><span data-stu-id="02143-108">Methods</span></span>

| <span data-ttu-id="02143-109">方法</span><span class="sxs-lookup"><span data-stu-id="02143-109">Method</span></span>       | <span data-ttu-id="02143-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="02143-110">Return Type</span></span>  |<span data-ttu-id="02143-111">说明</span><span class="sxs-lookup"><span data-stu-id="02143-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02143-112">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="02143-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="02143-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="02143-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="02143-114">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="02143-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="02143-115">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="02143-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="02143-116">无</span><span class="sxs-lookup"><span data-stu-id="02143-116">None</span></span> |<span data-ttu-id="02143-117">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="02143-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="02143-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="02143-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="02143-119">String collection</span><span class="sxs-lookup"><span data-stu-id="02143-119">String collection</span></span>|<span data-ttu-id="02143-p103">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="02143-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="02143-122">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="02143-122">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="02143-123">String collection</span><span class="sxs-lookup"><span data-stu-id="02143-123">String collection</span></span>|<span data-ttu-id="02143-p104">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="02143-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="02143-126">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="02143-126">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="02143-127">String collection</span><span class="sxs-lookup"><span data-stu-id="02143-127">String collection</span></span>| <span data-ttu-id="02143-p105">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="02143-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="02143-130">getByIds</span><span class="sxs-lookup"><span data-stu-id="02143-130">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="02143-131">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02143-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="02143-132">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="02143-132">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="02143-133">validateProperties</span><span class="sxs-lookup"><span data-stu-id="02143-133">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="02143-134">Json</span><span class="sxs-lookup"><span data-stu-id="02143-134">Json</span></span>| <span data-ttu-id="02143-135">验证 Office 365 组的显示名称或邮件别名是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="02143-135">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="02143-136">属性</span><span class="sxs-lookup"><span data-stu-id="02143-136">Properties</span></span>

| <span data-ttu-id="02143-137">属性</span><span class="sxs-lookup"><span data-stu-id="02143-137">Property</span></span>   | <span data-ttu-id="02143-138">类型</span><span class="sxs-lookup"><span data-stu-id="02143-138">Type</span></span> |<span data-ttu-id="02143-139">说明</span><span class="sxs-lookup"><span data-stu-id="02143-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02143-140">id</span><span class="sxs-lookup"><span data-stu-id="02143-140">id</span></span>|<span data-ttu-id="02143-141">String</span><span class="sxs-lookup"><span data-stu-id="02143-141">String</span></span>|<span data-ttu-id="02143-p106">用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="02143-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02143-146">关系</span><span class="sxs-lookup"><span data-stu-id="02143-146">Relationships</span></span>

<span data-ttu-id="02143-147">无</span><span class="sxs-lookup"><span data-stu-id="02143-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="02143-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02143-148">JSON representation</span></span>

<span data-ttu-id="02143-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02143-149">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
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
