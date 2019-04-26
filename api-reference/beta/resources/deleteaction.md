---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: a380376a813df5f519464978851049e020ded8b8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340947"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="5e171-102">DeleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e171-102">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e171-103">[**itemActivity**][activity] 上存在 **DeleteAction** 资源指示活动删除了一个项。</span><span class="sxs-lookup"><span data-stu-id="5e171-103">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5e171-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e171-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5e171-105">属性</span><span class="sxs-lookup"><span data-stu-id="5e171-105">Properties</span></span>

| <span data-ttu-id="5e171-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="5e171-106">Property name</span></span> | <span data-ttu-id="5e171-107">类型</span><span class="sxs-lookup"><span data-stu-id="5e171-107">Type</span></span>   | <span data-ttu-id="5e171-108">说明</span><span class="sxs-lookup"><span data-stu-id="5e171-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5e171-109">name</span><span class="sxs-lookup"><span data-stu-id="5e171-109">name</span></span>          | <span data-ttu-id="5e171-110">string</span><span class="sxs-lookup"><span data-stu-id="5e171-110">string</span></span> | <span data-ttu-id="5e171-111">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="5e171-111">The name of the item that was deleted.</span></span>
| <span data-ttu-id="5e171-112">objectType</span><span class="sxs-lookup"><span data-stu-id="5e171-112">objectType</span></span>    | <span data-ttu-id="5e171-113">string</span><span class="sxs-lookup"><span data-stu-id="5e171-113">string</span></span> | <span data-ttu-id="5e171-114">`File`或`Folder`, 具体取决于已删除项目的类型。</span><span class="sxs-lookup"><span data-stu-id="5e171-114">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="5e171-115">注解</span><span class="sxs-lookup"><span data-stu-id="5e171-115">Remarks</span></span>

<span data-ttu-id="5e171-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="5e171-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
