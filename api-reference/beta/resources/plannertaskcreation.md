---
title: plannerTaskCreation 资源类型
description: 包含有关 plannerTask 来源的信息。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8a2a4bf3aae5f23a04c7ecb8ad043631f946b20
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883236"
---
# <a name="plannertaskcreation-resource-type"></a><span data-ttu-id="9ffad-103">plannerTaskCreation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ffad-103">plannerTaskCreation resource type</span></span>

<span data-ttu-id="9ffad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ffad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ffad-105">包含有关 [plannerTask](plannerTask.md)的源的信息。</span><span class="sxs-lookup"><span data-stu-id="9ffad-105">Contains information about the origin of the [plannerTask](plannerTask.md).</span></span> <span data-ttu-id="9ffad-106">此资源将设置其所有属性，或者只有一个属性将具有一个值，该值指示任务由该属性描述的进程 `null` 创建。</span><span class="sxs-lookup"><span data-stu-id="9ffad-106">This resource will either have all its properties set to `null`, or exactly one property will have a value that indicates that the task was created by the process described by that property.</span></span> <span data-ttu-id="9ffad-107">所有 `null` 属性都表示该任务不是由任何专用进程创建的。</span><span class="sxs-lookup"><span data-stu-id="9ffad-107">All properties `null` indicates this task was not created by any specialized process.</span></span> <span data-ttu-id="9ffad-108">应用无需知道任务的来源，就可以处理它;但是，某些应用可以使用其他信息来提供有关这些任务的特定体验。</span><span class="sxs-lookup"><span data-stu-id="9ffad-108">Apps do not need to know the origin of the task to be able to work with it; however, some apps can use the additional information to provide specific experiences around these tasks.</span></span> <span data-ttu-id="9ffad-109">有关详细信息，请参阅特定资源的文档。</span><span class="sxs-lookup"><span data-stu-id="9ffad-109">See the documentation for specific resources to learn more.</span></span>

## <a name="properties"></a><span data-ttu-id="9ffad-110">属性</span><span class="sxs-lookup"><span data-stu-id="9ffad-110">Properties</span></span>
|<span data-ttu-id="9ffad-111">属性</span><span class="sxs-lookup"><span data-stu-id="9ffad-111">Property</span></span>|<span data-ttu-id="9ffad-112">类型</span><span class="sxs-lookup"><span data-stu-id="9ffad-112">Type</span></span>|<span data-ttu-id="9ffad-113">Description</span><span class="sxs-lookup"><span data-stu-id="9ffad-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ffad-114">teamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="9ffad-114">teamsPublicationInfo</span></span>|[<span data-ttu-id="9ffad-115">plannerTeamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="9ffad-115">plannerTeamsPublicationInfo</span></span>](../resources/plannerteamspublicationinfo.md)|<span data-ttu-id="9ffad-116">有关创建此任务的发布过程的信息。</span><span class="sxs-lookup"><span data-stu-id="9ffad-116">Information about the publication process that created this task.</span></span> <span data-ttu-id="9ffad-117">`null` 值表示该任务不是由发布过程创建的。</span><span class="sxs-lookup"><span data-stu-id="9ffad-117">`null` value indicates that the task was not created by a publication process.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ffad-118">关系</span><span class="sxs-lookup"><span data-stu-id="9ffad-118">Relationships</span></span>
<span data-ttu-id="9ffad-119">无。</span><span class="sxs-lookup"><span data-stu-id="9ffad-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ffad-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ffad-120">JSON representation</span></span>
<span data-ttu-id="9ffad-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ffad-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTaskCreation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskCreation",
  "teamsPublicationInfo": {
    "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
  }
}
```

