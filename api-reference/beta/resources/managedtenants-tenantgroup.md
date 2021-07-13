---
title: tenantGroup 资源类型
description: 表示托管租户的逻辑组。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2ab0d97afff68dca7d76b1ad6c4e461ad6af6233
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402272"
---
# <a name="tenantgroup-resource-type"></a><span data-ttu-id="9dd99-103">tenantGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="9dd99-103">tenantGroup resource type</span></span>

<span data-ttu-id="9dd99-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9dd99-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dd99-105">表示托管租户的逻辑组。</span><span class="sxs-lookup"><span data-stu-id="9dd99-105">Represents a logical group of managed tenants.</span></span>

## <a name="methods"></a><span data-ttu-id="9dd99-106">方法</span><span class="sxs-lookup"><span data-stu-id="9dd99-106">Methods</span></span>
|<span data-ttu-id="9dd99-107">方法</span><span class="sxs-lookup"><span data-stu-id="9dd99-107">Method</span></span>|<span data-ttu-id="9dd99-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9dd99-108">Return type</span></span>|<span data-ttu-id="9dd99-109">说明</span><span class="sxs-lookup"><span data-stu-id="9dd99-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9dd99-110">列出 tenantGroups</span><span class="sxs-lookup"><span data-stu-id="9dd99-110">List tenantGroups</span></span>](../api/managedtenants-managedtenant-list-tenantgroups.md)|<span data-ttu-id="9dd99-111">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd99-111">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection</span></span>|<span data-ttu-id="9dd99-112">获取 [tenantGroup 对象](../resources/managedtenants-tenantgroup.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="9dd99-112">Get a list of the [tenantGroup](../resources/managedtenants-tenantgroup.md) objects and their properties.</span></span>|
|[<span data-ttu-id="9dd99-113">获取 tenantGroup</span><span class="sxs-lookup"><span data-stu-id="9dd99-113">Get tenantGroup</span></span>](../api/managedtenants-tenantgroup-get.md)|[<span data-ttu-id="9dd99-114">microsoft.graph.managedTenants.tenantGroup</span><span class="sxs-lookup"><span data-stu-id="9dd99-114">microsoft.graph.managedTenants.tenantGroup</span></span>](../resources/managedtenants-tenantgroup.md)|<span data-ttu-id="9dd99-115">读取 [tenantGroup](../resources/managedtenants-tenantgroup.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9dd99-115">Read the properties and relationships of a [tenantGroup](../resources/managedtenants-tenantgroup.md) object.</span></span>|
|[<span data-ttu-id="9dd99-116">tenantSearch</span><span class="sxs-lookup"><span data-stu-id="9dd99-116">tenantSearch</span></span>](../api/managedtenants-tenantgroup-tenantsearch.md)|<span data-ttu-id="9dd99-117">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd99-117">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection</span></span>|<span data-ttu-id="9dd99-118">跨租户组搜索特定的托管租户。</span><span class="sxs-lookup"><span data-stu-id="9dd99-118">Searches for the specific managed tenant across tenant groups.</span></span>|

## <a name="properties"></a><span data-ttu-id="9dd99-119">属性</span><span class="sxs-lookup"><span data-stu-id="9dd99-119">Properties</span></span>
|<span data-ttu-id="9dd99-120">属性</span><span class="sxs-lookup"><span data-stu-id="9dd99-120">Property</span></span>|<span data-ttu-id="9dd99-121">类型</span><span class="sxs-lookup"><span data-stu-id="9dd99-121">Type</span></span>|<span data-ttu-id="9dd99-122">说明</span><span class="sxs-lookup"><span data-stu-id="9dd99-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd99-123">allTenantsIncluded</span><span class="sxs-lookup"><span data-stu-id="9dd99-123">allTenantsIncluded</span></span>|<span data-ttu-id="9dd99-124">布尔</span><span class="sxs-lookup"><span data-stu-id="9dd99-124">Boolean</span></span>|<span data-ttu-id="9dd99-125">一个标志，指示所有托管租户是否都包含在租户组中。</span><span class="sxs-lookup"><span data-stu-id="9dd99-125">A flag indicating whether all managed tenant are included in the tenant group.</span></span> <span data-ttu-id="9dd99-126">必填。</span><span class="sxs-lookup"><span data-stu-id="9dd99-126">Required.</span></span> <span data-ttu-id="9dd99-127">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd99-127">Read-only.</span></span>|
|<span data-ttu-id="9dd99-128">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd99-128">displayName</span></span>|<span data-ttu-id="9dd99-129">String</span><span class="sxs-lookup"><span data-stu-id="9dd99-129">String</span></span>|<span data-ttu-id="9dd99-130">租户显示名称的组。</span><span class="sxs-lookup"><span data-stu-id="9dd99-130">The display name for the tenant group.</span></span> <span data-ttu-id="9dd99-131">可选。</span><span class="sxs-lookup"><span data-stu-id="9dd99-131">Optional.</span></span> <span data-ttu-id="9dd99-132">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd99-132">Read-only.</span></span>|
|<span data-ttu-id="9dd99-133">id</span><span class="sxs-lookup"><span data-stu-id="9dd99-133">id</span></span>|<span data-ttu-id="9dd99-134">String</span><span class="sxs-lookup"><span data-stu-id="9dd99-134">String</span></span>|<span data-ttu-id="9dd99-135">租户组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9dd99-135">The unique identifier for the tenant group.</span></span> <span data-ttu-id="9dd99-136">必填。</span><span class="sxs-lookup"><span data-stu-id="9dd99-136">Required.</span></span> <span data-ttu-id="9dd99-137">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd99-137">Read-only.</span></span>|
|<span data-ttu-id="9dd99-138">managementActions</span><span class="sxs-lookup"><span data-stu-id="9dd99-138">managementActions</span></span>|<span data-ttu-id="9dd99-139">[microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd99-139">[microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md) collection</span></span>|<span data-ttu-id="9dd99-140">与租户组关联的管理操作的集合。</span><span class="sxs-lookup"><span data-stu-id="9dd99-140">The collection of management action associated with the tenant group.</span></span> <span data-ttu-id="9dd99-141">可选。</span><span class="sxs-lookup"><span data-stu-id="9dd99-141">Optional.</span></span> <span data-ttu-id="9dd99-142">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd99-142">Read-only.</span></span>|
|<span data-ttu-id="9dd99-143">managementIntents</span><span class="sxs-lookup"><span data-stu-id="9dd99-143">managementIntents</span></span>|<span data-ttu-id="9dd99-144">[microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd99-144">[microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md) collection</span></span>|<span data-ttu-id="9dd99-145">与租户组关联的管理意图的集合。</span><span class="sxs-lookup"><span data-stu-id="9dd99-145">The collection of management intents associated with the tenant group.</span></span> <span data-ttu-id="9dd99-146">可选。</span><span class="sxs-lookup"><span data-stu-id="9dd99-146">Optional.</span></span> <span data-ttu-id="9dd99-147">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd99-147">Read-only.</span></span>|
|<span data-ttu-id="9dd99-148">tenantIds</span><span class="sxs-lookup"><span data-stu-id="9dd99-148">tenantIds</span></span>|<span data-ttu-id="9dd99-149">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9dd99-149">String collection</span></span>|<span data-ttu-id="9dd99-150">托管租户标识符的集合包括在租户组中。</span><span class="sxs-lookup"><span data-stu-id="9dd99-150">The collection of managed tenant identifiers include in the tenant group.</span></span> <span data-ttu-id="9dd99-151">可选。</span><span class="sxs-lookup"><span data-stu-id="9dd99-151">Optional.</span></span> <span data-ttu-id="9dd99-152">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd99-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd99-153">关系</span><span class="sxs-lookup"><span data-stu-id="9dd99-153">Relationships</span></span>
<span data-ttu-id="9dd99-154">无。</span><span class="sxs-lookup"><span data-stu-id="9dd99-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dd99-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9dd99-155">JSON representation</span></span>
<span data-ttu-id="9dd99-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dd99-156">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "allTenantsIncluded": "Boolean",
  "tenantIds": [
    "String"
  ],
  "managementIntents": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
    }
  ],
  "managementActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
    }
  ]
}
```
