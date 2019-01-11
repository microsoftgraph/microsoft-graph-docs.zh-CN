---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 2ff3e1a2356c43457fe251928728632bd2228b10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809890"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="7c0c8-102">ItemActivityTimeSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c0c8-102">ItemActivityTimeSet resource type</span></span>

> <span data-ttu-id="7c0c8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c0c8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c0c8-105">**ItemActivityTimeSet** 资源提供有关项上某个[活动][activity]发生时间的信息。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7c0c8-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c0c8-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7c0c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="7c0c8-107">Properties</span></span>

| <span data-ttu-id="7c0c8-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="7c0c8-108">Property name</span></span>    | <span data-ttu-id="7c0c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="7c0c8-109">Type</span></span>           | <span data-ttu-id="7c0c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="7c0c8-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="7c0c8-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0c8-111">observedDateTime</span></span> | <span data-ttu-id="7c0c8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0c8-112">DateTimeOffset</span></span> | <span data-ttu-id="7c0c8-113">在观察到要发生活动时。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="7c0c8-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0c8-114">recordedDateTime</span></span> | <span data-ttu-id="7c0c8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0c8-115">DateTimeOffset</span></span> | <span data-ttu-id="7c0c8-116">在服务上记录观察时。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="7c0c8-117">对于离线协作方案来说，**观察**和**记录**时间差异尤为重要。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="7c0c8-118">如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="7c0c8-119">稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="7c0c8-120">注解</span><span class="sxs-lookup"><span data-stu-id="7c0c8-120">Remarks</span></span>

<span data-ttu-id="7c0c8-121">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="7c0c8-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
