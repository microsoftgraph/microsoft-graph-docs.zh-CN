---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 474d20e08d96294a30029e764d0b01f5b0c6bfcd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518511"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="d17fd-102">ItemActivityTimeSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="d17fd-102">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d17fd-103">**ItemActivityTimeSet** 资源提供有关项上某个[活动][activity]发生时间的信息。</span><span class="sxs-lookup"><span data-stu-id="d17fd-103">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="d17fd-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d17fd-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d17fd-105">属性</span><span class="sxs-lookup"><span data-stu-id="d17fd-105">Properties</span></span>

| <span data-ttu-id="d17fd-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="d17fd-106">Property name</span></span>    | <span data-ttu-id="d17fd-107">类型</span><span class="sxs-lookup"><span data-stu-id="d17fd-107">Type</span></span>           | <span data-ttu-id="d17fd-108">说明</span><span class="sxs-lookup"><span data-stu-id="d17fd-108">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="d17fd-109">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="d17fd-109">observedDateTime</span></span> | <span data-ttu-id="d17fd-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17fd-110">DateTimeOffset</span></span> | <span data-ttu-id="d17fd-111">在观察到要发生活动时。</span><span class="sxs-lookup"><span data-stu-id="d17fd-111">When the activity was observed to take place.</span></span>
| <span data-ttu-id="d17fd-112">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="d17fd-112">recordedDateTime</span></span> | <span data-ttu-id="d17fd-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17fd-113">DateTimeOffset</span></span> | <span data-ttu-id="d17fd-114">在服务上记录观察时。</span><span class="sxs-lookup"><span data-stu-id="d17fd-114">When the observation was recorded on the service.</span></span>

<span data-ttu-id="d17fd-115">对于离线协作方案来说，**观察**和**记录**时间差异尤为重要。</span><span class="sxs-lookup"><span data-stu-id="d17fd-115">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="d17fd-116">如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="d17fd-116">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="d17fd-117">稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="d17fd-117">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="d17fd-118">注解</span><span class="sxs-lookup"><span data-stu-id="d17fd-118">Remarks</span></span>

<span data-ttu-id="d17fd-119">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="d17fd-119">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitytimeset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
