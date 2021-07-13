---
title: riskyUser 资源类型
description: 表示每个托管租户中标记为风险的帐户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3f66998080abcf9580cdd36e0f3e4b24edab2d2d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402398"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="1c43f-103">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c43f-103">riskyUser resource type</span></span>

<span data-ttu-id="1c43f-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="1c43f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c43f-105">表示每个托管租户中标记为风险的帐户。</span><span class="sxs-lookup"><span data-stu-id="1c43f-105">Represents an account flagged for risk across each managed tenants.</span></span>

## <a name="methods"></a><span data-ttu-id="1c43f-106">方法</span><span class="sxs-lookup"><span data-stu-id="1c43f-106">Methods</span></span>
|<span data-ttu-id="1c43f-107">方法</span><span class="sxs-lookup"><span data-stu-id="1c43f-107">Method</span></span>|<span data-ttu-id="1c43f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c43f-108">Return type</span></span>|<span data-ttu-id="1c43f-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c43f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c43f-110">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1c43f-110">List riskyUsers</span></span>](../api/managedtenants-managedtenant-list-riskyusers.md)|<span data-ttu-id="1c43f-111">[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c43f-111">[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md) collection</span></span>|<span data-ttu-id="1c43f-112">获取 [riskyUser](../resources/managedtenants-riskyuser.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="1c43f-112">Get a list of the [riskyUser](../resources/managedtenants-riskyuser.md) objects and their properties.</span></span>|
|[<span data-ttu-id="1c43f-113">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="1c43f-113">Get riskyUser</span></span>](../api/managedtenants-riskyuser-get.md)|[<span data-ttu-id="1c43f-114">microsoft.graph.managedTenants.riskyUser</span><span class="sxs-lookup"><span data-stu-id="1c43f-114">microsoft.graph.managedTenants.riskyUser</span></span>](../resources/managedtenants-riskyuser.md)|<span data-ttu-id="1c43f-115">读取 [riskyUser](../resources/managedtenants-riskyuser.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1c43f-115">Read the properties and relationships of a [riskyUser](../resources/managedtenants-riskyuser.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c43f-116">属性</span><span class="sxs-lookup"><span data-stu-id="1c43f-116">Properties</span></span>
|<span data-ttu-id="1c43f-117">属性</span><span class="sxs-lookup"><span data-stu-id="1c43f-117">Property</span></span>|<span data-ttu-id="1c43f-118">类型</span><span class="sxs-lookup"><span data-stu-id="1c43f-118">Type</span></span>|<span data-ttu-id="1c43f-119">说明</span><span class="sxs-lookup"><span data-stu-id="1c43f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c43f-120">id</span><span class="sxs-lookup"><span data-stu-id="1c43f-120">id</span></span>|<span data-ttu-id="1c43f-121">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-121">String</span></span>|<span data-ttu-id="1c43f-122">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1c43f-122">The unique identifier for this entity.</span></span> <span data-ttu-id="1c43f-123">必填。</span><span class="sxs-lookup"><span data-stu-id="1c43f-123">Required.</span></span> <span data-ttu-id="1c43f-124">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-124">Read-only.</span></span>|
|<span data-ttu-id="1c43f-125">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1c43f-125">isDeleted</span></span>|<span data-ttu-id="1c43f-126">布尔</span><span class="sxs-lookup"><span data-stu-id="1c43f-126">Boolean</span></span>|<span data-ttu-id="1c43f-127">指示帐户是否已删除的标志。</span><span class="sxs-lookup"><span data-stu-id="1c43f-127">A flag indicating whether the account has been deleted.</span></span> <span data-ttu-id="1c43f-128">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-128">Optional.</span></span> <span data-ttu-id="1c43f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-129">Read-only.</span></span>|
|<span data-ttu-id="1c43f-130">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c43f-130">lastRefreshedDateTime</span></span>|<span data-ttu-id="1c43f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c43f-131">DateTimeOffset</span></span>|<span data-ttu-id="1c43f-132">实体上次在多租户管理平台中更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1c43f-132">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="1c43f-133">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-133">Optional.</span></span> <span data-ttu-id="1c43f-134">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-134">Read-only.</span></span>|
|<span data-ttu-id="1c43f-135">riskDetail</span><span class="sxs-lookup"><span data-stu-id="1c43f-135">riskDetail</span></span>|<span data-ttu-id="1c43f-136">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-136">String</span></span>|<span data-ttu-id="1c43f-137">标记为风险的帐户的风险详细信息。</span><span class="sxs-lookup"><span data-stu-id="1c43f-137">The risk details for the account flagged for risk.</span></span> <span data-ttu-id="1c43f-138">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-138">Optional.</span></span> <span data-ttu-id="1c43f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-139">Read-only.</span></span>|
|<span data-ttu-id="1c43f-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c43f-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="1c43f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c43f-141">DateTimeOffset</span></span>|<span data-ttu-id="1c43f-142">上次更新风险信息的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1c43f-142">The date and time when the risk information was last updated.</span></span> <span data-ttu-id="1c43f-143">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-143">Optional.</span></span> <span data-ttu-id="1c43f-144">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-144">Read-only.</span></span>|
|<span data-ttu-id="1c43f-145">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1c43f-145">riskLevel</span></span>|<span data-ttu-id="1c43f-146">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-146">String</span></span>|<span data-ttu-id="1c43f-147">检测到的风险级别。</span><span class="sxs-lookup"><span data-stu-id="1c43f-147">The level of risk that was detected.</span></span> <span data-ttu-id="1c43f-148">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1c43f-148">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="1c43f-149">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-149">Optional.</span></span> <span data-ttu-id="1c43f-150">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-150">Read-only.</span></span>|
|<span data-ttu-id="1c43f-151">riskState</span><span class="sxs-lookup"><span data-stu-id="1c43f-151">riskState</span></span>|<span data-ttu-id="1c43f-152">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-152">String</span></span>|<span data-ttu-id="1c43f-153">检测到的风险状态。</span><span class="sxs-lookup"><span data-stu-id="1c43f-153">The state of risk that was detected.</span></span> <span data-ttu-id="1c43f-154">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1c43f-154">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="1c43f-155">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-155">Optional.</span></span> <span data-ttu-id="1c43f-156">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-156">Read-only.</span></span>|
|<span data-ttu-id="1c43f-157">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="1c43f-157">tenantDisplayName</span></span>|<span data-ttu-id="1c43f-158">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-158">String</span></span>|<span data-ttu-id="1c43f-159">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="1c43f-159">The display name for the managed tenant.</span></span> <span data-ttu-id="1c43f-160">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-160">Optional.</span></span> <span data-ttu-id="1c43f-161">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-161">Read-only.</span></span>|
|<span data-ttu-id="1c43f-162">tenantId</span><span class="sxs-lookup"><span data-stu-id="1c43f-162">tenantId</span></span>|<span data-ttu-id="1c43f-163">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-163">String</span></span>|<span data-ttu-id="1c43f-164">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="1c43f-164">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="1c43f-165">必填。</span><span class="sxs-lookup"><span data-stu-id="1c43f-165">Required.</span></span> <span data-ttu-id="1c43f-166">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-166">Read-only.</span></span>|
|<span data-ttu-id="1c43f-167">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1c43f-167">userDisplayName</span></span>|<span data-ttu-id="1c43f-168">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-168">String</span></span>|<span data-ttu-id="1c43f-169">The 显示名称 for the account where risk was detected.</span><span class="sxs-lookup"><span data-stu-id="1c43f-169">The display name for the account where risk was detected.</span></span> <span data-ttu-id="1c43f-170">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-170">Optional.</span></span> <span data-ttu-id="1c43f-171">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-171">Read-only.</span></span>|
|<span data-ttu-id="1c43f-172">userId</span><span class="sxs-lookup"><span data-stu-id="1c43f-172">userId</span></span>|<span data-ttu-id="1c43f-173">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-173">String</span></span>|<span data-ttu-id="1c43f-174">检测到风险的用户帐户的标识符。</span><span class="sxs-lookup"><span data-stu-id="1c43f-174">The identifier for the user account where risk was detected.</span></span> <span data-ttu-id="1c43f-175">必填。</span><span class="sxs-lookup"><span data-stu-id="1c43f-175">Required.</span></span> <span data-ttu-id="1c43f-176">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-176">Read-only.</span></span>|
|<span data-ttu-id="1c43f-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1c43f-177">userPrincipalName</span></span>|<span data-ttu-id="1c43f-178">String</span><span class="sxs-lookup"><span data-stu-id="1c43f-178">String</span></span>|<span data-ttu-id="1c43f-179">用户主体名称 (检测) 帐户的 UPN 名称。</span><span class="sxs-lookup"><span data-stu-id="1c43f-179">The user principal name (UPN) for the account where risk was detected.</span></span> <span data-ttu-id="1c43f-180">可选。</span><span class="sxs-lookup"><span data-stu-id="1c43f-180">Optional.</span></span> <span data-ttu-id="1c43f-181">只读。</span><span class="sxs-lookup"><span data-stu-id="1c43f-181">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c43f-182">关系</span><span class="sxs-lookup"><span data-stu-id="1c43f-182">Relationships</span></span>
<span data-ttu-id="1c43f-183">无。</span><span class="sxs-lookup"><span data-stu-id="1c43f-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c43f-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c43f-184">JSON representation</span></span>
<span data-ttu-id="1c43f-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c43f-185">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
