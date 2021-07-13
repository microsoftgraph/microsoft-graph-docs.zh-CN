---
title: tenantCustomizedInformation 资源类型
description: 表示托管租户的可自定义信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 580479e6fd710eef7a0907ea51cd5605ef445e40
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402393"
---
# <a name="tenantcustomizedinformation-resource-type"></a><span data-ttu-id="6ccfb-103">tenantCustomizedInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ccfb-103">tenantCustomizedInformation resource type</span></span>

<span data-ttu-id="6ccfb-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6ccfb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ccfb-105">表示托管租户的可自定义信息。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-105">Represents customizable information for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="6ccfb-106">方法</span><span class="sxs-lookup"><span data-stu-id="6ccfb-106">Methods</span></span>
|<span data-ttu-id="6ccfb-107">方法</span><span class="sxs-lookup"><span data-stu-id="6ccfb-107">Method</span></span>|<span data-ttu-id="6ccfb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6ccfb-108">Return type</span></span>|<span data-ttu-id="6ccfb-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ccfb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ccfb-110">列出 tenantCustomizedInformations</span><span class="sxs-lookup"><span data-stu-id="6ccfb-110">List tenantCustomizedInformations</span></span>](../api/managedtenants-managedtenant-list-tenantscustomizedinformation.md)|<span data-ttu-id="6ccfb-111">[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ccfb-111">[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection</span></span>|<span data-ttu-id="6ccfb-112">获取 [tenantCustomizedInformation 对象](../resources/managedtenants-tenantcustomizedinformation.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-112">Get a list of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) objects and their properties.</span></span>|
|[<span data-ttu-id="6ccfb-113">获取 tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="6ccfb-113">Get tenantCustomizedInformation</span></span>](../api/managedtenants-tenantcustomizedinformation-get.md)|[<span data-ttu-id="6ccfb-114">microsoft.graph.managedTenants.tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="6ccfb-114">microsoft.graph.managedTenants.tenantCustomizedInformation</span></span>](../resources/managedtenants-tenantcustomizedinformation.md)|<span data-ttu-id="6ccfb-115">读取 [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-115">Read the properties and relationships of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>|
|[<span data-ttu-id="6ccfb-116">更新 tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="6ccfb-116">Update tenantCustomizedInformation</span></span>](../api/managedtenants-tenantcustomizedinformation-update.md)|[<span data-ttu-id="6ccfb-117">microsoft.graph.managedTenants.tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="6ccfb-117">microsoft.graph.managedTenants.tenantCustomizedInformation</span></span>](../resources/managedtenants-tenantcustomizedinformation.md)|<span data-ttu-id="6ccfb-118">更新 [tenantCustomizedInformation 对象](../resources/managedtenants-tenantcustomizedinformation.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-118">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ccfb-119">属性</span><span class="sxs-lookup"><span data-stu-id="6ccfb-119">Properties</span></span>
|<span data-ttu-id="6ccfb-120">属性</span><span class="sxs-lookup"><span data-stu-id="6ccfb-120">Property</span></span>|<span data-ttu-id="6ccfb-121">类型</span><span class="sxs-lookup"><span data-stu-id="6ccfb-121">Type</span></span>|<span data-ttu-id="6ccfb-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ccfb-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ccfb-123">contacts</span><span class="sxs-lookup"><span data-stu-id="6ccfb-123">contacts</span></span>|<span data-ttu-id="6ccfb-124">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ccfb-124">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="6ccfb-125">托管租户的联系人集合。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-125">The collection of contacts for the managed tenant.</span></span> <span data-ttu-id="6ccfb-126">可选。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-126">Optional.</span></span>|
|<span data-ttu-id="6ccfb-127">displayName</span><span class="sxs-lookup"><span data-stu-id="6ccfb-127">displayName</span></span>|<span data-ttu-id="6ccfb-128">String</span><span class="sxs-lookup"><span data-stu-id="6ccfb-128">String</span></span>|<span data-ttu-id="6ccfb-129">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-129">The display name for the managed tenant.</span></span> <span data-ttu-id="6ccfb-130">必填。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-130">Required.</span></span> <span data-ttu-id="6ccfb-131">只读。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-131">Read-only.</span></span>|
|<span data-ttu-id="6ccfb-132">id</span><span class="sxs-lookup"><span data-stu-id="6ccfb-132">id</span></span>|<span data-ttu-id="6ccfb-133">String</span><span class="sxs-lookup"><span data-stu-id="6ccfb-133">String</span></span>|<span data-ttu-id="6ccfb-134">托管Azure Active Directory租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-134">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="6ccfb-135">必填。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-135">Required.</span></span> <span data-ttu-id="6ccfb-136">只读。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-136">Read-only.</span></span>|
|<span data-ttu-id="6ccfb-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="6ccfb-137">tenantId</span></span>|<span data-ttu-id="6ccfb-138">String</span><span class="sxs-lookup"><span data-stu-id="6ccfb-138">String</span></span>|<span data-ttu-id="6ccfb-139">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="6ccfb-140">可选。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-140">Optional.</span></span> <span data-ttu-id="6ccfb-141">只读。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-141">Read-only.</span></span>|
|<span data-ttu-id="6ccfb-142">website</span><span class="sxs-lookup"><span data-stu-id="6ccfb-142">website</span></span>|<span data-ttu-id="6ccfb-143">String</span><span class="sxs-lookup"><span data-stu-id="6ccfb-143">String</span></span>|<span data-ttu-id="6ccfb-144">托管租户的网站。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-144">The website for the managed tenant.</span></span> <span data-ttu-id="6ccfb-145">必填。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-145">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ccfb-146">关系</span><span class="sxs-lookup"><span data-stu-id="6ccfb-146">Relationships</span></span>
<span data-ttu-id="6ccfb-147">无。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ccfb-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ccfb-148">JSON representation</span></span>
<span data-ttu-id="6ccfb-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ccfb-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```
