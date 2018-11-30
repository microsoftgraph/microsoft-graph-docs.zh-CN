---
title: plannerUserIds 资源类型
description: '**plannerUserIds** 资源表示与其共享计划的用户 ID 列表。它是开放类型。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享组的计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。'
ms.openlocfilehash: f2115cb31825f30190701bc2ab6b0d29669c4665
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011606"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="0c195-106">plannerUserIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c195-106">plannerUserIds resource type</span></span>

<span data-ttu-id="0c195-p102">**plannerUserIds** 资源表示与其共享[计划](plannerplan.md)的用户 ID 列表。它是开放类型。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="0c195-p102">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with. This is an Open Type. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="0c195-111">属性</span><span class="sxs-lookup"><span data-stu-id="0c195-111">Properties</span></span>
<span data-ttu-id="0c195-p103">开放类型的属性可以由客户端定义。在这种情况下，客户端应将用户 ID 作为属性，并且其值需为 `true` 布尔值。不再与用户 ID 共享时，则将属性值设置为 `false` 布尔值来自动删除属性。</span><span class="sxs-lookup"><span data-stu-id="0c195-p103">Properties of an Open Type can be defined by the client. In this case, the client should provide user ids as properties with their values being the `true` boolean. When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c195-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c195-115">JSON representation</span></span>

<span data-ttu-id="0c195-116">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c195-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="0c195-117">// 示例</span><span class="sxs-lookup"><span data-stu-id="0c195-117">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->