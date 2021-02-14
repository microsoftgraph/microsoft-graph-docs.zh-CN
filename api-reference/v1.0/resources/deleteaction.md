---
author: daspek
title: deleteAction 资源类型
description: deleteAction 对象提供有关删除项目的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e78b4369606b0e0e3880fc3bfd13fdec263fcb58
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239630"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="6a070-103">deleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a070-103">deleteAction resource type</span></span>

<span data-ttu-id="6a070-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a070-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a070-105">itemActivity 上 **存在 deleteAction** [][activity]资源表示活动已删除项目。</span><span class="sxs-lookup"><span data-stu-id="6a070-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="6a070-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="6a070-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="6a070-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a070-107">Properties</span></span>

| <span data-ttu-id="6a070-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="6a070-108">Property name</span></span> | <span data-ttu-id="6a070-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a070-109">Type</span></span>   | <span data-ttu-id="6a070-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a070-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6a070-111">name</span><span class="sxs-lookup"><span data-stu-id="6a070-111">name</span></span>          | <span data-ttu-id="6a070-112">string</span><span class="sxs-lookup"><span data-stu-id="6a070-112">string</span></span> | <span data-ttu-id="6a070-113">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="6a070-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="6a070-114">objectType</span><span class="sxs-lookup"><span data-stu-id="6a070-114">objectType</span></span>    | <span data-ttu-id="6a070-115">string</span><span class="sxs-lookup"><span data-stu-id="6a070-115">string</span></span> | <span data-ttu-id="6a070-116">`File``Folder`或 ，具体取决于已删除项目的类型。</span><span class="sxs-lookup"><span data-stu-id="6a070-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6a070-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a070-117">JSON representation</span></span>

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

