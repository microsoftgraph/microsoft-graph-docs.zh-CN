---
title: cloudPcProvisioningPolicyAssignment 资源类型
description: CloudPC 设置策略分配
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbbdf76dfb184efdae7279b5d4970367995c0a6c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378303"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="ad4a2-103">cloudPcProvisioningPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad4a2-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="ad4a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad4a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad4a2-105">表示设置策略分配的已定义集合。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-105">Represents a defined collection of provisioning policy assignments.</span></span>


## <a name="properties"></a><span data-ttu-id="ad4a2-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad4a2-106">Properties</span></span>

|<span data-ttu-id="ad4a2-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad4a2-107">Property</span></span>|<span data-ttu-id="ad4a2-108">类型</span><span class="sxs-lookup"><span data-stu-id="ad4a2-108">Type</span></span>|<span data-ttu-id="ad4a2-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad4a2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad4a2-110">id</span><span class="sxs-lookup"><span data-stu-id="ad4a2-110">id</span></span>|<span data-ttu-id="ad4a2-111">字符串</span><span class="sxs-lookup"><span data-stu-id="ad4a2-111">String</span></span>|<span data-ttu-id="ad4a2-112">设置策略分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="ad4a2-113">只读。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-113">Read-only.</span></span> <span data-ttu-id="ad4a2-114">如果 `target` 是用户组，则 ID 显示为 {policyId} _ {groupId}。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-114">If `target` is a user group, then the ID is shown as {policyId}_{groupId}.</span></span>|
|<span data-ttu-id="ad4a2-115">target</span><span class="sxs-lookup"><span data-stu-id="ad4a2-115">target</span></span>|[<span data-ttu-id="ad4a2-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ad4a2-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="ad4a2-117">预配策略的分配目标。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="ad4a2-118">目前，此策略支持的唯一目标是用户组。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-118">Currently, the only target supported for this policy is a user group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad4a2-119">关系</span><span class="sxs-lookup"><span data-stu-id="ad4a2-119">Relationships</span></span>

<span data-ttu-id="ad4a2-120">无。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad4a2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad4a2-121">JSON representation</span></span>

<span data-ttu-id="ad4a2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad4a2-122">The following is a JSON representation of the resource.</span></span>
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
