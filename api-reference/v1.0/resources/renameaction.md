---
author: daspek
ms.author: dspektor
title: renameAction 资源类型
description: RenameAction 对象提供有关重命名项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b21d4630ca29aff9322d5114a5048b42f19fa4a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533851"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="1b070-103">renameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b070-103">renameAction resource type</span></span>

<span data-ttu-id="1b070-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b070-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b070-105">[**ItemActivity**][activity]上的**renameAction**资源是否存在指示活动重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="1b070-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="1b070-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="1b070-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1b070-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b070-107">Properties</span></span>

| <span data-ttu-id="1b070-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="1b070-108">Property name</span></span> | <span data-ttu-id="1b070-109">类型</span><span class="sxs-lookup"><span data-stu-id="1b070-109">Type</span></span>   | <span data-ttu-id="1b070-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b070-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1b070-111">oldName</span><span class="sxs-lookup"><span data-stu-id="1b070-111">oldName</span></span>       | <span data-ttu-id="1b070-112">string</span><span class="sxs-lookup"><span data-stu-id="1b070-112">string</span></span> | <span data-ttu-id="1b070-113">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="1b070-113">The previous name of the item.</span></span>
| <span data-ttu-id="1b070-114">newName</span><span class="sxs-lookup"><span data-stu-id="1b070-114">newName</span></span>       | <span data-ttu-id="1b070-115">字符串</span><span class="sxs-lookup"><span data-stu-id="1b070-115">string</span></span> | <span data-ttu-id="1b070-116">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="1b070-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b070-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b070-117">JSON representation</span></span>

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
