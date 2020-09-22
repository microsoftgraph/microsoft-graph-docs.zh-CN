---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7af5b2ab614dae57ef7c18aee80133cd7a2096a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984066"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="9aabc-104">secureScoreControlProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="9aabc-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="9aabc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9aabc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9aabc-106">表示租户的每个控件数据的安全分数。</span><span class="sxs-lookup"><span data-stu-id="9aabc-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="9aabc-107">默认情况下，它将返回租户的所有控件，并可显式提取各个控件。</span><span class="sxs-lookup"><span data-stu-id="9aabc-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="9aabc-108">方法</span><span class="sxs-lookup"><span data-stu-id="9aabc-108">Methods</span></span>

| <span data-ttu-id="9aabc-109">方法</span><span class="sxs-lookup"><span data-stu-id="9aabc-109">Method</span></span>   | <span data-ttu-id="9aabc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9aabc-110">Return Type</span></span>|<span data-ttu-id="9aabc-111">说明</span><span class="sxs-lookup"><span data-stu-id="9aabc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9aabc-112">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="9aabc-112">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="9aabc-113">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="9aabc-113">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="9aabc-114">读取 secureScoreControlProfiles 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="9aabc-114">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="9aabc-115">获取 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="9aabc-115">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="9aabc-116">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="9aabc-116">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="9aabc-117">读取 secureScoreControlProfiles 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="9aabc-117">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="9aabc-118">更新 securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="9aabc-118">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="9aabc-119">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="9aabc-119">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="9aabc-120">更新 securescorecontrolprofile 对象。</span><span class="sxs-lookup"><span data-stu-id="9aabc-120">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="9aabc-121">属性</span><span class="sxs-lookup"><span data-stu-id="9aabc-121">Properties</span></span>

