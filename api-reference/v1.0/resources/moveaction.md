---
author: daspek
ms.author: dspektor
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 04c9ddad00b5705d84af6e72ac194a0d32fd015c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447379"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="1232c-103">moveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="1232c-103">moveAction resource type</span></span>

<span data-ttu-id="1232c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1232c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1232c-105">[**ItemActivity**][activity]上的**moveAction**资源是否存在指示活动已移动项目。</span><span class="sxs-lookup"><span data-stu-id="1232c-105">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="1232c-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="1232c-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1232c-107">属性</span><span class="sxs-lookup"><span data-stu-id="1232c-107">Properties</span></span>

| <span data-ttu-id="1232c-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="1232c-108">Property name</span></span> | <span data-ttu-id="1232c-109">类型</span><span class="sxs-lookup"><span data-stu-id="1232c-109">Type</span></span>   | <span data-ttu-id="1232c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1232c-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1232c-111">from</span><span class="sxs-lookup"><span data-stu-id="1232c-111">from</span></span>          | <span data-ttu-id="1232c-112">string</span><span class="sxs-lookup"><span data-stu-id="1232c-112">string</span></span> | <span data-ttu-id="1232c-113">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="1232c-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="1232c-114">to</span><span class="sxs-lookup"><span data-stu-id="1232c-114">to</span></span>            | <span data-ttu-id="1232c-115">string</span><span class="sxs-lookup"><span data-stu-id="1232c-115">string</span></span> | <span data-ttu-id="1232c-116">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="1232c-116">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1232c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1232c-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
