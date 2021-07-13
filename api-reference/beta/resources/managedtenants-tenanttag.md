---
title: tenantTag 资源类型
description: 表示可分配给托管租户的标记。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e48ad25e2af3ac491c6affe4bbb4712ab45e42fc
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402245"
---
# <a name="tenanttag-resource-type"></a><span data-ttu-id="9ee04-103">tenantTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ee04-103">tenantTag resource type</span></span>

<span data-ttu-id="9ee04-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9ee04-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ee04-105">表示可分配给托管租户的标记。</span><span class="sxs-lookup"><span data-stu-id="9ee04-105">Represents a tag that can be assigned to managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="9ee04-106">方法</span><span class="sxs-lookup"><span data-stu-id="9ee04-106">Methods</span></span>
|<span data-ttu-id="9ee04-107">方法</span><span class="sxs-lookup"><span data-stu-id="9ee04-107">Method</span></span>|<span data-ttu-id="9ee04-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ee04-108">Return type</span></span>|<span data-ttu-id="9ee04-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ee04-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ee04-110">列出 tenantTags</span><span class="sxs-lookup"><span data-stu-id="9ee04-110">List tenantTags</span></span>](../api/managedtenants-managedtenant-list-tenanttags.md)|<span data-ttu-id="9ee04-111">[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ee04-111">[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md) collection</span></span>|<span data-ttu-id="9ee04-112">获取 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="9ee04-112">Get a list of the [tenantTag](../resources/managedtenants-tenanttag.md) objects and their properties.</span></span>|
|[<span data-ttu-id="9ee04-113">创建 tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-113">Create tenantTag</span></span>](../api/managedtenants-managedtenant-post-tenanttags.md)|[<span data-ttu-id="9ee04-114">microsoft.graph.managedTenants.tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-114">microsoft.graph.managedTenants.tenantTag</span></span>](../resources/managedtenants-tenanttag.md)|<span data-ttu-id="9ee04-115">创建新的 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ee04-115">Create a new [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>|
|[<span data-ttu-id="9ee04-116">获取 tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-116">Get tenantTag</span></span>](../api/managedtenants-tenanttag-get.md)|[<span data-ttu-id="9ee04-117">microsoft.graph.managedTenants.tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-117">microsoft.graph.managedTenants.tenantTag</span></span>](../resources/managedtenants-tenanttag.md)|<span data-ttu-id="9ee04-118">读取 [tenantTag](../resources/managedtenants-tenanttag.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ee04-118">Read the properties and relationships of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>|
|[<span data-ttu-id="9ee04-119">更新 tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-119">Update tenantTag</span></span>](../api/managedtenants-tenanttag-update.md)|[<span data-ttu-id="9ee04-120">microsoft.graph.managedTenants.tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-120">microsoft.graph.managedTenants.tenantTag</span></span>](../resources/managedtenants-tenanttag.md)|<span data-ttu-id="9ee04-121">更新 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9ee04-121">Update the properties of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>|
|[<span data-ttu-id="9ee04-122">删除 tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-122">Delete tenantTag</span></span>](../api/managedtenants-tenanttag-delete.md)|<span data-ttu-id="9ee04-123">无</span><span class="sxs-lookup"><span data-stu-id="9ee04-123">None</span></span>|<span data-ttu-id="9ee04-124">删除 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ee04-124">Deletes a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>|
|[<span data-ttu-id="9ee04-125">assignTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-125">assignTag</span></span>](../api/managedtenants-tenanttag-assigntag.md)|[<span data-ttu-id="9ee04-126">microsoft.graph.managedTenants.tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-126">microsoft.graph.managedTenants.tenantTag</span></span>](../resources/managedtenants-tenanttag.md)|<span data-ttu-id="9ee04-127">将租户标记分配给指定的托管租户。</span><span class="sxs-lookup"><span data-stu-id="9ee04-127">Assigns the tenant tag to the specified managed tenants.</span></span>|
|[<span data-ttu-id="9ee04-128">unassignTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-128">unassignTag</span></span>](../api/managedtenants-tenanttag-unassigntag.md)|[<span data-ttu-id="9ee04-129">microsoft.graph.managedTenants.tenantTag</span><span class="sxs-lookup"><span data-stu-id="9ee04-129">microsoft.graph.managedTenants.tenantTag</span></span>](../resources/managedtenants-tenanttag.md)|<span data-ttu-id="9ee04-130">从指定的托管租户中取消分配租户标记。</span><span class="sxs-lookup"><span data-stu-id="9ee04-130">Un-assigns the tenant tag from the specified managed tenants.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ee04-131">属性</span><span class="sxs-lookup"><span data-stu-id="9ee04-131">Properties</span></span>
|<span data-ttu-id="9ee04-132">属性</span><span class="sxs-lookup"><span data-stu-id="9ee04-132">Property</span></span>|<span data-ttu-id="9ee04-133">类型</span><span class="sxs-lookup"><span data-stu-id="9ee04-133">Type</span></span>|<span data-ttu-id="9ee04-134">说明</span><span class="sxs-lookup"><span data-stu-id="9ee04-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee04-135">createdByUserId</span><span class="sxs-lookup"><span data-stu-id="9ee04-135">createdByUserId</span></span>|<span data-ttu-id="9ee04-136">String</span><span class="sxs-lookup"><span data-stu-id="9ee04-136">String</span></span>|<span data-ttu-id="9ee04-137">创建租户标记的帐户的标识符。</span><span class="sxs-lookup"><span data-stu-id="9ee04-137">The identifier for the account that created the tenant tag.</span></span> <span data-ttu-id="9ee04-138">必填。</span><span class="sxs-lookup"><span data-stu-id="9ee04-138">Required.</span></span> <span data-ttu-id="9ee04-139">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-139">Read-only.</span></span>|
|<span data-ttu-id="9ee04-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee04-140">createdDateTime</span></span>|<span data-ttu-id="9ee04-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee04-141">DateTimeOffset</span></span>|<span data-ttu-id="9ee04-142">创建租户标记的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9ee04-142">The date and time when the tenant tag was created.</span></span> <span data-ttu-id="9ee04-143">必填。</span><span class="sxs-lookup"><span data-stu-id="9ee04-143">Required.</span></span> <span data-ttu-id="9ee04-144">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-144">Read-only.</span></span>|
|<span data-ttu-id="9ee04-145">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee04-145">deletedDateTime</span></span>|<span data-ttu-id="9ee04-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee04-146">DateTimeOffset</span></span>|<span data-ttu-id="9ee04-147">删除租户标记的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9ee04-147">The date and time when the tenant tag was deleted.</span></span> <span data-ttu-id="9ee04-148">必填。</span><span class="sxs-lookup"><span data-stu-id="9ee04-148">Required.</span></span> <span data-ttu-id="9ee04-149">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-149">Read-only.</span></span>|
|<span data-ttu-id="9ee04-150">说明</span><span class="sxs-lookup"><span data-stu-id="9ee04-150">description</span></span>|<span data-ttu-id="9ee04-151">String</span><span class="sxs-lookup"><span data-stu-id="9ee04-151">String</span></span>|<span data-ttu-id="9ee04-152">租户标记的说明。</span><span class="sxs-lookup"><span data-stu-id="9ee04-152">The description for the tenant tag.</span></span> <span data-ttu-id="9ee04-153">可选。</span><span class="sxs-lookup"><span data-stu-id="9ee04-153">Optional.</span></span> <span data-ttu-id="9ee04-154">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-154">Read-only.</span></span>|
|<span data-ttu-id="9ee04-155">displayName</span><span class="sxs-lookup"><span data-stu-id="9ee04-155">displayName</span></span>|<span data-ttu-id="9ee04-156">String</span><span class="sxs-lookup"><span data-stu-id="9ee04-156">String</span></span>|<span data-ttu-id="9ee04-157">租户显示名称的变量。</span><span class="sxs-lookup"><span data-stu-id="9ee04-157">The display name for the tenant tag.</span></span> <span data-ttu-id="9ee04-158">必填。</span><span class="sxs-lookup"><span data-stu-id="9ee04-158">Required.</span></span> <span data-ttu-id="9ee04-159">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-159">Read-only.</span></span>|
|<span data-ttu-id="9ee04-160">id</span><span class="sxs-lookup"><span data-stu-id="9ee04-160">id</span></span>|<span data-ttu-id="9ee04-161">String</span><span class="sxs-lookup"><span data-stu-id="9ee04-161">String</span></span>|<span data-ttu-id="9ee04-162">租户标记的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9ee04-162">The unique identifier for the tenant tag.</span></span> <span data-ttu-id="9ee04-163">必填。</span><span class="sxs-lookup"><span data-stu-id="9ee04-163">Required.</span></span> <span data-ttu-id="9ee04-164">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-164">Read-only.</span></span>|
|<span data-ttu-id="9ee04-165">lastActionByUserId</span><span class="sxs-lookup"><span data-stu-id="9ee04-165">lastActionByUserId</span></span>|<span data-ttu-id="9ee04-166">String</span><span class="sxs-lookup"><span data-stu-id="9ee04-166">String</span></span>|<span data-ttu-id="9ee04-167">持续在租户标记上的帐户的标识符。</span><span class="sxs-lookup"><span data-stu-id="9ee04-167">The identifier for the account that lasted on the tenant tag.</span></span> <span data-ttu-id="9ee04-168">可选。</span><span class="sxs-lookup"><span data-stu-id="9ee04-168">Optional.</span></span> <span data-ttu-id="9ee04-169">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-169">Read-only.</span></span>|
|<span data-ttu-id="9ee04-170">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee04-170">lastActionDateTime</span></span>|<span data-ttu-id="9ee04-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee04-171">DateTimeOffset</span></span>|<span data-ttu-id="9ee04-172">上次对租户标记执行的操作的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9ee04-172">The date and time the last action was performed against the tenant tag.</span></span> <span data-ttu-id="9ee04-173">可选。</span><span class="sxs-lookup"><span data-stu-id="9ee04-173">Optional.</span></span> <span data-ttu-id="9ee04-174">只读。</span><span class="sxs-lookup"><span data-stu-id="9ee04-174">Read-only.</span></span>|
|<span data-ttu-id="9ee04-175">tenants</span><span class="sxs-lookup"><span data-stu-id="9ee04-175">tenants</span></span>|<span data-ttu-id="9ee04-176">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ee04-176">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) collection</span></span>|<span data-ttu-id="9ee04-177">与租户标记关联的托管租户的集合。</span><span class="sxs-lookup"><span data-stu-id="9ee04-177">The collection of managed tenants associated with the tenant tag.</span></span> <span data-ttu-id="9ee04-178">可选。</span><span class="sxs-lookup"><span data-stu-id="9ee04-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ee04-179">关系</span><span class="sxs-lookup"><span data-stu-id="9ee04-179">Relationships</span></span>
<span data-ttu-id="9ee04-180">无。</span><span class="sxs-lookup"><span data-stu-id="9ee04-180">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ee04-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ee04-181">JSON representation</span></span>
<span data-ttu-id="9ee04-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ee04-182">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantTag",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdByUserId": "String",
  "lastActionByUserId": "String",
  "tenants": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
    }
  ],
  "lastActionDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)"
}
```
