---
author: daspek
ms.author: dspektor
title: deleteAction 资源类型
description: DeleteAction 对象提供有关删除项目的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93f605e74a0a483a94593a9aaa40d6fd30efe914
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032730"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="3e5cc-103">deleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e5cc-103">deleteAction resource type</span></span>

<span data-ttu-id="3e5cc-104">[**ItemActivity**][activity]上的**deleteAction**资源是否存在指示活动已删除项目。</span><span class="sxs-lookup"><span data-stu-id="3e5cc-104">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="3e5cc-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="3e5cc-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="3e5cc-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e5cc-106">Properties</span></span>

| <span data-ttu-id="3e5cc-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="3e5cc-107">Property name</span></span> | <span data-ttu-id="3e5cc-108">类型</span><span class="sxs-lookup"><span data-stu-id="3e5cc-108">Type</span></span>   | <span data-ttu-id="3e5cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e5cc-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3e5cc-110">name</span><span class="sxs-lookup"><span data-stu-id="3e5cc-110">name</span></span>          | <span data-ttu-id="3e5cc-111">string</span><span class="sxs-lookup"><span data-stu-id="3e5cc-111">string</span></span> | <span data-ttu-id="3e5cc-112">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="3e5cc-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="3e5cc-113">objectType</span><span class="sxs-lookup"><span data-stu-id="3e5cc-113">objectType</span></span>    | <span data-ttu-id="3e5cc-114">string</span><span class="sxs-lookup"><span data-stu-id="3e5cc-114">string</span></span> | <span data-ttu-id="3e5cc-115">`File`或`Folder`, 具体取决于已删除项目的类型。</span><span class="sxs-lookup"><span data-stu-id="3e5cc-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3e5cc-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e5cc-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
