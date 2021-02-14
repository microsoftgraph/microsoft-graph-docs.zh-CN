---
author: daspek
title: renameAction 资源类型
description: renameAction 对象提供有关重命名项目的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 35e0aa9929b8e152265a5540625f5981a587edb7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238650"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="650ff-103">renameAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="650ff-103">renameAction resource type</span></span>

<span data-ttu-id="650ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="650ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="650ff-105">itemActivity 上 **存在 renameAction** [][activity]资源表示活动重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="650ff-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="650ff-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="650ff-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="650ff-107">属性</span><span class="sxs-lookup"><span data-stu-id="650ff-107">Properties</span></span>

| <span data-ttu-id="650ff-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="650ff-108">Property name</span></span> | <span data-ttu-id="650ff-109">类型</span><span class="sxs-lookup"><span data-stu-id="650ff-109">Type</span></span>   | <span data-ttu-id="650ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="650ff-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="650ff-111">oldName</span><span class="sxs-lookup"><span data-stu-id="650ff-111">oldName</span></span>       | <span data-ttu-id="650ff-112">string</span><span class="sxs-lookup"><span data-stu-id="650ff-112">string</span></span> | <span data-ttu-id="650ff-113">项的原名称。</span><span class="sxs-lookup"><span data-stu-id="650ff-113">The previous name of the item.</span></span>
| <span data-ttu-id="650ff-114">newName</span><span class="sxs-lookup"><span data-stu-id="650ff-114">newName</span></span>       | <span data-ttu-id="650ff-115">string</span><span class="sxs-lookup"><span data-stu-id="650ff-115">string</span></span> | <span data-ttu-id="650ff-116">项目的新名称。</span><span class="sxs-lookup"><span data-stu-id="650ff-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="650ff-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="650ff-117">JSON representation</span></span>

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

