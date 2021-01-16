---
title: plannerTeamsPublicationInfo 资源类型
description: 包含有关创建 plannerTask 的发布过程的详细信息。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9db73bb5a914a848f3e19e079321681b22510e8e
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883235"
---
# <a name="plannerteamspublicationinfo-resource-type"></a><span data-ttu-id="fd8f4-103">plannerTeamsPublicationInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd8f4-103">plannerTeamsPublicationInfo resource type</span></span>

<span data-ttu-id="fd8f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd8f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fd8f4-105">包含有关创建 [plannerTask](plannertask.md)的发布过程的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-105">Contains detailed information about the publication process that created a [plannerTask](plannertask.md).</span></span> <span data-ttu-id="fd8f4-106">发布过程基于模板创建任务副本。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-106">A publication process creates copies of tasks based on a template.</span></span> <span data-ttu-id="fd8f4-107">这些任务在多个计划中创建，并且用户具有受限权限;例如，无法删除它们，并且可能会阻止用户编辑某些字段。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-107">These tasks are created in multiple plans, and have restricted permissions for the users; for example, they cannot be deleted and users might be blocked from editing certain fields.</span></span> <span data-ttu-id="fd8f4-108">出版物用于在整个组织中分发任务并集中跟踪任务的进度。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-108">Publication is used to distribute tasks across an organization and track their progress centrally.</span></span>

## <a name="properties"></a><span data-ttu-id="fd8f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd8f4-109">Properties</span></span>
|<span data-ttu-id="fd8f4-110">属性</span><span class="sxs-lookup"><span data-stu-id="fd8f4-110">Property</span></span>|<span data-ttu-id="fd8f4-111">类型</span><span class="sxs-lookup"><span data-stu-id="fd8f4-111">Type</span></span>|<span data-ttu-id="fd8f4-112">Description</span><span class="sxs-lookup"><span data-stu-id="fd8f4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd8f4-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd8f4-113">lastModifiedDateTime</span></span>|<span data-ttu-id="fd8f4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8f4-114">DateTimeOffset</span></span>|<span data-ttu-id="fd8f4-115">上次由发布过程修改此任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-115">The date and time when this task was last modified by the publication process.</span></span> <span data-ttu-id="fd8f4-116">只读。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-116">Read-only.</span></span> |
|<span data-ttu-id="fd8f4-117">publicationId</span><span class="sxs-lookup"><span data-stu-id="fd8f4-117">publicationId</span></span>|<span data-ttu-id="fd8f4-118">String</span><span class="sxs-lookup"><span data-stu-id="fd8f4-118">String</span></span>| <span data-ttu-id="fd8f4-119">出版物的标识符。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-119">The identifier of the publication.</span></span> <span data-ttu-id="fd8f4-120">只读。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-120">Read-only.</span></span>|
|<span data-ttu-id="fd8f4-121">publishedToPlanId</span><span class="sxs-lookup"><span data-stu-id="fd8f4-121">publishedToPlanId</span></span>|<span data-ttu-id="fd8f4-122">String</span><span class="sxs-lookup"><span data-stu-id="fd8f4-122">String</span></span>|<span data-ttu-id="fd8f4-123">plannerPlan **此任务最初** 放置的标识符。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-123">The identifier of the **plannerPlan** this task was originally placed in.</span></span> <span data-ttu-id="fd8f4-124">只读。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-124">Read-only.</span></span> |
|<span data-ttu-id="fd8f4-125">publishingTeamId</span><span class="sxs-lookup"><span data-stu-id="fd8f4-125">publishingTeamId</span></span>|<span data-ttu-id="fd8f4-126">String</span><span class="sxs-lookup"><span data-stu-id="fd8f4-126">String</span></span>| <span data-ttu-id="fd8f4-127">启动发布 [过程的](team.md) 团队的标识符。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-127">The identifier of the [team](team.md) that initiated the publication process.</span></span> <span data-ttu-id="fd8f4-128">只读。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-128">Read-only.</span></span>|
|<span data-ttu-id="fd8f4-129">publishingTeamName</span><span class="sxs-lookup"><span data-stu-id="fd8f4-129">publishingTeamName</span></span>|<span data-ttu-id="fd8f4-130">String</span><span class="sxs-lookup"><span data-stu-id="fd8f4-130">String</span></span>|<span data-ttu-id="fd8f4-131">启动显示名称流程的团队的订阅。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-131">The display name of the team that initiated the publication process.</span></span> <span data-ttu-id="fd8f4-132">此显示名称仅供参考，可能不会表示团队的最新版本名称。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-132">This display name is for reference only, and might not represent the most up-to-date name of the team.</span></span> <span data-ttu-id="fd8f4-133">只读。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-133">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fd8f4-134">关系</span><span class="sxs-lookup"><span data-stu-id="fd8f4-134">Relationships</span></span>
<span data-ttu-id="fd8f4-135">无。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd8f4-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd8f4-136">JSON representation</span></span>
<span data-ttu-id="fd8f4-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd8f4-137">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTeamsPublicationInfo",
  "publicationId": "String",
  "publishingTeamId": "String",
  "publishingTeamName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishedToPlanId": "String"
}
```

