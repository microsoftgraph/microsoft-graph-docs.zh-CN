---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 83750686b4075f7577e88e1e6107dd2f2a5f4d2f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439903"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="b988e-104">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="b988e-104">directoryObject resource type</span></span>

<span data-ttu-id="b988e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b988e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b988e-p102">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="b988e-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="b988e-108">方法</span><span class="sxs-lookup"><span data-stu-id="b988e-108">Methods</span></span>

| <span data-ttu-id="b988e-109">方法</span><span class="sxs-lookup"><span data-stu-id="b988e-109">Method</span></span>       | <span data-ttu-id="b988e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b988e-110">Return Type</span></span>  |<span data-ttu-id="b988e-111">说明</span><span class="sxs-lookup"><span data-stu-id="b988e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b988e-112">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="b988e-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="b988e-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b988e-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="b988e-114">读取 directory 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b988e-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="b988e-115">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="b988e-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="b988e-116">无</span><span class="sxs-lookup"><span data-stu-id="b988e-116">None</span></span> |<span data-ttu-id="b988e-117">删除 directory 对象。</span><span class="sxs-lookup"><span data-stu-id="b988e-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="b988e-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b988e-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="b988e-119">String collection</span><span class="sxs-lookup"><span data-stu-id="b988e-119">String collection</span></span>|<span data-ttu-id="b988e-p103">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b988e-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="b988e-122">获取可用扩展属性</span><span class="sxs-lookup"><span data-stu-id="b988e-122">Get available extension properties</span></span>](../api/directoryobject-getavailableextensionproperties.md)|<span data-ttu-id="b988e-123">[extensionProperty](../resources/extensionproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b988e-123">[extensionProperty](../resources/extensionproperty.md) collection</span></span>|<span data-ttu-id="b988e-124">获取已在目录中注册的目录扩展属性的所有或筛选列表。</span><span class="sxs-lookup"><span data-stu-id="b988e-124">Get all or a filtered list of the directory extension properties that have been registered in a directory.</span></span>|
|[<span data-ttu-id="b988e-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b988e-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="b988e-126">String collection</span><span class="sxs-lookup"><span data-stu-id="b988e-126">String collection</span></span>|<span data-ttu-id="b988e-p104">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b988e-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="b988e-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b988e-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="b988e-130">String collection</span><span class="sxs-lookup"><span data-stu-id="b988e-130">String collection</span></span>| <span data-ttu-id="b988e-p105">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b988e-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="b988e-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="b988e-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="b988e-134">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b988e-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b988e-135">基于提供的 ID 集获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="b988e-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="b988e-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="b988e-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="b988e-137">Json</span><span class="sxs-lookup"><span data-stu-id="b988e-137">Json</span></span>| <span data-ttu-id="b988e-138">验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="b988e-138">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="b988e-139">属性</span><span class="sxs-lookup"><span data-stu-id="b988e-139">Properties</span></span>

| <span data-ttu-id="b988e-140">属性</span><span class="sxs-lookup"><span data-stu-id="b988e-140">Property</span></span>   | <span data-ttu-id="b988e-141">类型</span><span class="sxs-lookup"><span data-stu-id="b988e-141">Type</span></span> |<span data-ttu-id="b988e-142">说明</span><span class="sxs-lookup"><span data-stu-id="b988e-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b988e-143">id</span><span class="sxs-lookup"><span data-stu-id="b988e-143">id</span></span>|<span data-ttu-id="b988e-144">String</span><span class="sxs-lookup"><span data-stu-id="b988e-144">String</span></span>|<span data-ttu-id="b988e-145">对象的全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b988e-145">The unique identifier for the object.</span></span> <span data-ttu-id="b988e-146">例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="b988e-146">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="b988e-147">**id** 属性的值通常（但不总是）用 GUID 表示；将它视为不透明标识符，不要总将它视为 GUID。</span><span class="sxs-lookup"><span data-stu-id="b988e-147">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="b988e-148">键。</span><span class="sxs-lookup"><span data-stu-id="b988e-148">Key.</span></span> <span data-ttu-id="b988e-149">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b988e-149">Not nullable.</span></span> <span data-ttu-id="b988e-150">只读。</span><span class="sxs-lookup"><span data-stu-id="b988e-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b988e-151">关系</span><span class="sxs-lookup"><span data-stu-id="b988e-151">Relationships</span></span>

<span data-ttu-id="b988e-152">无</span><span class="sxs-lookup"><span data-stu-id="b988e-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b988e-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b988e-153">JSON representation</span></span>

<span data-ttu-id="b988e-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b988e-154">Here is a JSON representation of the resource</span></span>

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

