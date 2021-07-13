---
title: workloadStatus 资源类型
description: 表示工作负荷的状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 50cbd9cdc59426f413333835c4418112401d8038
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402381"
---
# <a name="workloadstatus-resource-type"></a><span data-ttu-id="9730d-103">workloadStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="9730d-103">workloadStatus resource type</span></span>

<span data-ttu-id="9730d-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9730d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9730d-105">表示工作负荷的状态。</span><span class="sxs-lookup"><span data-stu-id="9730d-105">Represent the status for a workload.</span></span>

## <a name="properties"></a><span data-ttu-id="9730d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9730d-106">Properties</span></span>
|<span data-ttu-id="9730d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9730d-107">Property</span></span>|<span data-ttu-id="9730d-108">类型</span><span class="sxs-lookup"><span data-stu-id="9730d-108">Type</span></span>|<span data-ttu-id="9730d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9730d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9730d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9730d-110">displayName</span></span>|<span data-ttu-id="9730d-111">String</span><span class="sxs-lookup"><span data-stu-id="9730d-111">String</span></span>|<span data-ttu-id="9730d-112">工作负荷显示名称的负载。</span><span class="sxs-lookup"><span data-stu-id="9730d-112">The display name for the workload.</span></span> <span data-ttu-id="9730d-113">必填。</span><span class="sxs-lookup"><span data-stu-id="9730d-113">Required.</span></span> <span data-ttu-id="9730d-114">只读。</span><span class="sxs-lookup"><span data-stu-id="9730d-114">Read-only.</span></span>|
|<span data-ttu-id="9730d-115">offboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="9730d-115">offboardedDateTime</span></span>|<span data-ttu-id="9730d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9730d-116">DateTimeOffset</span></span>|<span data-ttu-id="9730d-117">工作负荷从载出的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9730d-117">The date and time the workload was offboarded.</span></span> <span data-ttu-id="9730d-118">可选。</span><span class="sxs-lookup"><span data-stu-id="9730d-118">Optional.</span></span> <span data-ttu-id="9730d-119">只读。</span><span class="sxs-lookup"><span data-stu-id="9730d-119">Read-only.</span></span>|
|<span data-ttu-id="9730d-120">onboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="9730d-120">onboardedDateTime</span></span>|<span data-ttu-id="9730d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9730d-121">DateTimeOffset</span></span>|<span data-ttu-id="9730d-122">载入工作负荷的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9730d-122">The date and time the workload was onboarded.</span></span> <span data-ttu-id="9730d-123">可选。</span><span class="sxs-lookup"><span data-stu-id="9730d-123">Optional.</span></span> <span data-ttu-id="9730d-124">只读。</span><span class="sxs-lookup"><span data-stu-id="9730d-124">Read-only.</span></span>|
|<span data-ttu-id="9730d-125">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="9730d-125">onboardingStatus</span></span>|<span data-ttu-id="9730d-126">workloadOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="9730d-126">workloadOnboardingStatus</span></span>|<span data-ttu-id="9730d-127">工作负荷的载入状态。</span><span class="sxs-lookup"><span data-stu-id="9730d-127">The onboarding status for the workload.</span></span> <span data-ttu-id="9730d-128">可取值为：`notOnboarded`、`onboarded`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9730d-128">Possible values are: `notOnboarded`, `onboarded`, `unknownFutureValue`.</span></span> <span data-ttu-id="9730d-129">可选。</span><span class="sxs-lookup"><span data-stu-id="9730d-129">Optional.</span></span> <span data-ttu-id="9730d-130">只读。</span><span class="sxs-lookup"><span data-stu-id="9730d-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9730d-131">关系</span><span class="sxs-lookup"><span data-stu-id="9730d-131">Relationships</span></span>
<span data-ttu-id="9730d-132">无。</span><span class="sxs-lookup"><span data-stu-id="9730d-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9730d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9730d-133">JSON representation</span></span>
<span data-ttu-id="9730d-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9730d-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadStatus",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "displayName": "String",
  "offboardedDateTime": "String (timestamp)"
}
```
