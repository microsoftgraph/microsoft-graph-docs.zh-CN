---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 3eeb7b0bd1575a336cdeb9ff73e808a057f61743
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807479"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="3f6bb-104">secureScoreControlProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f6bb-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="3f6bb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f6bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f6bb-106">表示租户的每个控件数据的安全分数。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="3f6bb-107">默认情况下，它将返回租户的所有控件，并可显式提取各个控件。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="3f6bb-108">方法</span><span class="sxs-lookup"><span data-stu-id="3f6bb-108">Methods</span></span>

| <span data-ttu-id="3f6bb-109">方法</span><span class="sxs-lookup"><span data-stu-id="3f6bb-109">Method</span></span>   | <span data-ttu-id="3f6bb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f6bb-110">Return Type</span></span>|<span data-ttu-id="3f6bb-111">说明</span><span class="sxs-lookup"><span data-stu-id="3f6bb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f6bb-112">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="3f6bb-112">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="3f6bb-113">[secureScoreControlProfile](securescorecontrolprofiles.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f6bb-113">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="3f6bb-114">获取 secureScoreControlProfile 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-114">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="3f6bb-115">属性</span><span class="sxs-lookup"><span data-stu-id="3f6bb-115">Properties</span></span>

|<span data-ttu-id="3f6bb-116">名称</span><span class="sxs-lookup"><span data-stu-id="3f6bb-116">Name</span></span> |<span data-ttu-id="3f6bb-117">类型</span><span class="sxs-lookup"><span data-stu-id="3f6bb-117">Type</span></span> |<span data-ttu-id="3f6bb-118">说明</span><span class="sxs-lookup"><span data-stu-id="3f6bb-118">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="3f6bb-119">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="3f6bb-119">azureTenantId</span></span>   |   <span data-ttu-id="3f6bb-120">字符串</span><span class="sxs-lookup"><span data-stu-id="3f6bb-120">String</span></span>  |   <span data-ttu-id="3f6bb-121">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-121">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="3f6bb-122">controlName</span><span class="sxs-lookup"><span data-stu-id="3f6bb-122">controlName</span></span> |   <span data-ttu-id="3f6bb-123">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-123">String</span></span>  |   <span data-ttu-id="3f6bb-124">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-124">Name of the control.</span></span> |
|   <span data-ttu-id="3f6bb-125">title</span><span class="sxs-lookup"><span data-stu-id="3f6bb-125">title</span></span>   |   <span data-ttu-id="3f6bb-126">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-126">String</span></span>  |   <span data-ttu-id="3f6bb-127">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-127">Title of the control.</span></span>   |
| <span data-ttu-id="3f6bb-128">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="3f6bb-128">complianceInformation</span></span> | <span data-ttu-id="3f6bb-129">[complianceInformation](complianceinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f6bb-129">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="3f6bb-130">与安全得分控制相关联的合规性信息的集合</span><span class="sxs-lookup"><span data-stu-id="3f6bb-130">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="3f6bb-131">controlCategory</span><span class="sxs-lookup"><span data-stu-id="3f6bb-131">controlCategory</span></span> |   <span data-ttu-id="3f6bb-132">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-132">String</span></span>  |   <span data-ttu-id="3f6bb-133">控制操作类别 (帐户、数据、设备、应用程序、基础结构) 。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-133">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="3f6bb-134">actionType</span><span class="sxs-lookup"><span data-stu-id="3f6bb-134">actionType</span></span>  |   <span data-ttu-id="3f6bb-135">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-135">String</span></span>  |   <span data-ttu-id="3f6bb-136">Control action type (Config、审阅和行为) 。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-136">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="3f6bb-137">service</span><span class="sxs-lookup"><span data-stu-id="3f6bb-137">service</span></span> |   <span data-ttu-id="3f6bb-138">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-138">String</span></span>  |   <span data-ttu-id="3f6bb-139">拥有控件 (Exchange、Sharepoint、Azure AD) 的服务。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-139">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="3f6bb-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="3f6bb-140">maxScore</span></span> |  <span data-ttu-id="3f6bb-141">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-141">String</span></span>  |   <span data-ttu-id="3f6bb-142">指定日期的当前获得的最大分数。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-142">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="3f6bb-143">单层</span><span class="sxs-lookup"><span data-stu-id="3f6bb-143">tier</span></span> |  <span data-ttu-id="3f6bb-144">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-144">String</span></span>  |   <span data-ttu-id="3f6bb-145">控制层 (核心、纵深防御、高级 ) </span><span class="sxs-lookup"><span data-stu-id="3f6bb-145">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="3f6bb-146">userImpact</span><span class="sxs-lookup"><span data-stu-id="3f6bb-146">userImpact</span></span> |    <span data-ttu-id="3f6bb-147">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-147">String</span></span>  | <span data-ttu-id="3f6bb-148">实施控制 (低、中、高) 的用户影响。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-148">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="3f6bb-149">implementationCost</span><span class="sxs-lookup"><span data-stu-id="3f6bb-149">implementationCost</span></span> |    <span data-ttu-id="3f6bb-150">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-150">String</span></span>  |   <span data-ttu-id="3f6bb-151">Implemmentating 控件的资源成本 (low、适中、高) 。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-151">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="3f6bb-152">排名</span><span class="sxs-lookup"><span data-stu-id="3f6bb-152">rank</span></span> |  <span data-ttu-id="3f6bb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3f6bb-153">Int32</span></span>   |   <span data-ttu-id="3f6bb-154">Microsoft 的控制堆栈排名。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-154">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="3f6bb-155">病毒</span><span class="sxs-lookup"><span data-stu-id="3f6bb-155">threats</span></span> |   <span data-ttu-id="3f6bb-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="3f6bb-156">String Collection</span></span>   |   <span data-ttu-id="3f6bb-157">控制缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗) 的威胁列表。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-157">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="3f6bb-158">被</span><span class="sxs-lookup"><span data-stu-id="3f6bb-158">deprecated</span></span> |    <span data-ttu-id="3f6bb-159">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f6bb-159">Boolean</span></span> |   <span data-ttu-id="3f6bb-160">指示是否已对控件进行折旧的标志。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-160">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="3f6bb-161">纠正</span><span class="sxs-lookup"><span data-stu-id="3f6bb-161">remediation</span></span> |   <span data-ttu-id="3f6bb-162">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-162">String</span></span>  |   <span data-ttu-id="3f6bb-163">对控件将有助于修正的内容的说明。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-163">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="3f6bb-164">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="3f6bb-164">remediationImpact</span></span> | <span data-ttu-id="3f6bb-165">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-165">String</span></span>  |   <span data-ttu-id="3f6bb-166">对修正用户影响的说明。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-166">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="3f6bb-167">actionUrl</span><span class="sxs-lookup"><span data-stu-id="3f6bb-167">actionUrl</span></span> | <span data-ttu-id="3f6bb-168">String</span><span class="sxs-lookup"><span data-stu-id="3f6bb-168">String</span></span>  |   <span data-ttu-id="3f6bb-169">可将控件 actioned 到的位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-169">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="3f6bb-170">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="3f6bb-170">controlStateUpdates</span></span> | <span data-ttu-id="3f6bb-171">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f6bb-171">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="3f6bb-172">用于指示租户已将控件标记 (ignore、thirdParty、已评审)  (支持 [更新](../api/securescorecontrolprofiles-update.md)) 的标记。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-172">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="3f6bb-173">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="3f6bb-173">vendorInformation</span></span> | [<span data-ttu-id="3f6bb-174">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="3f6bb-174">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="3f6bb-175">关系</span><span class="sxs-lookup"><span data-stu-id="3f6bb-175">Relationships</span></span>

<span data-ttu-id="3f6bb-176">无。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f6bb-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f6bb-177">JSON representation</span></span>

<span data-ttu-id="3f6bb-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f6bb-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "title": "String",
  "azureTenantId": "String (identifier)",
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
