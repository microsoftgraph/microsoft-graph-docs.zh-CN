---
title: managementActionDeploymentStatus 资源类型
description: 表示给定托管租户的部署状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: efd789a7b4b48098e8d679273da1152f6611a28c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402308"
---
# <a name="managementactiondeploymentstatus-resource-type"></a><span data-ttu-id="e7d07-103">managementActionDeploymentStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7d07-103">managementActionDeploymentStatus resource type</span></span>

<span data-ttu-id="e7d07-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e7d07-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d07-105">表示给定托管租户的部署状态。</span><span class="sxs-lookup"><span data-stu-id="e7d07-105">Represents the deployment status for a given managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="e7d07-106">属性</span><span class="sxs-lookup"><span data-stu-id="e7d07-106">Properties</span></span>
|<span data-ttu-id="e7d07-107">属性</span><span class="sxs-lookup"><span data-stu-id="e7d07-107">Property</span></span>|<span data-ttu-id="e7d07-108">类型</span><span class="sxs-lookup"><span data-stu-id="e7d07-108">Type</span></span>|<span data-ttu-id="e7d07-109">说明</span><span class="sxs-lookup"><span data-stu-id="e7d07-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d07-110">managementActionId</span><span class="sxs-lookup"><span data-stu-id="e7d07-110">managementActionId</span></span>|<span data-ttu-id="e7d07-111">String</span><span class="sxs-lookup"><span data-stu-id="e7d07-111">String</span></span>|<span data-ttu-id="e7d07-112">管理操作标识符。</span><span class="sxs-lookup"><span data-stu-id="e7d07-112">The identifier for the management action.</span></span> <span data-ttu-id="e7d07-113">必填。</span><span class="sxs-lookup"><span data-stu-id="e7d07-113">Required.</span></span> <span data-ttu-id="e7d07-114">只读。</span><span class="sxs-lookup"><span data-stu-id="e7d07-114">Read-only.</span></span>|
|<span data-ttu-id="e7d07-115">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="e7d07-115">managementTemplateId</span></span>|<span data-ttu-id="e7d07-116">String</span><span class="sxs-lookup"><span data-stu-id="e7d07-116">String</span></span>|<span data-ttu-id="e7d07-117">用于生成管理操作的管理模板标识符。</span><span class="sxs-lookup"><span data-stu-id="e7d07-117">The management template identifier that was used to generate the management action.</span></span> <span data-ttu-id="e7d07-118">必填。</span><span class="sxs-lookup"><span data-stu-id="e7d07-118">Required.</span></span> <span data-ttu-id="e7d07-119">只读。</span><span class="sxs-lookup"><span data-stu-id="e7d07-119">Read-only.</span></span>|
|<span data-ttu-id="e7d07-120">状态</span><span class="sxs-lookup"><span data-stu-id="e7d07-120">status</span></span>|<span data-ttu-id="e7d07-121">managementActionStatus</span><span class="sxs-lookup"><span data-stu-id="e7d07-121">managementActionStatus</span></span>|<span data-ttu-id="e7d07-122">管理操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e7d07-122">The status of the management action.</span></span> <span data-ttu-id="e7d07-123">可取值为：`toAddress`、`completed`、`error`、`timeOut`、`inProgress`、`planned`、`resolvedBy3rdParty`、`resolvedThroughAlternateMitigation`、`riskAccepted`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e7d07-123">Possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`.</span></span> <span data-ttu-id="e7d07-124">必填。</span><span class="sxs-lookup"><span data-stu-id="e7d07-124">Required.</span></span>|
|<span data-ttu-id="e7d07-125">workloadActionDeploymentStatuses</span><span class="sxs-lookup"><span data-stu-id="e7d07-125">workloadActionDeploymentStatuses</span></span>|<span data-ttu-id="e7d07-126">[microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7d07-126">[microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md) collection</span></span>|<span data-ttu-id="e7d07-127">给定管理操作工作负荷操作部署方案的集合。</span><span class="sxs-lookup"><span data-stu-id="e7d07-127">The collection of workload action deployment statues for the given management action.</span></span> <span data-ttu-id="e7d07-128">可选。</span><span class="sxs-lookup"><span data-stu-id="e7d07-128">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7d07-129">关系</span><span class="sxs-lookup"><span data-stu-id="e7d07-129">Relationships</span></span>
<span data-ttu-id="e7d07-130">无。</span><span class="sxs-lookup"><span data-stu-id="e7d07-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7d07-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7d07-131">JSON representation</span></span>
<span data-ttu-id="e7d07-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7d07-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
