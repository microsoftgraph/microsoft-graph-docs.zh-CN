---
author: daspek
ms.author: dspektor
title: renameAction 资源类型
description: RenameAction 对象提供有关重命名项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 693c5d8586a7ceef2c30f1e6dae17ac47d8e2d1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967315"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="80e2e-103">renameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="80e2e-103">renameAction resource type</span></span>

<span data-ttu-id="80e2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80e2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80e2e-105">[**ItemActivity**][activity]上的**renameAction**资源是否存在指示活动重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="80e2e-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="80e2e-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="80e2e-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="80e2e-107">属性</span><span class="sxs-lookup"><span data-stu-id="80e2e-107">Properties</span></span>

| <span data-ttu-id="80e2e-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="80e2e-108">Property name</span></span> | <span data-ttu-id="80e2e-109">类型</span><span class="sxs-lookup"><span data-stu-id="80e2e-109">Type</span></span>   | <span data-ttu-id="80e2e-110">说明</span><span class="sxs-lookup"><span data-stu-id="80e2e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="80e2e-111">oldName</span><span class="sxs-lookup"><span data-stu-id="80e2e-111">oldName</span></span>       | <span data-ttu-id="80e2e-112">string</span><span class="sxs-lookup"><span data-stu-id="80e2e-112">string</span></span> | <span data-ttu-id="80e2e-113">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="80e2e-113">The previous name of the item.</span></span>
| <span data-ttu-id="80e2e-114">newName</span><span class="sxs-lookup"><span data-stu-id="80e2e-114">newName</span></span>       | <span data-ttu-id="80e2e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="80e2e-115">string</span></span> | <span data-ttu-id="80e2e-116">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="80e2e-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80e2e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80e2e-117">JSON representation</span></span>

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

