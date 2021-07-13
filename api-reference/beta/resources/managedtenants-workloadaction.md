---
title: workloadAction 资源类型
description: 表示将为特定工作负荷执行的操作。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e6dbbe1458aa6dba37a26af70ee0e64b92a52cf4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402088"
---
# <a name="workloadaction-resource-type"></a><span data-ttu-id="d623b-103">workloadAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="d623b-103">workloadAction resource type</span></span>

<span data-ttu-id="d623b-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d623b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d623b-105">表示将为特定工作负荷执行的操作。</span><span class="sxs-lookup"><span data-stu-id="d623b-105">Represents an action that will be performed for a specific workload.</span></span>

## <a name="properties"></a><span data-ttu-id="d623b-106">属性</span><span class="sxs-lookup"><span data-stu-id="d623b-106">Properties</span></span>
|<span data-ttu-id="d623b-107">属性</span><span class="sxs-lookup"><span data-stu-id="d623b-107">Property</span></span>|<span data-ttu-id="d623b-108">类型</span><span class="sxs-lookup"><span data-stu-id="d623b-108">Type</span></span>|<span data-ttu-id="d623b-109">说明</span><span class="sxs-lookup"><span data-stu-id="d623b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d623b-110">actionId</span><span class="sxs-lookup"><span data-stu-id="d623b-110">actionId</span></span>|<span data-ttu-id="d623b-111">String</span><span class="sxs-lookup"><span data-stu-id="d623b-111">String</span></span>|<span data-ttu-id="d623b-112">工作负荷操作的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d623b-112">The unique identifier for the workload action.</span></span> <span data-ttu-id="d623b-113">必填。</span><span class="sxs-lookup"><span data-stu-id="d623b-113">Required.</span></span> <span data-ttu-id="d623b-114">只读。</span><span class="sxs-lookup"><span data-stu-id="d623b-114">Read-only.</span></span>|
|<span data-ttu-id="d623b-115">“类别”</span><span class="sxs-lookup"><span data-stu-id="d623b-115">category</span></span>|<span data-ttu-id="d623b-116">workloadActionCategory</span><span class="sxs-lookup"><span data-stu-id="d623b-116">workloadActionCategory</span></span>|<span data-ttu-id="d623b-117">工作负荷操作类别。</span><span class="sxs-lookup"><span data-stu-id="d623b-117">The category for the workload action.</span></span> <span data-ttu-id="d623b-118">可取值为：`automated`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d623b-118">Possible values are: `automated`, `manual`, `unknownFutureValue`.</span></span> <span data-ttu-id="d623b-119">可选。</span><span class="sxs-lookup"><span data-stu-id="d623b-119">Optional.</span></span> <span data-ttu-id="d623b-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d623b-120">Read-only.</span></span>|
|<span data-ttu-id="d623b-121">说明</span><span class="sxs-lookup"><span data-stu-id="d623b-121">description</span></span>|<span data-ttu-id="d623b-122">String</span><span class="sxs-lookup"><span data-stu-id="d623b-122">String</span></span>|<span data-ttu-id="d623b-123">工作负荷操作的说明。</span><span class="sxs-lookup"><span data-stu-id="d623b-123">The description for the workload action.</span></span> <span data-ttu-id="d623b-124">可选。</span><span class="sxs-lookup"><span data-stu-id="d623b-124">Optional.</span></span> <span data-ttu-id="d623b-125">只读。</span><span class="sxs-lookup"><span data-stu-id="d623b-125">Read-only.</span></span>|
|<span data-ttu-id="d623b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d623b-126">displayName</span></span>|<span data-ttu-id="d623b-127">String</span><span class="sxs-lookup"><span data-stu-id="d623b-127">String</span></span>|<span data-ttu-id="d623b-128">工作负荷显示名称的项。</span><span class="sxs-lookup"><span data-stu-id="d623b-128">The display name for the workload action.</span></span> <span data-ttu-id="d623b-129">可选。</span><span class="sxs-lookup"><span data-stu-id="d623b-129">Optional.</span></span> <span data-ttu-id="d623b-130">只读。</span><span class="sxs-lookup"><span data-stu-id="d623b-130">Read-only.</span></span>|
|<span data-ttu-id="d623b-131">service</span><span class="sxs-lookup"><span data-stu-id="d623b-131">service</span></span>|<span data-ttu-id="d623b-132">String</span><span class="sxs-lookup"><span data-stu-id="d623b-132">String</span></span>|<span data-ttu-id="d623b-133">与工作负荷操作关联的服务。</span><span class="sxs-lookup"><span data-stu-id="d623b-133">The service associated with workload action.</span></span> <span data-ttu-id="d623b-134">可选。</span><span class="sxs-lookup"><span data-stu-id="d623b-134">Optional.</span></span> <span data-ttu-id="d623b-135">只读。</span><span class="sxs-lookup"><span data-stu-id="d623b-135">Read-only.</span></span>|
|<span data-ttu-id="d623b-136">settings</span><span class="sxs-lookup"><span data-stu-id="d623b-136">settings</span></span>|<span data-ttu-id="d623b-137">[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d623b-137">[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection</span></span>|<span data-ttu-id="d623b-138">与工作负荷操作关联的设置集合。</span><span class="sxs-lookup"><span data-stu-id="d623b-138">The collection of settings associated with the workload action.</span></span> <span data-ttu-id="d623b-139">可选。</span><span class="sxs-lookup"><span data-stu-id="d623b-139">Optional.</span></span> <span data-ttu-id="d623b-140">只读。</span><span class="sxs-lookup"><span data-stu-id="d623b-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d623b-141">关系</span><span class="sxs-lookup"><span data-stu-id="d623b-141">Relationships</span></span>
<span data-ttu-id="d623b-142">无。</span><span class="sxs-lookup"><span data-stu-id="d623b-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d623b-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d623b-143">JSON representation</span></span>
<span data-ttu-id="d623b-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d623b-144">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadAction",
  "actionId": "String",
  "category": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```
