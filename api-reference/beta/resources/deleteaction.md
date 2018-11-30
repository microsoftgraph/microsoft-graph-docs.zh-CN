---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
ms.openlocfilehash: 041552f88561981338fa2ea5719d5af102fb3574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043981"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="b22f8-102">DeleteAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b22f8-102">DeleteAction resource type</span></span>

> <span data-ttu-id="b22f8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b22f8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b22f8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b22f8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b22f8-105">[**itemActivity**][activity] 上存在 **DeleteAction** 资源指示活动删除了一个项。</span><span class="sxs-lookup"><span data-stu-id="b22f8-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b22f8-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b22f8-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b22f8-107">属性</span><span class="sxs-lookup"><span data-stu-id="b22f8-107">Properties</span></span>

| <span data-ttu-id="b22f8-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="b22f8-108">Property name</span></span> | <span data-ttu-id="b22f8-109">类型</span><span class="sxs-lookup"><span data-stu-id="b22f8-109">Type</span></span>   | <span data-ttu-id="b22f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="b22f8-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b22f8-111">name</span><span class="sxs-lookup"><span data-stu-id="b22f8-111">name</span></span>          | <span data-ttu-id="b22f8-112">string</span><span class="sxs-lookup"><span data-stu-id="b22f8-112">string</span></span> | <span data-ttu-id="b22f8-113">已删除的项的名称。</span><span class="sxs-lookup"><span data-stu-id="b22f8-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="b22f8-114">objectType</span><span class="sxs-lookup"><span data-stu-id="b22f8-114">objectType</span></span>    | <span data-ttu-id="b22f8-115">string</span><span class="sxs-lookup"><span data-stu-id="b22f8-115">string</span></span> | <span data-ttu-id="b22f8-116">`File`或`Folder`，具体取决于已删除的项目的类型。</span><span class="sxs-lookup"><span data-stu-id="b22f8-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="b22f8-117">注解</span><span class="sxs-lookup"><span data-stu-id="b22f8-117">Remarks</span></span>

<span data-ttu-id="b22f8-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b22f8-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
