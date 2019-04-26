---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563078"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="94903-102">RenameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="94903-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94903-103">[**itemActivity**][activity] 上存在 **RenameAction** 资源指示活动重命名了一个项。</span><span class="sxs-lookup"><span data-stu-id="94903-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="94903-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94903-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="94903-105">属性</span><span class="sxs-lookup"><span data-stu-id="94903-105">Properties</span></span>

| <span data-ttu-id="94903-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="94903-106">Property name</span></span> | <span data-ttu-id="94903-107">类型</span><span class="sxs-lookup"><span data-stu-id="94903-107">Type</span></span>   | <span data-ttu-id="94903-108">说明</span><span class="sxs-lookup"><span data-stu-id="94903-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="94903-109">oldName</span><span class="sxs-lookup"><span data-stu-id="94903-109">oldName</span></span>       | <span data-ttu-id="94903-110">string</span><span class="sxs-lookup"><span data-stu-id="94903-110">string</span></span> | <span data-ttu-id="94903-111">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="94903-111">The previous name of the item.</span></span>
| <span data-ttu-id="94903-112">newName</span><span class="sxs-lookup"><span data-stu-id="94903-112">newName</span></span>       | <span data-ttu-id="94903-113">string</span><span class="sxs-lookup"><span data-stu-id="94903-113">string</span></span> | <span data-ttu-id="94903-114">项的新名称。</span><span class="sxs-lookup"><span data-stu-id="94903-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="94903-115">注解</span><span class="sxs-lookup"><span data-stu-id="94903-115">Remarks</span></span>

<span data-ttu-id="94903-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="94903-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
