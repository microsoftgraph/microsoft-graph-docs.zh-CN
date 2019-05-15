---
author: daspek
ms.author: dspektor
title: renameAction 资源类型
description: RenameAction 对象提供有关重命名项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bce040130d74b7977fc1f988a34edde674f9e0d4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970643"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="308a3-103">renameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="308a3-103">renameAction resource type</span></span>

<span data-ttu-id="308a3-104">[activity] [**ItemActivity**]上的**renameAction**资源是否存在指示活动重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="308a3-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="308a3-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="308a3-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="308a3-106">属性</span><span class="sxs-lookup"><span data-stu-id="308a3-106">Properties</span></span>

| <span data-ttu-id="308a3-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="308a3-107">Property name</span></span> | <span data-ttu-id="308a3-108">类型</span><span class="sxs-lookup"><span data-stu-id="308a3-108">Type</span></span>   | <span data-ttu-id="308a3-109">说明</span><span class="sxs-lookup"><span data-stu-id="308a3-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="308a3-110">oldName</span><span class="sxs-lookup"><span data-stu-id="308a3-110">oldName</span></span>       | <span data-ttu-id="308a3-111">string</span><span class="sxs-lookup"><span data-stu-id="308a3-111">string</span></span> | <span data-ttu-id="308a3-112">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="308a3-112">The previous name of the item.</span></span>
| <span data-ttu-id="308a3-113">newName</span><span class="sxs-lookup"><span data-stu-id="308a3-113">newName</span></span>       | <span data-ttu-id="308a3-114">string</span><span class="sxs-lookup"><span data-stu-id="308a3-114">string</span></span> | <span data-ttu-id="308a3-115">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="308a3-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="308a3-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="308a3-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->
