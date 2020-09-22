---
author: daspek
description: itemActivity 上存在 RenameAction 资源指示活动重命名了一个项。
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e14521b6be27a9b4b2772cd80c172e5faf73b0d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003498"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="5b55e-103">RenameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b55e-103">RenameAction resource type</span></span>

<span data-ttu-id="5b55e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b55e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b55e-105">[**itemActivity**][activity] 上存在 **RenameAction** 资源指示活动重命名了一个项。</span><span class="sxs-lookup"><span data-stu-id="5b55e-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5b55e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b55e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5b55e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5b55e-107">Properties</span></span>

| <span data-ttu-id="5b55e-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="5b55e-108">Property name</span></span> | <span data-ttu-id="5b55e-109">类型</span><span class="sxs-lookup"><span data-stu-id="5b55e-109">Type</span></span>   | <span data-ttu-id="5b55e-110">说明</span><span class="sxs-lookup"><span data-stu-id="5b55e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5b55e-111">oldName</span><span class="sxs-lookup"><span data-stu-id="5b55e-111">oldName</span></span>       | <span data-ttu-id="5b55e-112">string</span><span class="sxs-lookup"><span data-stu-id="5b55e-112">string</span></span> | <span data-ttu-id="5b55e-113">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="5b55e-113">The previous name of the item.</span></span>
| <span data-ttu-id="5b55e-114">newName</span><span class="sxs-lookup"><span data-stu-id="5b55e-114">newName</span></span>       | <span data-ttu-id="5b55e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="5b55e-115">string</span></span> | <span data-ttu-id="5b55e-116">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="5b55e-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="5b55e-117">注解</span><span class="sxs-lookup"><span data-stu-id="5b55e-117">Remarks</span></span>

<span data-ttu-id="5b55e-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="5b55e-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->


