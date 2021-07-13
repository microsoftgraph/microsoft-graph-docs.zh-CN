---
title: tenantDetailedInformation 资源类型
description: 表示托管租户的详细信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 40aa157b12ccef64b6eb7ab6c92349a3e74745f8
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402273"
---
# <a name="tenantdetailedinformation-resource-type"></a><span data-ttu-id="c8fb6-103">tenantDetailedInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8fb6-103">tenantDetailedInformation resource type</span></span>

<span data-ttu-id="c8fb6-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c8fb6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8fb6-105">表示托管租户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-105">Represents detailed information for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="c8fb6-106">方法</span><span class="sxs-lookup"><span data-stu-id="c8fb6-106">Methods</span></span>
|<span data-ttu-id="c8fb6-107">方法</span><span class="sxs-lookup"><span data-stu-id="c8fb6-107">Method</span></span>|<span data-ttu-id="c8fb6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8fb6-108">Return type</span></span>|<span data-ttu-id="c8fb6-109">说明</span><span class="sxs-lookup"><span data-stu-id="c8fb6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8fb6-110">列出 tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="c8fb6-110">List tenantDetailedInformation</span></span>](../api/managedtenants-managedtenant-list-tenantsdetailedinformation.md)|<span data-ttu-id="c8fb6-111">[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8fb6-111">[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) collection</span></span>|<span data-ttu-id="c8fb6-112">获取 [tenantDetailedInformation 对象](../resources/managedtenants-tenantdetailedinformation.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-112">Get a list of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c8fb6-113">获取 tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="c8fb6-113">Get tenantDetailedInformation</span></span>](../api/managedtenants-tenantdetailedinformation-get.md)|[<span data-ttu-id="c8fb6-114">microsoft.graph.managedTenants.tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="c8fb6-114">microsoft.graph.managedTenants.tenantDetailedInformation</span></span>](../resources/managedtenants-tenantdetailedinformation.md)|<span data-ttu-id="c8fb6-115">读取 [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-115">Read the properties and relationships of a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8fb6-116">属性</span><span class="sxs-lookup"><span data-stu-id="c8fb6-116">Properties</span></span>
|<span data-ttu-id="c8fb6-117">属性</span><span class="sxs-lookup"><span data-stu-id="c8fb6-117">Property</span></span>|<span data-ttu-id="c8fb6-118">类型</span><span class="sxs-lookup"><span data-stu-id="c8fb6-118">Type</span></span>|<span data-ttu-id="c8fb6-119">说明</span><span class="sxs-lookup"><span data-stu-id="c8fb6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8fb6-120">城市</span><span class="sxs-lookup"><span data-stu-id="c8fb6-120">city</span></span>|<span data-ttu-id="c8fb6-121">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-121">String</span></span>|<span data-ttu-id="c8fb6-122">托管租户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-122">The city where the managed tenant is located.</span></span> <span data-ttu-id="c8fb6-123">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-123">Optional.</span></span> <span data-ttu-id="c8fb6-124">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-124">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-125">countryCode</span><span class="sxs-lookup"><span data-stu-id="c8fb6-125">countryCode</span></span>|<span data-ttu-id="c8fb6-126">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-126">String</span></span>|<span data-ttu-id="c8fb6-127">托管租户所在的国家/地区的代码。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-127">The code for the country where the managed tenant is located.</span></span> <span data-ttu-id="c8fb6-128">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-128">Optional.</span></span> <span data-ttu-id="c8fb6-129">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-129">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-130">countryName</span><span class="sxs-lookup"><span data-stu-id="c8fb6-130">countryName</span></span>|<span data-ttu-id="c8fb6-131">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-131">String</span></span>|<span data-ttu-id="c8fb6-132">托管租户所在的国家/地区的名称。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-132">The name for the country where the managed tenant is located.</span></span> <span data-ttu-id="c8fb6-133">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-133">Optional.</span></span> <span data-ttu-id="c8fb6-134">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-134">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="c8fb6-135">defaultDomainName</span></span>|<span data-ttu-id="c8fb6-136">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-136">String</span></span>|<span data-ttu-id="c8fb6-137">托管租户的默认域名。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-137">The default domain name for the managed tenant.</span></span> <span data-ttu-id="c8fb6-138">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-138">Optional.</span></span> <span data-ttu-id="c8fb6-139">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-139">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="c8fb6-140">displayName</span></span>|<span data-ttu-id="c8fb6-141">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-141">String</span></span>|<span data-ttu-id="c8fb6-142">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-142">The display name for the managed tenant.</span></span>|
|<span data-ttu-id="c8fb6-143">id</span><span class="sxs-lookup"><span data-stu-id="c8fb6-143">id</span></span>|<span data-ttu-id="c8fb6-144">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-144">String</span></span>|<span data-ttu-id="c8fb6-145">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-145">The unique identifier for this entity.</span></span> <span data-ttu-id="c8fb6-146">必填。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-146">Required.</span></span> <span data-ttu-id="c8fb6-147">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-147">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-148">industryName</span><span class="sxs-lookup"><span data-stu-id="c8fb6-148">industryName</span></span>|<span data-ttu-id="c8fb6-149">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-149">String</span></span>|<span data-ttu-id="c8fb6-150">与托管租户关联的业务行业。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-150">The business industry associated with the managed tenant.</span></span> <span data-ttu-id="c8fb6-151">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-151">Optional.</span></span> <span data-ttu-id="c8fb6-152">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-152">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-153">region</span><span class="sxs-lookup"><span data-stu-id="c8fb6-153">region</span></span>|<span data-ttu-id="c8fb6-154">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-154">String</span></span>|<span data-ttu-id="c8fb6-155">托管租户所在的区域。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-155">The region where the managed tenant is located.</span></span> <span data-ttu-id="c8fb6-156">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-156">Optional.</span></span> <span data-ttu-id="c8fb6-157">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-157">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-158">segmentName</span><span class="sxs-lookup"><span data-stu-id="c8fb6-158">segmentName</span></span>|<span data-ttu-id="c8fb6-159">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-159">String</span></span>|<span data-ttu-id="c8fb6-160">与托管租户关联的业务部门。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-160">The business segment associated with the managed tenant.</span></span> <span data-ttu-id="c8fb6-161">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-161">Optional.</span></span> <span data-ttu-id="c8fb6-162">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-162">Read-only.</span></span>|
|<span data-ttu-id="c8fb6-163">tenantId</span><span class="sxs-lookup"><span data-stu-id="c8fb6-163">tenantId</span></span>|<span data-ttu-id="c8fb6-164">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-164">String</span></span>|<span data-ttu-id="c8fb6-165">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-165">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="c8fb6-166">verticalName</span><span class="sxs-lookup"><span data-stu-id="c8fb6-166">verticalName</span></span>|<span data-ttu-id="c8fb6-167">String</span><span class="sxs-lookup"><span data-stu-id="c8fb6-167">String</span></span>|<span data-ttu-id="c8fb6-168">与托管租户关联的垂直。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-168">The vertical associated with the managed tenant.</span></span> <span data-ttu-id="c8fb6-169">可选。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-169">Optional.</span></span> <span data-ttu-id="c8fb6-170">只读。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-170">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8fb6-171">关系</span><span class="sxs-lookup"><span data-stu-id="c8fb6-171">Relationships</span></span>
<span data-ttu-id="c8fb6-172">无。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8fb6-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8fb6-173">JSON representation</span></span>
<span data-ttu-id="c8fb6-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8fb6-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String"
}
```

