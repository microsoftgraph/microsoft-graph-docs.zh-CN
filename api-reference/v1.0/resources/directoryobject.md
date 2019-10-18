---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c1b462b001c9ccecfb792b705506a5b43f8b0254
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032737"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="10a44-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="10a44-104">directoryObject resource type</span></span>

<span data-ttu-id="10a44-p102">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="10a44-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="10a44-107">方法</span><span class="sxs-lookup"><span data-stu-id="10a44-107">Methods</span></span>

| <span data-ttu-id="10a44-108">方法</span><span class="sxs-lookup"><span data-stu-id="10a44-108">Method</span></span>       | <span data-ttu-id="10a44-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="10a44-109">Return Type</span></span>  |<span data-ttu-id="10a44-110">说明</span><span class="sxs-lookup"><span data-stu-id="10a44-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10a44-111">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="10a44-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="10a44-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="10a44-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="10a44-113">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10a44-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="10a44-114">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="10a44-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="10a44-115">无</span><span class="sxs-lookup"><span data-stu-id="10a44-115">None</span></span> |<span data-ttu-id="10a44-116">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="10a44-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="10a44-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="10a44-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="10a44-118">String collection</span><span class="sxs-lookup"><span data-stu-id="10a44-118">String collection</span></span>|<span data-ttu-id="10a44-p103">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="10a44-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="10a44-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="10a44-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="10a44-122">String collection</span><span class="sxs-lookup"><span data-stu-id="10a44-122">String collection</span></span>|<span data-ttu-id="10a44-p104">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="10a44-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="10a44-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="10a44-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="10a44-126">String collection</span><span class="sxs-lookup"><span data-stu-id="10a44-126">String collection</span></span>| <span data-ttu-id="10a44-p105">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="10a44-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="10a44-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="10a44-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="10a44-130">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="10a44-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="10a44-131">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="10a44-131">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="10a44-132">validateProperties</span><span class="sxs-lookup"><span data-stu-id="10a44-132">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="10a44-133">Json</span><span class="sxs-lookup"><span data-stu-id="10a44-133">Json</span></span>| <span data-ttu-id="10a44-134">验证 Office 365 组的显示名称或邮件别名是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="10a44-134">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="10a44-135">属性</span><span class="sxs-lookup"><span data-stu-id="10a44-135">Properties</span></span>

| <span data-ttu-id="10a44-136">属性</span><span class="sxs-lookup"><span data-stu-id="10a44-136">Property</span></span>   | <span data-ttu-id="10a44-137">类型</span><span class="sxs-lookup"><span data-stu-id="10a44-137">Type</span></span> |<span data-ttu-id="10a44-138">说明</span><span class="sxs-lookup"><span data-stu-id="10a44-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10a44-139">id</span><span class="sxs-lookup"><span data-stu-id="10a44-139">id</span></span>|<span data-ttu-id="10a44-140">String</span><span class="sxs-lookup"><span data-stu-id="10a44-140">String</span></span>|<span data-ttu-id="10a44-p106">用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="10a44-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10a44-145">关系</span><span class="sxs-lookup"><span data-stu-id="10a44-145">Relationships</span></span>

<span data-ttu-id="10a44-146">无</span><span class="sxs-lookup"><span data-stu-id="10a44-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="10a44-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10a44-147">JSON representation</span></span>

<span data-ttu-id="10a44-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10a44-148">Here is a JSON representation of the resource</span></span>

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
