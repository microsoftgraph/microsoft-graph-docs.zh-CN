---
author: daspek
description: ItemActivityTimeSet 资源提供有关项上某个活动发生时间的信息。
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c81bf7885ee1466e293236a987e90e21323daefd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010089"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="29d30-103">ItemActivityTimeSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="29d30-103">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29d30-104">**ItemActivityTimeSet** 资源提供有关项上某个[活动][activity]发生时间的信息。</span><span class="sxs-lookup"><span data-stu-id="29d30-104">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="29d30-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29d30-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="29d30-106">属性</span><span class="sxs-lookup"><span data-stu-id="29d30-106">Properties</span></span>

| <span data-ttu-id="29d30-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="29d30-107">Property name</span></span>    | <span data-ttu-id="29d30-108">类型</span><span class="sxs-lookup"><span data-stu-id="29d30-108">Type</span></span>           | <span data-ttu-id="29d30-109">说明</span><span class="sxs-lookup"><span data-stu-id="29d30-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="29d30-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="29d30-110">observedDateTime</span></span> | <span data-ttu-id="29d30-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d30-111">DateTimeOffset</span></span> | <span data-ttu-id="29d30-112">在观察到要发生活动时。</span><span class="sxs-lookup"><span data-stu-id="29d30-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="29d30-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="29d30-113">recordedDateTime</span></span> | <span data-ttu-id="29d30-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d30-114">DateTimeOffset</span></span> | <span data-ttu-id="29d30-115">在服务上记录观察时。</span><span class="sxs-lookup"><span data-stu-id="29d30-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="29d30-116">对于离线协作方案来说，**观察**和**记录**时间差异尤为重要。</span><span class="sxs-lookup"><span data-stu-id="29d30-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="29d30-117">如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="29d30-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="29d30-118">稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="29d30-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="29d30-119">注解</span><span class="sxs-lookup"><span data-stu-id="29d30-119">Remarks</span></span>

<span data-ttu-id="29d30-120">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="29d30-120">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
