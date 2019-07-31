---
author: daspek
description: itemActivity 上存在 DeleteAction 资源指示活动删除了一个项。
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c5617c61f3221351930ab8d4bf940eaf1efa0629
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973837"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="218f7-103">DeleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="218f7-103">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218f7-104">[**itemActivity**][activity] 上存在 **DeleteAction** 资源指示活动删除了一个项。</span><span class="sxs-lookup"><span data-stu-id="218f7-104">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="218f7-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="218f7-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="218f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="218f7-106">Properties</span></span>

| <span data-ttu-id="218f7-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="218f7-107">Property name</span></span> | <span data-ttu-id="218f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="218f7-108">Type</span></span>   | <span data-ttu-id="218f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="218f7-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="218f7-110">name</span><span class="sxs-lookup"><span data-stu-id="218f7-110">name</span></span>          | <span data-ttu-id="218f7-111">string</span><span class="sxs-lookup"><span data-stu-id="218f7-111">string</span></span> | <span data-ttu-id="218f7-112">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="218f7-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="218f7-113">objectType</span><span class="sxs-lookup"><span data-stu-id="218f7-113">objectType</span></span>    | <span data-ttu-id="218f7-114">string</span><span class="sxs-lookup"><span data-stu-id="218f7-114">string</span></span> | <span data-ttu-id="218f7-115">`File`或`Folder`, 具体取决于已删除项目的类型。</span><span class="sxs-lookup"><span data-stu-id="218f7-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="218f7-116">注解</span><span class="sxs-lookup"><span data-stu-id="218f7-116">Remarks</span></span>

<span data-ttu-id="218f7-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="218f7-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
