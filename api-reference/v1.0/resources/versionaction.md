---
author: daspek
ms.author: dspektor
title: versionAction 资源类型
description: VersionAction 对象提供有关导致新项目版本的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: cde5c906c41972950431d5219bea73e4095f74e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533416"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="f2912-103">versionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2912-103">versionAction resource type</span></span>

<span data-ttu-id="f2912-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2912-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2912-105">[**ItemActivity**][activity]上的**versionAction**资源存在指示活动导致创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="f2912-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="f2912-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="f2912-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="f2912-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2912-107">Properties</span></span>

| <span data-ttu-id="f2912-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="f2912-108">Property name</span></span> | <span data-ttu-id="f2912-109">类型</span><span class="sxs-lookup"><span data-stu-id="f2912-109">Type</span></span>   | <span data-ttu-id="f2912-110">说明</span><span class="sxs-lookup"><span data-stu-id="f2912-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f2912-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="f2912-111">newVersion</span></span>    | <span data-ttu-id="f2912-112">string</span><span class="sxs-lookup"><span data-stu-id="f2912-112">string</span></span> | <span data-ttu-id="f2912-113">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="f2912-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2912-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2912-114">JSON representation</span></span>

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
