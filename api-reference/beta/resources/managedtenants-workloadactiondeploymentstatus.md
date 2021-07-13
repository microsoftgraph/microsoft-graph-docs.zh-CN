---
title: workloadActionDeploymentStatus 资源类型
description: 表示工作负荷操作部署状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a8c14b821ceabf8c8196a25c141ad8730f7151d6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402089"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a><span data-ttu-id="bf2c0-103">workloadActionDeploymentStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf2c0-103">workloadActionDeploymentStatus resource type</span></span>

<span data-ttu-id="bf2c0-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="bf2c0-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf2c0-105">表示工作负荷操作部署状态。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-105">Represents the deployment status for the workload action.</span></span>

## <a name="properties"></a><span data-ttu-id="bf2c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="bf2c0-106">Properties</span></span>
|<span data-ttu-id="bf2c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf2c0-107">Property</span></span>|<span data-ttu-id="bf2c0-108">类型</span><span class="sxs-lookup"><span data-stu-id="bf2c0-108">Type</span></span>|<span data-ttu-id="bf2c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf2c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf2c0-110">actionId</span><span class="sxs-lookup"><span data-stu-id="bf2c0-110">actionId</span></span>|<span data-ttu-id="bf2c0-111">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-111">String</span></span>|<span data-ttu-id="bf2c0-112">工作负荷操作的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-112">The unique identifier for the workload action.</span></span> <span data-ttu-id="bf2c0-113">必填。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-113">Required.</span></span> <span data-ttu-id="bf2c0-114">只读。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-114">Read-only.</span></span>|
|<span data-ttu-id="bf2c0-115">deployedPolicyId</span><span class="sxs-lookup"><span data-stu-id="bf2c0-115">deployedPolicyId</span></span>|<span data-ttu-id="bf2c0-116">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-116">String</span></span>|<span data-ttu-id="bf2c0-117">通过应用工作负荷操作创建的任何策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-117">The identifier of any policy that was created by applying the workload action.</span></span> <span data-ttu-id="bf2c0-118">可选。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-118">Optional.</span></span> <span data-ttu-id="bf2c0-119">只读。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-119">Read-only.</span></span>|
|<span data-ttu-id="bf2c0-120">error</span><span class="sxs-lookup"><span data-stu-id="bf2c0-120">error</span></span>|[<span data-ttu-id="bf2c0-121">microsoft.graph.genericError</span><span class="sxs-lookup"><span data-stu-id="bf2c0-121">microsoft.graph.genericError</span></span>](../resources/genericerror.md)|<span data-ttu-id="bf2c0-122">部署工作负荷操作时发生的异常的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-122">The detailed information for exceptions that occur when deploying the workload action.</span></span> <span data-ttu-id="bf2c0-123">可选。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-123">Optional.</span></span> <span data-ttu-id="bf2c0-124">必填。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-124">Required.</span></span>|
|<span data-ttu-id="bf2c0-125">lastDeploymentDateTime</span><span class="sxs-lookup"><span data-stu-id="bf2c0-125">lastDeploymentDateTime</span></span>|<span data-ttu-id="bf2c0-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf2c0-126">DateTimeOffset</span></span>|<span data-ttu-id="bf2c0-127">上次部署工作负荷操作日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-127">The date and time the workload action was last deployed.</span></span> <span data-ttu-id="bf2c0-128">可选。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-128">Optional.</span></span>|
|<span data-ttu-id="bf2c0-129">状态</span><span class="sxs-lookup"><span data-stu-id="bf2c0-129">status</span></span>|<span data-ttu-id="bf2c0-130">workloadActionStatus</span><span class="sxs-lookup"><span data-stu-id="bf2c0-130">workloadActionStatus</span></span>|<span data-ttu-id="bf2c0-131">工作负荷操作部署的状态。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-131">The status of the workload action deployment.</span></span> <span data-ttu-id="bf2c0-132">可取值为：`toAddress`、`completed`、`error`、`timeOut`、`inProgress`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-132">Possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`.</span></span> <span data-ttu-id="bf2c0-133">必填。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-133">Required.</span></span> <span data-ttu-id="bf2c0-134">只读。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf2c0-135">关系</span><span class="sxs-lookup"><span data-stu-id="bf2c0-135">Relationships</span></span>
<span data-ttu-id="bf2c0-136">无。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf2c0-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf2c0-137">JSON representation</span></span>
<span data-ttu-id="bf2c0-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf2c0-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)"
}
```
