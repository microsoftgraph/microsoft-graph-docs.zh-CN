---
author: daspek
ms.author: dspektor
title: itemActivityTimeSet 资源类型
description: ItemActionSet 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9dce21afc1acc8e93181204e026f74a597c9120f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036587"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="13f37-103">itemActivityTimeSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="13f37-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="13f37-104">**ItemActivityTimeSet**资源提供有关何时发生某个项目的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="13f37-104">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="13f37-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="13f37-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="13f37-106">属性</span><span class="sxs-lookup"><span data-stu-id="13f37-106">Properties</span></span>

| <span data-ttu-id="13f37-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="13f37-107">Property name</span></span>    | <span data-ttu-id="13f37-108">类型</span><span class="sxs-lookup"><span data-stu-id="13f37-108">Type</span></span>           | <span data-ttu-id="13f37-109">说明</span><span class="sxs-lookup"><span data-stu-id="13f37-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="13f37-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="13f37-110">observedDateTime</span></span> | <span data-ttu-id="13f37-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f37-111">DateTimeOffset</span></span> | <span data-ttu-id="13f37-112">在观察到要发生活动时。</span><span class="sxs-lookup"><span data-stu-id="13f37-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="13f37-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="13f37-113">recordedDateTime</span></span> | <span data-ttu-id="13f37-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f37-114">DateTimeOffset</span></span> | <span data-ttu-id="13f37-115">在服务上记录观察时。</span><span class="sxs-lookup"><span data-stu-id="13f37-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="13f37-116">对于离线协作方案来说，**观察**和**记录**时间差异尤为重要。</span><span class="sxs-lookup"><span data-stu-id="13f37-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="13f37-117">如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="13f37-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="13f37-118">稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="13f37-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13f37-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13f37-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
