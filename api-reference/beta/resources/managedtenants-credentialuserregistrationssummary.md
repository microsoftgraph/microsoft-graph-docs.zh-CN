---
title: credentialUserRegistrationsSummary 资源类型
description: 表示给定托管Azure Active Directory的凭据用户注册的摘要。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 43a3f5cd39e8c151c71f976042e9bb33ae527dc4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402068"
---
# <a name="credentialuserregistrationssummary-resource-type"></a><span data-ttu-id="6e3c2-103">credentialUserRegistrationsSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e3c2-103">credentialUserRegistrationsSummary resource type</span></span>

<span data-ttu-id="6e3c2-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6e3c2-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e3c2-105">表示给定托管Azure Active Directory的凭据用户注册的摘要。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-105">Represents a summary of Azure Active Directory credential user registrations for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="6e3c2-106">方法</span><span class="sxs-lookup"><span data-stu-id="6e3c2-106">Methods</span></span>
|<span data-ttu-id="6e3c2-107">方法</span><span class="sxs-lookup"><span data-stu-id="6e3c2-107">Method</span></span>|<span data-ttu-id="6e3c2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6e3c2-108">Return type</span></span>|<span data-ttu-id="6e3c2-109">说明</span><span class="sxs-lookup"><span data-stu-id="6e3c2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e3c2-110">列出 credentialUserRegistrationsSummaries</span><span class="sxs-lookup"><span data-stu-id="6e3c2-110">List credentialUserRegistrationsSummaries</span></span>](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|<span data-ttu-id="6e3c2-111">[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6e3c2-111">[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) collection</span></span>|<span data-ttu-id="6e3c2-112">获取 [credentialUserRegistrationsSummary 对象](../resources/managedtenants-credentialuserregistrationssummary.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-112">Get a list of the [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects and their properties.</span></span>|
|[<span data-ttu-id="6e3c2-113">获取 credentialUserRegistrationsSummary</span><span class="sxs-lookup"><span data-stu-id="6e3c2-113">Get credentialUserRegistrationsSummary</span></span>](../api/managedtenants-credentialuserregistrationssummary-get.md)|[<span data-ttu-id="6e3c2-114">microsoft.graph.managedTenants.credentialUserRegistrationsSummary</span><span class="sxs-lookup"><span data-stu-id="6e3c2-114">microsoft.graph.managedTenants.credentialUserRegistrationsSummary</span></span>](../resources/managedtenants-credentialuserregistrationssummary.md)|<span data-ttu-id="6e3c2-115">读取 [credentialUserRegistrationsSummary 对象的属性和](../resources/managedtenants-credentialuserregistrationssummary.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-115">Read the properties and relationships of a [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e3c2-116">属性</span><span class="sxs-lookup"><span data-stu-id="6e3c2-116">Properties</span></span>
|<span data-ttu-id="6e3c2-117">属性</span><span class="sxs-lookup"><span data-stu-id="6e3c2-117">Property</span></span>|<span data-ttu-id="6e3c2-118">类型</span><span class="sxs-lookup"><span data-stu-id="6e3c2-118">Type</span></span>|<span data-ttu-id="6e3c2-119">说明</span><span class="sxs-lookup"><span data-stu-id="6e3c2-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e3c2-120">id</span><span class="sxs-lookup"><span data-stu-id="6e3c2-120">id</span></span>|<span data-ttu-id="6e3c2-121">String</span><span class="sxs-lookup"><span data-stu-id="6e3c2-121">String</span></span>|<span data-ttu-id="6e3c2-122">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-122">The unique identifier for this entity.</span></span> <span data-ttu-id="6e3c2-123">必填。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-123">Required.</span></span> <span data-ttu-id="6e3c2-124">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-124">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-125">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e3c2-125">lastRefreshedDateTime</span></span>|<span data-ttu-id="6e3c2-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e3c2-126">DateTimeOffset</span></span>|<span data-ttu-id="6e3c2-127">实体上次在多租户管理平台中更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-127">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="6e3c2-128">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-128">Optional.</span></span> <span data-ttu-id="6e3c2-129">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-129">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-130">mfaAndSsprCapableUserCount</span><span class="sxs-lookup"><span data-stu-id="6e3c2-130">mfaAndSsprCapableUserCount</span></span>|<span data-ttu-id="6e3c2-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6e3c2-131">Int32</span></span>|<span data-ttu-id="6e3c2-132">能够执行多重身份验证或自助服务密码重置的用户数。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-132">The number of users that are capable of performing multi-factor authentication or self service password reset.</span></span> <span data-ttu-id="6e3c2-133">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-133">Optional.</span></span> <span data-ttu-id="6e3c2-134">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-134">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-135">mfaConditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="6e3c2-135">mfaConditionalAccessPolicyState</span></span>|<span data-ttu-id="6e3c2-136">String</span><span class="sxs-lookup"><span data-stu-id="6e3c2-136">String</span></span>|<span data-ttu-id="6e3c2-137">强制执行多重身份验证的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-137">The state of a conditional access policy that enforces multi-factor authentication.</span></span> <span data-ttu-id="6e3c2-138">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-138">Optional.</span></span> <span data-ttu-id="6e3c2-139">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-139">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-140">mfaRegisteredUserCount</span><span class="sxs-lookup"><span data-stu-id="6e3c2-140">mfaRegisteredUserCount</span></span>|<span data-ttu-id="6e3c2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6e3c2-141">Int32</span></span>|<span data-ttu-id="6e3c2-142">注册多重身份验证的用户数。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-142">The number of users registered for multi-factor authentication.</span></span> <span data-ttu-id="6e3c2-143">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-143">Optional.</span></span> <span data-ttu-id="6e3c2-144">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-144">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-145">securityDefaultsEnabled</span><span class="sxs-lookup"><span data-stu-id="6e3c2-145">securityDefaultsEnabled</span></span>|<span data-ttu-id="6e3c2-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6e3c2-146">Boolean</span></span>|<span data-ttu-id="6e3c2-147">一个标志，指示是否已启用标识安全性默认值。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-147">A flag indicating whether Identity Security Defaults is enabled.</span></span> <span data-ttu-id="6e3c2-148">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-148">Optional.</span></span> <span data-ttu-id="6e3c2-149">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-149">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-150">ssprEnabledUserCount</span><span class="sxs-lookup"><span data-stu-id="6e3c2-150">ssprEnabledUserCount</span></span>|<span data-ttu-id="6e3c2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6e3c2-151">Int32</span></span>|<span data-ttu-id="6e3c2-152">启用自助服务密码重置的用户数。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-152">The number of users enabled for self service password reset.</span></span> <span data-ttu-id="6e3c2-153">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-153">Optional.</span></span> <span data-ttu-id="6e3c2-154">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-154">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-155">ssprRegisteredUserCount</span><span class="sxs-lookup"><span data-stu-id="6e3c2-155">ssprRegisteredUserCount</span></span>|<span data-ttu-id="6e3c2-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6e3c2-156">Int32</span></span>|<span data-ttu-id="6e3c2-157">注册自助服务密码重置的用户数。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-157">The number of users registered for self service password reset.</span></span> <span data-ttu-id="6e3c2-158">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-158">Optional.</span></span> <span data-ttu-id="6e3c2-159">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-159">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-160">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e3c2-160">tenantDisplayName</span></span>|<span data-ttu-id="6e3c2-161">String</span><span class="sxs-lookup"><span data-stu-id="6e3c2-161">String</span></span>|<span data-ttu-id="6e3c2-162">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-162">The display name for the managed tenant.</span></span> <span data-ttu-id="6e3c2-163">必填。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-163">Required.</span></span> <span data-ttu-id="6e3c2-164">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-164">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-165">tenantId</span><span class="sxs-lookup"><span data-stu-id="6e3c2-165">tenantId</span></span>|<span data-ttu-id="6e3c2-166">String</span><span class="sxs-lookup"><span data-stu-id="6e3c2-166">String</span></span>|<span data-ttu-id="6e3c2-167">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-167">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="6e3c2-168">必填。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-168">Required.</span></span> <span data-ttu-id="6e3c2-169">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-169">Read-only.</span></span>|
|<span data-ttu-id="6e3c2-170">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="6e3c2-170">totalUserCount</span></span>|<span data-ttu-id="6e3c2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6e3c2-171">Int32</span></span>|<span data-ttu-id="6e3c2-172">给定托管租户中的用户总数。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-172">The total number of users in the given managed tenant.</span></span> <span data-ttu-id="6e3c2-173">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-173">Optional.</span></span> <span data-ttu-id="6e3c2-174">只读。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-174">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e3c2-175">关系</span><span class="sxs-lookup"><span data-stu-id="6e3c2-175">Relationships</span></span>
<span data-ttu-id="6e3c2-176">无。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e3c2-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e3c2-177">JSON representation</span></span>
<span data-ttu-id="6e3c2-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e3c2-178">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
