---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: 88fa2738c014f028ebd2cc6e37f83151c7fc984a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835705"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="8b4ad-102">RenameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b4ad-102">RenameAction resource type</span></span>

> <span data-ttu-id="8b4ad-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8b4ad-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b4ad-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b4ad-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b4ad-105">[**itemActivity**][activity] 上存在 **RenameAction** 资源指示活动重命名了一个项。</span><span class="sxs-lookup"><span data-stu-id="8b4ad-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8b4ad-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b4ad-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8b4ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="8b4ad-107">Properties</span></span>

| <span data-ttu-id="8b4ad-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="8b4ad-108">Property name</span></span> | <span data-ttu-id="8b4ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="8b4ad-109">Type</span></span>   | <span data-ttu-id="8b4ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="8b4ad-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8b4ad-111">oldName</span><span class="sxs-lookup"><span data-stu-id="8b4ad-111">oldName</span></span>       | <span data-ttu-id="8b4ad-112">string</span><span class="sxs-lookup"><span data-stu-id="8b4ad-112">string</span></span> | <span data-ttu-id="8b4ad-113">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="8b4ad-113">The previous name of the item.</span></span>
| <span data-ttu-id="8b4ad-114">newName</span><span class="sxs-lookup"><span data-stu-id="8b4ad-114">newName</span></span>       | <span data-ttu-id="8b4ad-115">string</span><span class="sxs-lookup"><span data-stu-id="8b4ad-115">string</span></span> | <span data-ttu-id="8b4ad-116">新项目的名称。</span><span class="sxs-lookup"><span data-stu-id="8b4ad-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="8b4ad-117">注解</span><span class="sxs-lookup"><span data-stu-id="8b4ad-117">Remarks</span></span>

<span data-ttu-id="8b4ad-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="8b4ad-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
