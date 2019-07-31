---
author: daspek
description: itemActivity 上存在 RenameAction 资源指示活动重命名了一个项。
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d62d3f7f836ece716bdc3e616e1943de8c040652
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965415"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="6c577-103">RenameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c577-103">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c577-104">[**itemActivity**][activity] 上存在 **RenameAction** 资源指示活动重命名了一个项。</span><span class="sxs-lookup"><span data-stu-id="6c577-104">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="6c577-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c577-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6c577-106">属性</span><span class="sxs-lookup"><span data-stu-id="6c577-106">Properties</span></span>

| <span data-ttu-id="6c577-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="6c577-107">Property name</span></span> | <span data-ttu-id="6c577-108">类型</span><span class="sxs-lookup"><span data-stu-id="6c577-108">Type</span></span>   | <span data-ttu-id="6c577-109">说明</span><span class="sxs-lookup"><span data-stu-id="6c577-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6c577-110">oldName</span><span class="sxs-lookup"><span data-stu-id="6c577-110">oldName</span></span>       | <span data-ttu-id="6c577-111">string</span><span class="sxs-lookup"><span data-stu-id="6c577-111">string</span></span> | <span data-ttu-id="6c577-112">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="6c577-112">The previous name of the item.</span></span>
| <span data-ttu-id="6c577-113">newName</span><span class="sxs-lookup"><span data-stu-id="6c577-113">newName</span></span>       | <span data-ttu-id="6c577-114">string</span><span class="sxs-lookup"><span data-stu-id="6c577-114">string</span></span> | <span data-ttu-id="6c577-115">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="6c577-115">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="6c577-116">注解</span><span class="sxs-lookup"><span data-stu-id="6c577-116">Remarks</span></span>

<span data-ttu-id="6c577-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="6c577-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
