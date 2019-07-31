---
author: daspek
description: itemActivity 上存在 CreateAction 资源指示活动已创建一个项。
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e47a57e392ef629730a9de68c973d54b2ab5c2fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973179"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="988bf-103">CreateAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="988bf-103">CreateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="988bf-104">[**itemActivity**][activity] 上存在 **CreateAction** 资源指示活动已创建一个项。</span><span class="sxs-lookup"><span data-stu-id="988bf-104">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="988bf-105">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="988bf-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="988bf-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="988bf-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="988bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="988bf-107">Properties</span></span>

<span data-ttu-id="988bf-108">无。</span><span class="sxs-lookup"><span data-stu-id="988bf-108">None.</span></span> <span data-ttu-id="988bf-109">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="988bf-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="988bf-110">注解</span><span class="sxs-lookup"><span data-stu-id="988bf-110">Remarks</span></span>

<span data-ttu-id="988bf-111">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="988bf-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": []
}
-->
