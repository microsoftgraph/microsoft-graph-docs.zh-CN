---
title: managementActionTenantDeploymentStatus 资源类型
description: 表示管理操作租户级别的部署状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 1967c3ad96cc9c4e76a718cafab7ba14207753a9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402284"
---
# <a name="managementactiontenantdeploymentstatus-resource-type"></a><span data-ttu-id="c742f-103">managementActionTenantDeploymentStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="c742f-103">managementActionTenantDeploymentStatus resource type</span></span>

<span data-ttu-id="c742f-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c742f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c742f-105">表示管理操作租户级别的部署状态。</span><span class="sxs-lookup"><span data-stu-id="c742f-105">Represents tenant level deployment status for the management action.</span></span>

## <a name="methods"></a><span data-ttu-id="c742f-106">方法</span><span class="sxs-lookup"><span data-stu-id="c742f-106">Methods</span></span>
|<span data-ttu-id="c742f-107">方法</span><span class="sxs-lookup"><span data-stu-id="c742f-107">Method</span></span>|<span data-ttu-id="c742f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c742f-108">Return type</span></span>|<span data-ttu-id="c742f-109">说明</span><span class="sxs-lookup"><span data-stu-id="c742f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c742f-110">List managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c742f-110">List managementActionTenantDeploymentStatus</span></span>](../api/managedtenants-managedtenant-list-managementactiontenantdeploymentstatuses.md)|<span data-ttu-id="c742f-111">[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c742f-111">[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) collection</span></span>|<span data-ttu-id="c742f-112">获取 [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c742f-112">Get a list of the [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c742f-113">获取 managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c742f-113">Get managementActionTenantDeploymentStatus</span></span>](../api/managedtenants-managementactiontenantdeploymentstatus-get.md)|[<span data-ttu-id="c742f-114">microsoft.graph.managedTenants.managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c742f-114">microsoft.graph.managedTenants.managementActionTenantDeploymentStatus</span></span>](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|<span data-ttu-id="c742f-115">读取 [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c742f-115">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>|
|[<span data-ttu-id="c742f-116">changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c742f-116">changeDeploymentStatus</span></span>](../api/managedtenants-managementactiontenantdeploymentstatus-changedeploymentstatus.md)|[<span data-ttu-id="c742f-117">microsoft.graph.managedTenants.managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c742f-117">microsoft.graph.managedTenants.managementActionDeploymentStatus</span></span>](../resources/managedtenants-managementactiondeploymentstatus.md)|<span data-ttu-id="c742f-118">更改管理操作部署状态。</span><span class="sxs-lookup"><span data-stu-id="c742f-118">Changes the deployment status for the management action.</span></span>|

## <a name="properties"></a><span data-ttu-id="c742f-119">属性</span><span class="sxs-lookup"><span data-stu-id="c742f-119">Properties</span></span>
|<span data-ttu-id="c742f-120">属性</span><span class="sxs-lookup"><span data-stu-id="c742f-120">Property</span></span>|<span data-ttu-id="c742f-121">类型</span><span class="sxs-lookup"><span data-stu-id="c742f-121">Type</span></span>|<span data-ttu-id="c742f-122">说明</span><span class="sxs-lookup"><span data-stu-id="c742f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c742f-123">id</span><span class="sxs-lookup"><span data-stu-id="c742f-123">id</span></span>|<span data-ttu-id="c742f-124">String</span><span class="sxs-lookup"><span data-stu-id="c742f-124">String</span></span>|<span data-ttu-id="c742f-125">租户级别部署状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c742f-125">The unique identifier for the tenant level deployment status.</span></span> <span data-ttu-id="c742f-126">必填。</span><span class="sxs-lookup"><span data-stu-id="c742f-126">Required.</span></span> <span data-ttu-id="c742f-127">只读。</span><span class="sxs-lookup"><span data-stu-id="c742f-127">Read-only.</span></span>|
|<span data-ttu-id="c742f-128">statuses</span><span class="sxs-lookup"><span data-stu-id="c742f-128">statuses</span></span>|<span data-ttu-id="c742f-129">[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c742f-129">[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) collection</span></span>|<span data-ttu-id="c742f-130">管理操作的每个实例的部署状态集合。</span><span class="sxs-lookup"><span data-stu-id="c742f-130">The collection of deployment status for each instance of a management action.</span></span> <span data-ttu-id="c742f-131">可选。</span><span class="sxs-lookup"><span data-stu-id="c742f-131">Optional.</span></span>|
|<span data-ttu-id="c742f-132">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="c742f-132">tenantGroupId</span></span>|<span data-ttu-id="c742f-133">String</span><span class="sxs-lookup"><span data-stu-id="c742f-133">String</span></span>|<span data-ttu-id="c742f-134">与管理操作关联的租户组的标识符。</span><span class="sxs-lookup"><span data-stu-id="c742f-134">The identifier for the tenant group that is associated with the management action.</span></span> <span data-ttu-id="c742f-135">必填。</span><span class="sxs-lookup"><span data-stu-id="c742f-135">Required.</span></span> <span data-ttu-id="c742f-136">只读。</span><span class="sxs-lookup"><span data-stu-id="c742f-136">Read-only.</span></span>|
|<span data-ttu-id="c742f-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="c742f-137">tenantId</span></span>|<span data-ttu-id="c742f-138">String</span><span class="sxs-lookup"><span data-stu-id="c742f-138">String</span></span>|<span data-ttu-id="c742f-139">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="c742f-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="c742f-140">必填。</span><span class="sxs-lookup"><span data-stu-id="c742f-140">Required.</span></span> <span data-ttu-id="c742f-141">只读。</span><span class="sxs-lookup"><span data-stu-id="c742f-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c742f-142">关系</span><span class="sxs-lookup"><span data-stu-id="c742f-142">Relationships</span></span>
<span data-ttu-id="c742f-143">无。</span><span class="sxs-lookup"><span data-stu-id="c742f-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c742f-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c742f-144">JSON representation</span></span>
<span data-ttu-id="c742f-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c742f-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "id": "String (identifier)",
  "tenantGroupId": "String",
  "tenantId": "String",
  "statuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
    }
  ]
}
```
