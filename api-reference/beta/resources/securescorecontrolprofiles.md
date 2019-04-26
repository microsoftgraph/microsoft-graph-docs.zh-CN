---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。
localization_priority: Normal
ms.openlocfilehash: 41a74af0de47bbe77b8ea04cbea011a6f085d1bb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343407"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="bb800-104">secureScoreControlProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb800-104">secureScoreControlProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb800-105">表示租户的每个控件数据的安全分数。</span><span class="sxs-lookup"><span data-stu-id="bb800-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="bb800-106">默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。</span><span class="sxs-lookup"><span data-stu-id="bb800-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="bb800-107">方法</span><span class="sxs-lookup"><span data-stu-id="bb800-107">Methods</span></span>

| <span data-ttu-id="bb800-108">方法</span><span class="sxs-lookup"><span data-stu-id="bb800-108">Method</span></span>   | <span data-ttu-id="bb800-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb800-109">Return Type</span></span>|<span data-ttu-id="bb800-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb800-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb800-111">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="bb800-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="bb800-112">[secureScoreControlProfile](securescorecontrolprofiles.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb800-112">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="bb800-113">获取 secureScoreControlProfile 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bb800-113">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="bb800-114">属性</span><span class="sxs-lookup"><span data-stu-id="bb800-114">Properties</span></span>

