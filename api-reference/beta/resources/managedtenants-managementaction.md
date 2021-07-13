---
title: managementAction 资源类型
description: 表示给定托管租户的基线管理操作。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 156d4ff0d7ffb9574793ccdd5d56bc2a89cd3b22
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402400"
---
# <a name="managementaction-resource-type"></a><span data-ttu-id="aabf4-103">managementAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="aabf4-103">managementAction resource type</span></span>

<span data-ttu-id="aabf4-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="aabf4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aabf4-105">表示给定托管租户的基线管理操作。</span><span class="sxs-lookup"><span data-stu-id="aabf4-105">Represents a baseline management action for a given managed tenant.</span></span> <span data-ttu-id="aabf4-106">管理操作的示例包括设备加密、执行配置Azure Active Directory注册设备，以及要求管理员进行多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="aabf4-106">Examples of management actions are device encryption, perform configurations to allow Azure Active Directory device enrollment, and require multi-factor authentication for admins.</span></span>

## <a name="methods"></a><span data-ttu-id="aabf4-107">方法</span><span class="sxs-lookup"><span data-stu-id="aabf4-107">Methods</span></span>
|<span data-ttu-id="aabf4-108">方法</span><span class="sxs-lookup"><span data-stu-id="aabf4-108">Method</span></span>|<span data-ttu-id="aabf4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aabf4-109">Return type</span></span>|<span data-ttu-id="aabf4-110">说明</span><span class="sxs-lookup"><span data-stu-id="aabf4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aabf4-111">列出 managementActions</span><span class="sxs-lookup"><span data-stu-id="aabf4-111">List managementActions</span></span>](../api/managedtenants-managedtenant-list-managementactions.md)|<span data-ttu-id="aabf4-112">[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aabf4-112">[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) collection</span></span>|<span data-ttu-id="aabf4-113">获取 [managementAction 对象](../resources/managedtenants-managementaction.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="aabf4-113">Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.</span></span>|
|[<span data-ttu-id="aabf4-114">获取 managementAction</span><span class="sxs-lookup"><span data-stu-id="aabf4-114">Get managementAction</span></span>](../api/managedtenants-managementaction-get.md)|[<span data-ttu-id="aabf4-115">microsoft.graph.managedTenants.managementAction</span><span class="sxs-lookup"><span data-stu-id="aabf4-115">microsoft.graph.managedTenants.managementAction</span></span>](../resources/managedtenants-managementaction.md)|<span data-ttu-id="aabf4-116">读取 [managementAction](../resources/managedtenants-managementaction.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aabf4-116">Read the properties and relationships of a [managementAction](../resources/managedtenants-managementaction.md) object.</span></span>|
|[<span data-ttu-id="aabf4-117">apply</span><span class="sxs-lookup"><span data-stu-id="aabf4-117">apply</span></span>](../api/managedtenants-managementaction-apply.md)|[<span data-ttu-id="aabf4-118">microsoft.graph.managedTenants.managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="aabf4-118">microsoft.graph.managedTenants.managementActionDeploymentStatus</span></span>](../resources/managedtenants-managementactiondeploymentstatus.md)|<span data-ttu-id="aabf4-119">对托管租户应用管理操作。</span><span class="sxs-lookup"><span data-stu-id="aabf4-119">Applies the management actions against the managed tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="aabf4-120">属性</span><span class="sxs-lookup"><span data-stu-id="aabf4-120">Properties</span></span>
|<span data-ttu-id="aabf4-121">属性</span><span class="sxs-lookup"><span data-stu-id="aabf4-121">Property</span></span>|<span data-ttu-id="aabf4-122">类型</span><span class="sxs-lookup"><span data-stu-id="aabf4-122">Type</span></span>|<span data-ttu-id="aabf4-123">说明</span><span class="sxs-lookup"><span data-stu-id="aabf4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aabf4-124">category</span><span class="sxs-lookup"><span data-stu-id="aabf4-124">category</span></span>|<span data-ttu-id="aabf4-125">managementCategory</span><span class="sxs-lookup"><span data-stu-id="aabf4-125">managementCategory</span></span>|<span data-ttu-id="aabf4-126">管理操作类别。</span><span class="sxs-lookup"><span data-stu-id="aabf4-126">The category for the management action.</span></span> <span data-ttu-id="aabf4-127">可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="aabf4-127">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="aabf4-128">可选。</span><span class="sxs-lookup"><span data-stu-id="aabf4-128">Optional.</span></span> <span data-ttu-id="aabf4-129">只读。</span><span class="sxs-lookup"><span data-stu-id="aabf4-129">Read-only.</span></span>|
|<span data-ttu-id="aabf4-130">说明</span><span class="sxs-lookup"><span data-stu-id="aabf4-130">description</span></span>|<span data-ttu-id="aabf4-131">String</span><span class="sxs-lookup"><span data-stu-id="aabf4-131">String</span></span>|<span data-ttu-id="aabf4-132">管理操作的说明。</span><span class="sxs-lookup"><span data-stu-id="aabf4-132">The description for the management action.</span></span> <span data-ttu-id="aabf4-133">可选。</span><span class="sxs-lookup"><span data-stu-id="aabf4-133">Optional.</span></span> <span data-ttu-id="aabf4-134">只读。</span><span class="sxs-lookup"><span data-stu-id="aabf4-134">Read-only.</span></span>|
|<span data-ttu-id="aabf4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aabf4-135">displayName</span></span>|<span data-ttu-id="aabf4-136">String</span><span class="sxs-lookup"><span data-stu-id="aabf4-136">String</span></span>|<span data-ttu-id="aabf4-137">管理显示名称的项。</span><span class="sxs-lookup"><span data-stu-id="aabf4-137">The display name for the management action.</span></span> <span data-ttu-id="aabf4-138">可选。</span><span class="sxs-lookup"><span data-stu-id="aabf4-138">Optional.</span></span> <span data-ttu-id="aabf4-139">只读。</span><span class="sxs-lookup"><span data-stu-id="aabf4-139">Read-only.</span></span>|
|<span data-ttu-id="aabf4-140">id</span><span class="sxs-lookup"><span data-stu-id="aabf4-140">id</span></span>|<span data-ttu-id="aabf4-141">String</span><span class="sxs-lookup"><span data-stu-id="aabf4-141">String</span></span>|<span data-ttu-id="aabf4-142">管理操作的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aabf4-142">The unique identifier for the management action.</span></span> <span data-ttu-id="aabf4-143">必填。</span><span class="sxs-lookup"><span data-stu-id="aabf4-143">Required.</span></span> <span data-ttu-id="aabf4-144">只读。</span><span class="sxs-lookup"><span data-stu-id="aabf4-144">Read-only.</span></span>|
|<span data-ttu-id="aabf4-145">referenceTemplateId</span><span class="sxs-lookup"><span data-stu-id="aabf4-145">referenceTemplateId</span></span>|<span data-ttu-id="aabf4-146">String</span><span class="sxs-lookup"><span data-stu-id="aabf4-146">String</span></span>|<span data-ttu-id="aabf4-147">用于生成管理操作的管理模板的引用。</span><span class="sxs-lookup"><span data-stu-id="aabf4-147">The reference for the management template used to generate the management action.</span></span> <span data-ttu-id="aabf4-148">必填。</span><span class="sxs-lookup"><span data-stu-id="aabf4-148">Required.</span></span> <span data-ttu-id="aabf4-149">只读。</span><span class="sxs-lookup"><span data-stu-id="aabf4-149">Read-only.</span></span>|
|<span data-ttu-id="aabf4-150">workloadActions</span><span class="sxs-lookup"><span data-stu-id="aabf4-150">workloadActions</span></span>|<span data-ttu-id="aabf4-151">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aabf4-151">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection</span></span>|<span data-ttu-id="aabf4-152">与管理操作关联的工作负荷操作的集合。</span><span class="sxs-lookup"><span data-stu-id="aabf4-152">The collection of workload actions associated with the management action.</span></span> <span data-ttu-id="aabf4-153">必填。</span><span class="sxs-lookup"><span data-stu-id="aabf4-153">Required.</span></span> <span data-ttu-id="aabf4-154">只读。</span><span class="sxs-lookup"><span data-stu-id="aabf4-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aabf4-155">关系</span><span class="sxs-lookup"><span data-stu-id="aabf4-155">Relationships</span></span>
<span data-ttu-id="aabf4-156">无。</span><span class="sxs-lookup"><span data-stu-id="aabf4-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aabf4-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aabf4-157">JSON representation</span></span>
<span data-ttu-id="aabf4-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aabf4-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
