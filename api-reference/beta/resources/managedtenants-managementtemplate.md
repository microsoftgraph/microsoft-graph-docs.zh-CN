---
title: managementTemplate 资源类型
description: 表示一组可以针对托管租户执行的操作和设置。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2055db2d291dce3da0b4ad144c07b09bbb2fea6f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402277"
---
# <a name="managementtemplate-resource-type"></a><span data-ttu-id="0173a-103">managementTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0173a-103">managementTemplate resource type</span></span>

<span data-ttu-id="0173a-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0173a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0173a-105">表示一组可以针对托管租户执行的操作和设置。</span><span class="sxs-lookup"><span data-stu-id="0173a-105">Represents a group of actions and setting that can be performed against a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="0173a-106">方法</span><span class="sxs-lookup"><span data-stu-id="0173a-106">Methods</span></span>
|<span data-ttu-id="0173a-107">方法</span><span class="sxs-lookup"><span data-stu-id="0173a-107">Method</span></span>|<span data-ttu-id="0173a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0173a-108">Return type</span></span>|<span data-ttu-id="0173a-109">说明</span><span class="sxs-lookup"><span data-stu-id="0173a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0173a-110">List managementTemplates</span><span class="sxs-lookup"><span data-stu-id="0173a-110">List managementTemplates</span></span>](../api/managedtenants-managedtenant-list-managementtemplates.md)|<span data-ttu-id="0173a-111">[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0173a-111">[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection</span></span>|<span data-ttu-id="0173a-112">获取 [managementTemplate 对象](../resources/managedtenants-managementtemplate.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0173a-112">Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.</span></span>|
|[<span data-ttu-id="0173a-113">获取 managementTemplate</span><span class="sxs-lookup"><span data-stu-id="0173a-113">Get managementTemplate</span></span>](../api/managedtenants-managementtemplate-get.md)|[<span data-ttu-id="0173a-114">microsoft.graph.managedTenants.managementTemplate</span><span class="sxs-lookup"><span data-stu-id="0173a-114">microsoft.graph.managedTenants.managementTemplate</span></span>](../resources/managedtenants-managementtemplate.md)|<span data-ttu-id="0173a-115">读取 [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0173a-115">Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0173a-116">属性</span><span class="sxs-lookup"><span data-stu-id="0173a-116">Properties</span></span>
|<span data-ttu-id="0173a-117">属性</span><span class="sxs-lookup"><span data-stu-id="0173a-117">Property</span></span>|<span data-ttu-id="0173a-118">类型</span><span class="sxs-lookup"><span data-stu-id="0173a-118">Type</span></span>|<span data-ttu-id="0173a-119">说明</span><span class="sxs-lookup"><span data-stu-id="0173a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0173a-120">category</span><span class="sxs-lookup"><span data-stu-id="0173a-120">category</span></span>|<span data-ttu-id="0173a-121">managementCategory</span><span class="sxs-lookup"><span data-stu-id="0173a-121">managementCategory</span></span>|<span data-ttu-id="0173a-122">管理模板的管理类别。</span><span class="sxs-lookup"><span data-stu-id="0173a-122">The management category for the management template.</span></span> <span data-ttu-id="0173a-123">可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0173a-123">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="0173a-124">必填。</span><span class="sxs-lookup"><span data-stu-id="0173a-124">Required.</span></span> <span data-ttu-id="0173a-125">只读。</span><span class="sxs-lookup"><span data-stu-id="0173a-125">Read-only.</span></span>|
|<span data-ttu-id="0173a-126">说明</span><span class="sxs-lookup"><span data-stu-id="0173a-126">description</span></span>|<span data-ttu-id="0173a-127">String</span><span class="sxs-lookup"><span data-stu-id="0173a-127">String</span></span>|<span data-ttu-id="0173a-128">管理模板的说明。</span><span class="sxs-lookup"><span data-stu-id="0173a-128">The description for the management template.</span></span> <span data-ttu-id="0173a-129">可选。</span><span class="sxs-lookup"><span data-stu-id="0173a-129">Optional.</span></span> <span data-ttu-id="0173a-130">只读。</span><span class="sxs-lookup"><span data-stu-id="0173a-130">Read-only.</span></span>|
|<span data-ttu-id="0173a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0173a-131">displayName</span></span>|<span data-ttu-id="0173a-132">String</span><span class="sxs-lookup"><span data-stu-id="0173a-132">String</span></span>|<span data-ttu-id="0173a-133">管理显示名称的表单。</span><span class="sxs-lookup"><span data-stu-id="0173a-133">The display name for the management template.</span></span> <span data-ttu-id="0173a-134">必填。</span><span class="sxs-lookup"><span data-stu-id="0173a-134">Required.</span></span> <span data-ttu-id="0173a-135">只读。</span><span class="sxs-lookup"><span data-stu-id="0173a-135">Read-only.</span></span>|
|<span data-ttu-id="0173a-136">id</span><span class="sxs-lookup"><span data-stu-id="0173a-136">id</span></span>|<span data-ttu-id="0173a-137">String</span><span class="sxs-lookup"><span data-stu-id="0173a-137">String</span></span>|<span data-ttu-id="0173a-138">管理模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0173a-138">The unique identifier for the management template.</span></span> <span data-ttu-id="0173a-139">必填。</span><span class="sxs-lookup"><span data-stu-id="0173a-139">Required.</span></span> <span data-ttu-id="0173a-140">只读。</span><span class="sxs-lookup"><span data-stu-id="0173a-140">Read-only.</span></span>|
|<span data-ttu-id="0173a-141">parameters</span><span class="sxs-lookup"><span data-stu-id="0173a-141">parameters</span></span>|<span data-ttu-id="0173a-142">[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0173a-142">[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) collection</span></span>|<span data-ttu-id="0173a-143">管理模板使用的参数集合。</span><span class="sxs-lookup"><span data-stu-id="0173a-143">The collection of parameters used by the management template.</span></span> <span data-ttu-id="0173a-144">可选。</span><span class="sxs-lookup"><span data-stu-id="0173a-144">Optional.</span></span> <span data-ttu-id="0173a-145">只读。</span><span class="sxs-lookup"><span data-stu-id="0173a-145">Read-only.</span></span>|
|<span data-ttu-id="0173a-146">workloadActions</span><span class="sxs-lookup"><span data-stu-id="0173a-146">workloadActions</span></span>|<span data-ttu-id="0173a-147">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0173a-147">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection</span></span>|<span data-ttu-id="0173a-148">与管理模板关联的工作负荷操作的集合。</span><span class="sxs-lookup"><span data-stu-id="0173a-148">The collection of workload actions associated with the management template.</span></span> <span data-ttu-id="0173a-149">可选。</span><span class="sxs-lookup"><span data-stu-id="0173a-149">Optional.</span></span> <span data-ttu-id="0173a-150">只读。</span><span class="sxs-lookup"><span data-stu-id="0173a-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0173a-151">关系</span><span class="sxs-lookup"><span data-stu-id="0173a-151">Relationships</span></span>
<span data-ttu-id="0173a-152">无。</span><span class="sxs-lookup"><span data-stu-id="0173a-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0173a-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0173a-153">JSON representation</span></span>
<span data-ttu-id="0173a-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0173a-154">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
