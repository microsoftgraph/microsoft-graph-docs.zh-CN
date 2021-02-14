---
author: daspek
title: itemActivityTimeSet 资源类型
description: itemActionSet 对象提供有关在项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1f614c597efdb95b04c4079bd68240aa865d66dd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238671"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="cc707-103">itemActivityTimeSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc707-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="cc707-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc707-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc707-105">**itemActivityTimeSet** 资源提供有关何时 [发生项目活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="cc707-105">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="cc707-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="cc707-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="cc707-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc707-107">Properties</span></span>

| <span data-ttu-id="cc707-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="cc707-108">Property name</span></span>    | <span data-ttu-id="cc707-109">类型</span><span class="sxs-lookup"><span data-stu-id="cc707-109">Type</span></span>           | <span data-ttu-id="cc707-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc707-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="cc707-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc707-111">observedDateTime</span></span> | <span data-ttu-id="cc707-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc707-112">DateTimeOffset</span></span> | <span data-ttu-id="cc707-113">在观察到要发生活动时。</span><span class="sxs-lookup"><span data-stu-id="cc707-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="cc707-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc707-114">recordedDateTime</span></span> | <span data-ttu-id="cc707-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc707-115">DateTimeOffset</span></span> | <span data-ttu-id="cc707-116">在服务上记录观察时。</span><span class="sxs-lookup"><span data-stu-id="cc707-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="cc707-117">对于离线协作方案来说，**观察** 和 **记录** 时间差异尤为重要。</span><span class="sxs-lookup"><span data-stu-id="cc707-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="cc707-118">如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="cc707-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="cc707-119">稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="cc707-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc707-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc707-120">JSON representation</span></span>

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

