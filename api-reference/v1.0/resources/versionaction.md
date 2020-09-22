---
author: daspek
ms.author: dspektor
title: versionAction 资源类型
description: VersionAction 对象提供有关导致新项目版本的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 94efbb554420030eb33a814de72d5d79ab065738
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015279"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="b0ce4-103">versionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0ce4-103">versionAction resource type</span></span>

<span data-ttu-id="b0ce4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0ce4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0ce4-105">[**ItemActivity**][activity]上的**versionAction**资源存在指示活动导致创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="b0ce4-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="b0ce4-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b0ce4-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b0ce4-107">属性</span><span class="sxs-lookup"><span data-stu-id="b0ce4-107">Properties</span></span>

| <span data-ttu-id="b0ce4-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="b0ce4-108">Property name</span></span> | <span data-ttu-id="b0ce4-109">类型</span><span class="sxs-lookup"><span data-stu-id="b0ce4-109">Type</span></span>   | <span data-ttu-id="b0ce4-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0ce4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b0ce4-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="b0ce4-111">newVersion</span></span>    | <span data-ttu-id="b0ce4-112">string</span><span class="sxs-lookup"><span data-stu-id="b0ce4-112">string</span></span> | <span data-ttu-id="b0ce4-113">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="b0ce4-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ce4-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0ce4-114">JSON representation</span></span>

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

