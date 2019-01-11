---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
ms.openlocfilehash: ebdcabf51017bb407090d9ab4690b9e693a12953
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866057"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="0ecc9-102">CreateAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ecc9-102">CreateAction resource type</span></span>

> <span data-ttu-id="0ecc9-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ecc9-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ecc9-105">[**itemActivity**][activity] 上存在 **CreateAction** 资源指示活动已创建一个项。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-105">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="0ecc9-106">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0ecc9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ecc9-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="0ecc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ecc9-108">Properties</span></span>

<span data-ttu-id="0ecc9-109">无。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-109">None.</span></span> <span data-ttu-id="0ecc9-110">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0ecc9-111">注解</span><span class="sxs-lookup"><span data-stu-id="0ecc9-111">Remarks</span></span>

<span data-ttu-id="0ecc9-112">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="0ecc9-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction"
} -->
