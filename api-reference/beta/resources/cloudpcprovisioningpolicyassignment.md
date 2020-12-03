---
title: cloudPcProvisioningPolicyAssignment 资源类型
description: CloudPC 设置策略分配
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 06a90efc67b483fed569a4e7029a74dac4f7f9ee
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563700"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="59e3d-103">cloudPcProvisioningPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="59e3d-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="59e3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59e3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e3d-105">表示设置策略分配的已定义集合。</span><span class="sxs-lookup"><span data-stu-id="59e3d-105">Represents a defined collection of provisioning policy assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="59e3d-106">属性</span><span class="sxs-lookup"><span data-stu-id="59e3d-106">Properties</span></span>

|<span data-ttu-id="59e3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="59e3d-107">Property</span></span>|<span data-ttu-id="59e3d-108">类型</span><span class="sxs-lookup"><span data-stu-id="59e3d-108">Type</span></span>|<span data-ttu-id="59e3d-109">说明</span><span class="sxs-lookup"><span data-stu-id="59e3d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59e3d-110">id</span><span class="sxs-lookup"><span data-stu-id="59e3d-110">id</span></span>|<span data-ttu-id="59e3d-111">String</span><span class="sxs-lookup"><span data-stu-id="59e3d-111">String</span></span>|<span data-ttu-id="59e3d-112">设置策略分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="59e3d-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="59e3d-113">只读。</span><span class="sxs-lookup"><span data-stu-id="59e3d-113">Read-only.</span></span> <span data-ttu-id="59e3d-114">如果 `target` 是用户组，则 ID 显示为 {policyId} _ {groupId}。</span><span class="sxs-lookup"><span data-stu-id="59e3d-114">If `target` is a user group, then the ID is shown as {policyId}_{groupId}.</span></span>|
|<span data-ttu-id="59e3d-115">target</span><span class="sxs-lookup"><span data-stu-id="59e3d-115">target</span></span>|[<span data-ttu-id="59e3d-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="59e3d-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="59e3d-117">预配策略的分配目标。</span><span class="sxs-lookup"><span data-stu-id="59e3d-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="59e3d-118">目前，此策略支持的唯一目标是用户组。</span><span class="sxs-lookup"><span data-stu-id="59e3d-118">Currently, the only target supported for this policy is a user group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59e3d-119">关系</span><span class="sxs-lookup"><span data-stu-id="59e3d-119">Relationships</span></span>

<span data-ttu-id="59e3d-120">无。</span><span class="sxs-lookup"><span data-stu-id="59e3d-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59e3d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59e3d-121">JSON representation</span></span>

<span data-ttu-id="59e3d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59e3d-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
