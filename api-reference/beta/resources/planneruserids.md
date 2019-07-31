---
title: plannerUserIds 资源类型
description: '**PlannerUserIds**资源表示与计划共享的用户 id 的列表。 这是开放类型。 如果您使用的是 Office 365 组, 请使用组 API 来管理组成员身份, 以共享组的计划。 您还可以将组的现有成员添加到此集合中, 但它们不需要他们访问该组拥有的计划。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3382da3131040f6ae3dc78102ac6e5d64a23695c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965843"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="313ed-106">plannerUserIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="313ed-106">plannerUserIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="313ed-107">**PlannerUserIds**资源表示与[计划](plannerplan.md)共享的用户 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="313ed-107">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with.</span></span> <span data-ttu-id="313ed-108">这是开放类型。</span><span class="sxs-lookup"><span data-stu-id="313ed-108">This is an Open Type.</span></span> <span data-ttu-id="313ed-109">如果您使用的是 Office 365 组, 请使用组 API 来管理组成员身份, 以共享[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="313ed-109">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="313ed-110">您还可以将组的现有成员添加到此集合中, 但它们不需要他们访问该组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="313ed-110">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="313ed-111">属性</span><span class="sxs-lookup"><span data-stu-id="313ed-111">Properties</span></span>
<span data-ttu-id="313ed-112">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="313ed-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="313ed-113">在这种情况下, 客户端应将`true`用户 id 作为属性提供, 其值为 boolean。</span><span class="sxs-lookup"><span data-stu-id="313ed-113">In this case, the client should provide user ids as properties with their values being the `true` boolean.</span></span> <span data-ttu-id="313ed-114">当不再与用户 id 共享时, 将通过将属性值设置为`false`布尔值来自动删除属性。</span><span class="sxs-lookup"><span data-stu-id="313ed-114">When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="313ed-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="313ed-115">JSON representation</span></span>

<span data-ttu-id="313ed-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="313ed-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="313ed-117">示例</span><span class="sxs-lookup"><span data-stu-id="313ed-117">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
