---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515466"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="c1f9a-102">RenameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1f9a-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1f9a-103">[**itemActivity**][activity] 上存在 **RenameAction** 资源指示活动重命名了一个项。</span><span class="sxs-lookup"><span data-stu-id="c1f9a-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c1f9a-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1f9a-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c1f9a-105">属性</span><span class="sxs-lookup"><span data-stu-id="c1f9a-105">Properties</span></span>

| <span data-ttu-id="c1f9a-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="c1f9a-106">Property name</span></span> | <span data-ttu-id="c1f9a-107">类型</span><span class="sxs-lookup"><span data-stu-id="c1f9a-107">Type</span></span>   | <span data-ttu-id="c1f9a-108">说明</span><span class="sxs-lookup"><span data-stu-id="c1f9a-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c1f9a-109">oldName</span><span class="sxs-lookup"><span data-stu-id="c1f9a-109">oldName</span></span>       | <span data-ttu-id="c1f9a-110">string</span><span class="sxs-lookup"><span data-stu-id="c1f9a-110">string</span></span> | <span data-ttu-id="c1f9a-111">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="c1f9a-111">The previous name of the item.</span></span>
| <span data-ttu-id="c1f9a-112">newname</span><span class="sxs-lookup"><span data-stu-id="c1f9a-112">newName</span></span>       | <span data-ttu-id="c1f9a-113">string</span><span class="sxs-lookup"><span data-stu-id="c1f9a-113">string</span></span> | <span data-ttu-id="c1f9a-114">新项目的名称。</span><span class="sxs-lookup"><span data-stu-id="c1f9a-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="c1f9a-115">注解</span><span class="sxs-lookup"><span data-stu-id="c1f9a-115">Remarks</span></span>

<span data-ttu-id="c1f9a-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="c1f9a-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/renameaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
