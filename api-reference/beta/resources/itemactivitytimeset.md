---
author: daspek
description: ItemActivityTimeSet 资源提供有关项上某个活动发生时间的信息。
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 33a9f4c42393c0c77c331889d8e77244de6226e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523105"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="5442d-103">ItemActivityTimeSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="5442d-103">ItemActivityTimeSet resource type</span></span>

<span data-ttu-id="5442d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5442d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5442d-105">**ItemActivityTimeSet** 资源提供有关项上某个[活动][activity]发生时间的信息。</span><span class="sxs-lookup"><span data-stu-id="5442d-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5442d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5442d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5442d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5442d-107">Properties</span></span>

| <span data-ttu-id="5442d-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="5442d-108">Property name</span></span>    | <span data-ttu-id="5442d-109">类型</span><span class="sxs-lookup"><span data-stu-id="5442d-109">Type</span></span>           | <span data-ttu-id="5442d-110">说明</span><span class="sxs-lookup"><span data-stu-id="5442d-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="5442d-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="5442d-111">observedDateTime</span></span> | <span data-ttu-id="5442d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5442d-112">DateTimeOffset</span></span> | <span data-ttu-id="5442d-113">在观察到要发生活动时。</span><span class="sxs-lookup"><span data-stu-id="5442d-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="5442d-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="5442d-114">recordedDateTime</span></span> | <span data-ttu-id="5442d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5442d-115">DateTimeOffset</span></span> | <span data-ttu-id="5442d-116">在服务上记录观察时。</span><span class="sxs-lookup"><span data-stu-id="5442d-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="5442d-117">对于离线协作方案来说，**观察**和**记录**时间差异尤为重要。</span><span class="sxs-lookup"><span data-stu-id="5442d-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="5442d-118">如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="5442d-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="5442d-119">稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="5442d-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="5442d-120">注解</span><span class="sxs-lookup"><span data-stu-id="5442d-120">Remarks</span></span>

<span data-ttu-id="5442d-121">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="5442d-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
