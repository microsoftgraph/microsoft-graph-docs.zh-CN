---
author: daspek
ms.author: dspektor
title: deleteAction 资源类型
description: DeleteAction 对象提供有关删除项目的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d19b41d886c459822abc2ea1b04acebd94c7b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531689"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="45a30-103">deleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="45a30-103">deleteAction resource type</span></span>

<span data-ttu-id="45a30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45a30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45a30-105">[**ItemActivity**][activity]上的**deleteAction**资源是否存在指示活动已删除项目。</span><span class="sxs-lookup"><span data-stu-id="45a30-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="45a30-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="45a30-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="45a30-107">属性</span><span class="sxs-lookup"><span data-stu-id="45a30-107">Properties</span></span>

| <span data-ttu-id="45a30-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="45a30-108">Property name</span></span> | <span data-ttu-id="45a30-109">类型</span><span class="sxs-lookup"><span data-stu-id="45a30-109">Type</span></span>   | <span data-ttu-id="45a30-110">说明</span><span class="sxs-lookup"><span data-stu-id="45a30-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="45a30-111">name</span><span class="sxs-lookup"><span data-stu-id="45a30-111">name</span></span>          | <span data-ttu-id="45a30-112">string</span><span class="sxs-lookup"><span data-stu-id="45a30-112">string</span></span> | <span data-ttu-id="45a30-113">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="45a30-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="45a30-114">objectType</span><span class="sxs-lookup"><span data-stu-id="45a30-114">objectType</span></span>    | <span data-ttu-id="45a30-115">字符串</span><span class="sxs-lookup"><span data-stu-id="45a30-115">string</span></span> | <span data-ttu-id="45a30-116">`File`或`Folder`，具体取决于已删除项目的类型。</span><span class="sxs-lookup"><span data-stu-id="45a30-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="45a30-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45a30-117">JSON representation</span></span>

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