|<span data-ttu-id="9aabc-122">名称</span><span class="sxs-lookup"><span data-stu-id="9aabc-122">Name</span></span> |<span data-ttu-id="9aabc-123">类型</span><span class="sxs-lookup"><span data-stu-id="9aabc-123">Type</span></span> |<span data-ttu-id="9aabc-124">说明</span><span class="sxs-lookup"><span data-stu-id="9aabc-124">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="9aabc-125">id</span><span class="sxs-lookup"><span data-stu-id="9aabc-125">id</span></span>|<span data-ttu-id="9aabc-126">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-126">String</span></span>|<span data-ttu-id="9aabc-127">提供程序生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9aabc-127">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="9aabc-128">只读。</span><span class="sxs-lookup"><span data-stu-id="9aabc-128">Read-only.</span></span> <span data-ttu-id="9aabc-129">必需。</span><span class="sxs-lookup"><span data-stu-id="9aabc-129">Required.</span></span>|
|<span data-ttu-id="9aabc-130">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="9aabc-130">azureTenantId</span></span>|<span data-ttu-id="9aabc-131">字符串</span><span class="sxs-lookup"><span data-stu-id="9aabc-131">String</span></span>|<span data-ttu-id="9aabc-132">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="9aabc-132">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="9aabc-133">actionType</span><span class="sxs-lookup"><span data-stu-id="9aabc-133">actionType</span></span>|<span data-ttu-id="9aabc-134">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-134">String</span></span>|<span data-ttu-id="9aabc-135">Control action type (Config、审阅和行为) 。</span><span class="sxs-lookup"><span data-stu-id="9aabc-135">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="9aabc-136">actionUrl</span><span class="sxs-lookup"><span data-stu-id="9aabc-136">actionUrl</span></span>|<span data-ttu-id="9aabc-137">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-137">String</span></span>|<span data-ttu-id="9aabc-138">可将控件 actioned 到的位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="9aabc-138">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="9aabc-139">controlCategory</span><span class="sxs-lookup"><span data-stu-id="9aabc-139">controlCategory</span></span>|<span data-ttu-id="9aabc-140">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-140">String</span></span>|<span data-ttu-id="9aabc-141">控制操作类别 (标识、数据、设备、应用程序、基础结构) 。</span><span class="sxs-lookup"><span data-stu-id="9aabc-141">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="9aabc-142">title</span><span class="sxs-lookup"><span data-stu-id="9aabc-142">title</span></span>|<span data-ttu-id="9aabc-143">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-143">String</span></span>|<span data-ttu-id="9aabc-144">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="9aabc-144">Title of the control.</span></span>|
|<span data-ttu-id="9aabc-145">被</span><span class="sxs-lookup"><span data-stu-id="9aabc-145">deprecated</span></span>|<span data-ttu-id="9aabc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9aabc-146">Boolean</span></span>|<span data-ttu-id="9aabc-147">指示是否已对控件进行折旧的标志。</span><span class="sxs-lookup"><span data-stu-id="9aabc-147">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="9aabc-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="9aabc-148">implementationCost</span></span>|<span data-ttu-id="9aabc-149">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-149">String</span></span>|<span data-ttu-id="9aabc-150">Implemmentating 控件的资源成本 (low、适中、高) 。</span><span class="sxs-lookup"><span data-stu-id="9aabc-150">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="9aabc-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9aabc-151">lastModifiedDateTime</span></span>|<span data-ttu-id="9aabc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aabc-152">DateTimeOffset</span></span>|<span data-ttu-id="9aabc-153">上次修改控件配置文件实体的时间。</span><span class="sxs-lookup"><span data-stu-id="9aabc-153">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="9aabc-154">时间戳类型表示日期和时间</span><span class="sxs-lookup"><span data-stu-id="9aabc-154">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="9aabc-155">maxScore</span><span class="sxs-lookup"><span data-stu-id="9aabc-155">maxScore</span></span>|<span data-ttu-id="9aabc-156">双精度</span><span class="sxs-lookup"><span data-stu-id="9aabc-156">Double</span></span>|<span data-ttu-id="9aabc-157">控件的最大实现得分。</span><span class="sxs-lookup"><span data-stu-id="9aabc-157">max attainable score for the control.</span></span>|
|<span data-ttu-id="9aabc-158">排名</span><span class="sxs-lookup"><span data-stu-id="9aabc-158">rank</span></span>|<span data-ttu-id="9aabc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9aabc-159">Int32</span></span>|<span data-ttu-id="9aabc-160">Microsoft 的控制堆栈排名。</span><span class="sxs-lookup"><span data-stu-id="9aabc-160">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="9aabc-161">纠正</span><span class="sxs-lookup"><span data-stu-id="9aabc-161">remediation</span></span>|<span data-ttu-id="9aabc-162">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-162">String</span></span>|<span data-ttu-id="9aabc-163">对控件将有助于修正的内容的说明。</span><span class="sxs-lookup"><span data-stu-id="9aabc-163">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="9aabc-164">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="9aabc-164">remediationImpact</span></span>|<span data-ttu-id="9aabc-165">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-165">String</span></span>|<span data-ttu-id="9aabc-166">对修正用户影响的说明。</span><span class="sxs-lookup"><span data-stu-id="9aabc-166">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="9aabc-167">service</span><span class="sxs-lookup"><span data-stu-id="9aabc-167">service</span></span>|<span data-ttu-id="9aabc-168">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-168">String</span></span>|<span data-ttu-id="9aabc-169">拥有控件 (Exchange、Sharepoint、Azure AD) 的服务。</span><span class="sxs-lookup"><span data-stu-id="9aabc-169">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="9aabc-170">病毒</span><span class="sxs-lookup"><span data-stu-id="9aabc-170">threats</span></span>|<span data-ttu-id="9aabc-171">String collection</span><span class="sxs-lookup"><span data-stu-id="9aabc-171">String collection</span></span>|<span data-ttu-id="9aabc-172">控制缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage 的威胁列表</span><span class="sxs-lookup"><span data-stu-id="9aabc-172">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="9aabc-173">elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗) 。</span><span class="sxs-lookup"><span data-stu-id="9aabc-173">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="9aabc-174">单层</span><span class="sxs-lookup"><span data-stu-id="9aabc-174">tier</span></span>|<span data-ttu-id="9aabc-175">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-175">String</span></span>|<span data-ttu-id="9aabc-176">控制层 (核心、纵深防御、高级 ) </span><span class="sxs-lookup"><span data-stu-id="9aabc-176">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="9aabc-177">userImpact</span><span class="sxs-lookup"><span data-stu-id="9aabc-177">userImpact</span></span>|<span data-ttu-id="9aabc-178">String</span><span class="sxs-lookup"><span data-stu-id="9aabc-178">String</span></span>|<span data-ttu-id="9aabc-179">实施控制 (低、中、高) 的用户影响。</span><span class="sxs-lookup"><span data-stu-id="9aabc-179">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="9aabc-180">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="9aabc-180">complianceInformation</span></span>|<span data-ttu-id="9aabc-181">[complianceInformation](complianceinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9aabc-181">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="9aabc-182">与安全得分控制相关联的合规性信息的集合</span><span class="sxs-lookup"><span data-stu-id="9aabc-182">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="9aabc-183">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="9aabc-183">controlStateUpdates</span></span>|<span data-ttu-id="9aabc-184">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9aabc-184">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="9aabc-185">用于指示租户已将控件标记 (忽略、thirdParty、已评审)  (支持 [更新](../api/securescorecontrolprofile-update.md)) 的标记。</span><span class="sxs-lookup"><span data-stu-id="9aabc-185">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="9aabc-186">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="9aabc-186">vendorInformation</span></span>|[<span data-ttu-id="9aabc-187">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="9aabc-187">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="9aabc-188">包含有关安全产品/服务供应商、提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft;provider = SecureScore) 。</span><span class="sxs-lookup"><span data-stu-id="9aabc-188">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="9aabc-189">必需。</span><span class="sxs-lookup"><span data-stu-id="9aabc-189">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aabc-190">关系</span><span class="sxs-lookup"><span data-stu-id="9aabc-190">Relationships</span></span>

<span data-ttu-id="9aabc-191">无。</span><span class="sxs-lookup"><span data-stu-id="9aabc-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aabc-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9aabc-192">JSON representation</span></span>

<span data-ttu-id="9aabc-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aabc-193">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

