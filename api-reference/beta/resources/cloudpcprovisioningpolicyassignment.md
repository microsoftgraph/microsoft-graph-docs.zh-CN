---
title: cloudPcProvisioningPolicyAssignment 资源类型
description: CloudPC 预配策略分配
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a96c3717b97b3f721c77b1150841f1eb51ded89f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082235"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="2ba2a-103">cloudPcProvisioningPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ba2a-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="2ba2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba2a-105">表示已定义的设置策略分配集合。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-105">Represents a defined collection of provisioning policy assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="2ba2a-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ba2a-106">Properties</span></span>

|<span data-ttu-id="2ba2a-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ba2a-107">Property</span></span>|<span data-ttu-id="2ba2a-108">类型</span><span class="sxs-lookup"><span data-stu-id="2ba2a-108">Type</span></span>|<span data-ttu-id="2ba2a-109">说明</span><span class="sxs-lookup"><span data-stu-id="2ba2a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba2a-110">id</span><span class="sxs-lookup"><span data-stu-id="2ba2a-110">id</span></span>|<span data-ttu-id="2ba2a-111">String</span><span class="sxs-lookup"><span data-stu-id="2ba2a-111">String</span></span>|<span data-ttu-id="2ba2a-112">预配策略分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="2ba2a-113">只读。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-113">Read-only.</span></span> <span data-ttu-id="2ba2a-114">如果 `target` 为用户组，则 ID 显示为 {policyId} \_ {groupId}。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-114">If `target` is a user group, then the ID is shown as {policyId}\_{groupId}.</span></span>|
|<span data-ttu-id="2ba2a-115">target</span><span class="sxs-lookup"><span data-stu-id="2ba2a-115">target</span></span>|[<span data-ttu-id="2ba2a-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2ba2a-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="2ba2a-117">预配策略的分配目标。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="2ba2a-118">目前，此策略支持的唯一目标为用户组。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-118">Currently, the only target supported for this policy is a user group.</span></span> <span data-ttu-id="2ba2a-119">有关详细信息，请参阅 [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-119">For details, see [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2ba2a-120">关系</span><span class="sxs-lookup"><span data-stu-id="2ba2a-120">Relationships</span></span>

<span data-ttu-id="2ba2a-121">无。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ba2a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ba2a-122">JSON representation</span></span>

<span data-ttu-id="2ba2a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-123">The following is a JSON representation of the resource.</span></span>
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
