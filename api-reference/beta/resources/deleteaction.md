---
author: daspek
description: itemActivity 上存在 DeleteAction 资源指示活动删除了一个项。
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b8f00827a37ba9c010acd1b52e751bd55638afb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049882"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="40df7-103">DeleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="40df7-103">DeleteAction resource type</span></span>

<span data-ttu-id="40df7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40df7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40df7-105">[**itemActivity**][activity] 上存在 **DeleteAction** 资源指示活动删除了一个项。</span><span class="sxs-lookup"><span data-stu-id="40df7-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="40df7-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40df7-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="40df7-107">属性</span><span class="sxs-lookup"><span data-stu-id="40df7-107">Properties</span></span>

| <span data-ttu-id="40df7-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="40df7-108">Property name</span></span> | <span data-ttu-id="40df7-109">类型</span><span class="sxs-lookup"><span data-stu-id="40df7-109">Type</span></span>   | <span data-ttu-id="40df7-110">说明</span><span class="sxs-lookup"><span data-stu-id="40df7-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="40df7-111">name</span><span class="sxs-lookup"><span data-stu-id="40df7-111">name</span></span>          | <span data-ttu-id="40df7-112">string</span><span class="sxs-lookup"><span data-stu-id="40df7-112">string</span></span> | <span data-ttu-id="40df7-113">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="40df7-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="40df7-114">objectType</span><span class="sxs-lookup"><span data-stu-id="40df7-114">objectType</span></span>    | <span data-ttu-id="40df7-115">string</span><span class="sxs-lookup"><span data-stu-id="40df7-115">string</span></span> | <span data-ttu-id="40df7-116">`File` 或 `Folder` ，具体取决于已删除项目的类型。</span><span class="sxs-lookup"><span data-stu-id="40df7-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="40df7-117">注解</span><span class="sxs-lookup"><span data-stu-id="40df7-117">Remarks</span></span>

<span data-ttu-id="40df7-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="40df7-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


