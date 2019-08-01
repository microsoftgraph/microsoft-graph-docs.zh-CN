---
author: daspek
ms.author: dspektor
title: versionAction 资源类型
description: VersionAction 对象提供有关导致新项目版本的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 22f06691824d2ffa5b773a796b4c456cb2fcaecc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033444"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="b999a-103">versionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b999a-103">versionAction resource type</span></span>

<span data-ttu-id="b999a-104">[**ItemActivity**][activity]上的**versionAction**资源存在指示活动导致创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="b999a-104">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="b999a-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b999a-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b999a-106">属性</span><span class="sxs-lookup"><span data-stu-id="b999a-106">Properties</span></span>

| <span data-ttu-id="b999a-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="b999a-107">Property name</span></span> | <span data-ttu-id="b999a-108">类型</span><span class="sxs-lookup"><span data-stu-id="b999a-108">Type</span></span>   | <span data-ttu-id="b999a-109">说明</span><span class="sxs-lookup"><span data-stu-id="b999a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b999a-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="b999a-110">newVersion</span></span>    | <span data-ttu-id="b999a-111">string</span><span class="sxs-lookup"><span data-stu-id="b999a-111">string</span></span> | <span data-ttu-id="b999a-112">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="b999a-112">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b999a-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b999a-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->