|<span data-ttu-id="bb800-115">名称</span><span class="sxs-lookup"><span data-stu-id="bb800-115">Name</span></span> |<span data-ttu-id="bb800-116">类型</span><span class="sxs-lookup"><span data-stu-id="bb800-116">Type</span></span> |<span data-ttu-id="bb800-117">说明</span><span class="sxs-lookup"><span data-stu-id="bb800-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="bb800-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="bb800-118">azureTenantId</span></span>   |   <span data-ttu-id="bb800-119">String</span><span class="sxs-lookup"><span data-stu-id="bb800-119">String</span></span>  |   <span data-ttu-id="bb800-120">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="bb800-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="bb800-121">controlName</span><span class="sxs-lookup"><span data-stu-id="bb800-121">controlName</span></span> |   <span data-ttu-id="bb800-122">String</span><span class="sxs-lookup"><span data-stu-id="bb800-122">String</span></span>  |   <span data-ttu-id="bb800-123">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="bb800-123">Name of the control.</span></span> |
|   <span data-ttu-id="bb800-124">title</span><span class="sxs-lookup"><span data-stu-id="bb800-124">title</span></span>   |   <span data-ttu-id="bb800-125">String</span><span class="sxs-lookup"><span data-stu-id="bb800-125">String</span></span>  |   <span data-ttu-id="bb800-126">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="bb800-126">Title of the control.</span></span>   |
| <span data-ttu-id="bb800-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="bb800-127">complianceInformation</span></span> | <span data-ttu-id="bb800-128">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb800-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="bb800-129">与安全得分控制相关联的合规性信息的集合</span><span class="sxs-lookup"><span data-stu-id="bb800-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="bb800-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="bb800-130">controlCategory</span></span> |   <span data-ttu-id="bb800-131">String</span><span class="sxs-lookup"><span data-stu-id="bb800-131">String</span></span>  |   <span data-ttu-id="bb800-132">控制措施类别 (帐户、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="bb800-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="bb800-133">actionType</span><span class="sxs-lookup"><span data-stu-id="bb800-133">actionType</span></span>  |   <span data-ttu-id="bb800-134">String</span><span class="sxs-lookup"><span data-stu-id="bb800-134">String</span></span>  |   <span data-ttu-id="bb800-135">控制操作类型 (Config、审阅、行为)。</span><span class="sxs-lookup"><span data-stu-id="bb800-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="bb800-136">service</span><span class="sxs-lookup"><span data-stu-id="bb800-136">service</span></span> |   <span data-ttu-id="bb800-137">String</span><span class="sxs-lookup"><span data-stu-id="bb800-137">String</span></span>  |   <span data-ttu-id="bb800-138">拥有控件的服务 (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="bb800-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="bb800-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="bb800-139">maxScore</span></span> |  <span data-ttu-id="bb800-140">String</span><span class="sxs-lookup"><span data-stu-id="bb800-140">String</span></span>  |   <span data-ttu-id="bb800-141">指定日期的当前获得的最大分数。</span><span class="sxs-lookup"><span data-stu-id="bb800-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="bb800-142">单层</span><span class="sxs-lookup"><span data-stu-id="bb800-142">tier</span></span> |  <span data-ttu-id="bb800-143">String</span><span class="sxs-lookup"><span data-stu-id="bb800-143">String</span></span>  |   <span data-ttu-id="bb800-144">控制层 (Core, 纵深防御, 高级。)</span><span class="sxs-lookup"><span data-stu-id="bb800-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="bb800-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="bb800-145">userImpact</span></span> |    <span data-ttu-id="bb800-146">String</span><span class="sxs-lookup"><span data-stu-id="bb800-146">String</span></span>  | <span data-ttu-id="bb800-147">实施控制的用户影响 (低、中等、高)。</span><span class="sxs-lookup"><span data-stu-id="bb800-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="bb800-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="bb800-148">implementationCost</span></span> |    <span data-ttu-id="bb800-149">String</span><span class="sxs-lookup"><span data-stu-id="bb800-149">String</span></span>  |   <span data-ttu-id="bb800-150">implemmentating 控件的资源成本 (low、适中、high)。</span><span class="sxs-lookup"><span data-stu-id="bb800-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="bb800-151">排名</span><span class="sxs-lookup"><span data-stu-id="bb800-151">rank</span></span> |  <span data-ttu-id="bb800-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bb800-152">Int32</span></span>   |   <span data-ttu-id="bb800-153">Microsoft 的控制堆栈排名。</span><span class="sxs-lookup"><span data-stu-id="bb800-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="bb800-154">病毒</span><span class="sxs-lookup"><span data-stu-id="bb800-154">threats</span></span> |   <span data-ttu-id="bb800-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="bb800-155">String Collection</span></span>   |   <span data-ttu-id="bb800-156">控制缓解的威胁列表 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗)。</span><span class="sxs-lookup"><span data-stu-id="bb800-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="bb800-157">被</span><span class="sxs-lookup"><span data-stu-id="bb800-157">deprecated</span></span> |    <span data-ttu-id="bb800-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb800-158">Boolean</span></span> |   <span data-ttu-id="bb800-159">指示是否已对控件进行折旧的标志。</span><span class="sxs-lookup"><span data-stu-id="bb800-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="bb800-160">纠正</span><span class="sxs-lookup"><span data-stu-id="bb800-160">remediation</span></span> |   <span data-ttu-id="bb800-161">String</span><span class="sxs-lookup"><span data-stu-id="bb800-161">String</span></span>  |   <span data-ttu-id="bb800-162">对控件将有助于修正的内容的说明。</span><span class="sxs-lookup"><span data-stu-id="bb800-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="bb800-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="bb800-163">remediationImpact</span></span> | <span data-ttu-id="bb800-164">String</span><span class="sxs-lookup"><span data-stu-id="bb800-164">String</span></span>  |   <span data-ttu-id="bb800-165">对修正用户影响的说明。</span><span class="sxs-lookup"><span data-stu-id="bb800-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="bb800-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="bb800-166">actionUrl</span></span> | <span data-ttu-id="bb800-167">String</span><span class="sxs-lookup"><span data-stu-id="bb800-167">String</span></span>  |   <span data-ttu-id="bb800-168">可将控件 actioned 到的位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="bb800-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="bb800-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="bb800-169">controlStateUpdates</span></span> | <span data-ttu-id="bb800-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb800-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="bb800-171">用于指示租户已标记控件的位置的标志 (忽略、thirdParty、已审阅) (支持[更新](../api/securescorecontrolprofiles-update.md))。</span><span class="sxs-lookup"><span data-stu-id="bb800-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="bb800-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="bb800-172">vendorInformation</span></span> | [<span data-ttu-id="bb800-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="bb800-173">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="bb800-174">Relationships</span><span class="sxs-lookup"><span data-stu-id="bb800-174">Relationships</span></span>

<span data-ttu-id="bb800-175">无。</span><span class="sxs-lookup"><span data-stu-id="bb800-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb800-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb800-176">JSON representation</span></span>

<span data-ttu-id="bb800-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb800-177">The following is a JSON representation of the resource.</span></span>

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
