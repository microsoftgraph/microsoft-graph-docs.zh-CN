---
author: daspek
ms.author: dspektor
title: renameAction 资源类型
description: RenameAction 对象提供有关重命名项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2949a3875d657dba3c64b6753855476c1d66bfb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034718"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="cc8c4-103">renameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc8c4-103">renameAction resource type</span></span>

<span data-ttu-id="cc8c4-104">[**ItemActivity**][activity]上的**renameAction**资源是否存在指示活动重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="cc8c4-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="cc8c4-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="cc8c4-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="cc8c4-106">属性</span><span class="sxs-lookup"><span data-stu-id="cc8c4-106">Properties</span></span>

| <span data-ttu-id="cc8c4-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="cc8c4-107">Property name</span></span> | <span data-ttu-id="cc8c4-108">类型</span><span class="sxs-lookup"><span data-stu-id="cc8c4-108">Type</span></span>   | <span data-ttu-id="cc8c4-109">说明</span><span class="sxs-lookup"><span data-stu-id="cc8c4-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="cc8c4-110">oldName</span><span class="sxs-lookup"><span data-stu-id="cc8c4-110">oldName</span></span>       | <span data-ttu-id="cc8c4-111">string</span><span class="sxs-lookup"><span data-stu-id="cc8c4-111">string</span></span> | <span data-ttu-id="cc8c4-112">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="cc8c4-112">The previous name of the item.</span></span>
| <span data-ttu-id="cc8c4-113">newName</span><span class="sxs-lookup"><span data-stu-id="cc8c4-113">newName</span></span>       | <span data-ttu-id="cc8c4-114">string</span><span class="sxs-lookup"><span data-stu-id="cc8c4-114">string</span></span> | <span data-ttu-id="cc8c4-115">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="cc8c4-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc8c4-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc8c4-116">JSON representation</span></span>

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
