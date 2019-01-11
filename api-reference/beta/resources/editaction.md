---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 78e4d1aff2003cc6d23580f4e52b46667cf6a9e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841704"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="8cc34-102">EditAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cc34-102">EditAction resource type</span></span>

> <span data-ttu-id="8cc34-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8cc34-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cc34-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8cc34-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cc34-105">[**itemActivity**][activity] 上存在 **EditAction** 资源指示活动已编辑一个项。</span><span class="sxs-lookup"><span data-stu-id="8cc34-105">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="8cc34-106">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="8cc34-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8cc34-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cc34-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="8cc34-108">属性</span><span class="sxs-lookup"><span data-stu-id="8cc34-108">Properties</span></span>

<span data-ttu-id="8cc34-109">无。</span><span class="sxs-lookup"><span data-stu-id="8cc34-109">None.</span></span> <span data-ttu-id="8cc34-110">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="8cc34-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="8cc34-111">注解</span><span class="sxs-lookup"><span data-stu-id="8cc34-111">Remarks</span></span>

<span data-ttu-id="8cc34-112">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="8cc34-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction"
} -->
