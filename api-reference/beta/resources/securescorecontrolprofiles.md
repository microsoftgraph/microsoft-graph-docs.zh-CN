---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5e244576cb014719d454fe37bd8395054efe2e2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965276"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="7c752-104">secureScoreControlProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c752-104">secureScoreControlProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c752-105">表示租户的每个控件数据的安全分数。</span><span class="sxs-lookup"><span data-stu-id="7c752-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="7c752-106">默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。</span><span class="sxs-lookup"><span data-stu-id="7c752-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="7c752-107">方法</span><span class="sxs-lookup"><span data-stu-id="7c752-107">Methods</span></span>

| <span data-ttu-id="7c752-108">方法</span><span class="sxs-lookup"><span data-stu-id="7c752-108">Method</span></span>   | <span data-ttu-id="7c752-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c752-109">Return Type</span></span>|<span data-ttu-id="7c752-110">说明</span><span class="sxs-lookup"><span data-stu-id="7c752-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c752-111">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="7c752-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="7c752-112">[secureScoreControlProfile](securescorecontrolprofiles.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c752-112">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="7c752-113">获取 secureScoreControlProfile 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="7c752-113">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="7c752-114">属性</span><span class="sxs-lookup"><span data-stu-id="7c752-114">Properties</span></span>

|<span data-ttu-id="7c752-115">名称</span><span class="sxs-lookup"><span data-stu-id="7c752-115">Name</span></span> |<span data-ttu-id="7c752-116">类型</span><span class="sxs-lookup"><span data-stu-id="7c752-116">Type</span></span> |<span data-ttu-id="7c752-117">说明</span><span class="sxs-lookup"><span data-stu-id="7c752-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="7c752-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="7c752-118">azureTenantId</span></span>   |   <span data-ttu-id="7c752-119">字符串</span><span class="sxs-lookup"><span data-stu-id="7c752-119">String</span></span>  |   <span data-ttu-id="7c752-120">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="7c752-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="7c752-121">controlName</span><span class="sxs-lookup"><span data-stu-id="7c752-121">controlName</span></span> |   <span data-ttu-id="7c752-122">String</span><span class="sxs-lookup"><span data-stu-id="7c752-122">String</span></span>  |   <span data-ttu-id="7c752-123">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="7c752-123">Name of the control.</span></span> |
|   <span data-ttu-id="7c752-124">title</span><span class="sxs-lookup"><span data-stu-id="7c752-124">title</span></span>   |   <span data-ttu-id="7c752-125">String</span><span class="sxs-lookup"><span data-stu-id="7c752-125">String</span></span>  |   <span data-ttu-id="7c752-126">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="7c752-126">Title of the control.</span></span>   |
| <span data-ttu-id="7c752-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="7c752-127">complianceInformation</span></span> | <span data-ttu-id="7c752-128">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c752-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="7c752-129">与安全得分控制相关联的合规性信息的集合</span><span class="sxs-lookup"><span data-stu-id="7c752-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="7c752-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="7c752-130">controlCategory</span></span> |   <span data-ttu-id="7c752-131">String</span><span class="sxs-lookup"><span data-stu-id="7c752-131">String</span></span>  |   <span data-ttu-id="7c752-132">控制措施类别 (帐户、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="7c752-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="7c752-133">actionType</span><span class="sxs-lookup"><span data-stu-id="7c752-133">actionType</span></span>  |   <span data-ttu-id="7c752-134">String</span><span class="sxs-lookup"><span data-stu-id="7c752-134">String</span></span>  |   <span data-ttu-id="7c752-135">控制操作类型 (Config、审阅、行为)。</span><span class="sxs-lookup"><span data-stu-id="7c752-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="7c752-136">service</span><span class="sxs-lookup"><span data-stu-id="7c752-136">service</span></span> |   <span data-ttu-id="7c752-137">String</span><span class="sxs-lookup"><span data-stu-id="7c752-137">String</span></span>  |   <span data-ttu-id="7c752-138">拥有控件的服务 (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="7c752-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="7c752-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="7c752-139">maxScore</span></span> |  <span data-ttu-id="7c752-140">String</span><span class="sxs-lookup"><span data-stu-id="7c752-140">String</span></span>  |   <span data-ttu-id="7c752-141">指定日期的当前获得的最大分数。</span><span class="sxs-lookup"><span data-stu-id="7c752-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="7c752-142">单层</span><span class="sxs-lookup"><span data-stu-id="7c752-142">tier</span></span> |  <span data-ttu-id="7c752-143">String</span><span class="sxs-lookup"><span data-stu-id="7c752-143">String</span></span>  |   <span data-ttu-id="7c752-144">控制层 (Core, 纵深防御, 高级。)</span><span class="sxs-lookup"><span data-stu-id="7c752-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="7c752-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="7c752-145">userImpact</span></span> |    <span data-ttu-id="7c752-146">String</span><span class="sxs-lookup"><span data-stu-id="7c752-146">String</span></span>  | <span data-ttu-id="7c752-147">实施控制的用户影响 (低、中等、高)。</span><span class="sxs-lookup"><span data-stu-id="7c752-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="7c752-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="7c752-148">implementationCost</span></span> |    <span data-ttu-id="7c752-149">String</span><span class="sxs-lookup"><span data-stu-id="7c752-149">String</span></span>  |   <span data-ttu-id="7c752-150">Implemmentating 控件的资源成本 (low、适中、high)。</span><span class="sxs-lookup"><span data-stu-id="7c752-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="7c752-151">排名</span><span class="sxs-lookup"><span data-stu-id="7c752-151">rank</span></span> |  <span data-ttu-id="7c752-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7c752-152">Int32</span></span>   |   <span data-ttu-id="7c752-153">Microsoft 的控制堆栈排名。</span><span class="sxs-lookup"><span data-stu-id="7c752-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="7c752-154">病毒</span><span class="sxs-lookup"><span data-stu-id="7c752-154">threats</span></span> |   <span data-ttu-id="7c752-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="7c752-155">String Collection</span></span>   |   <span data-ttu-id="7c752-156">控制缓解的威胁列表 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗)。</span><span class="sxs-lookup"><span data-stu-id="7c752-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="7c752-157">被</span><span class="sxs-lookup"><span data-stu-id="7c752-157">deprecated</span></span> |    <span data-ttu-id="7c752-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c752-158">Boolean</span></span> |   <span data-ttu-id="7c752-159">指示是否已对控件进行折旧的标志。</span><span class="sxs-lookup"><span data-stu-id="7c752-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="7c752-160">纠正</span><span class="sxs-lookup"><span data-stu-id="7c752-160">remediation</span></span> |   <span data-ttu-id="7c752-161">String</span><span class="sxs-lookup"><span data-stu-id="7c752-161">String</span></span>  |   <span data-ttu-id="7c752-162">对控件将有助于修正的内容的说明。</span><span class="sxs-lookup"><span data-stu-id="7c752-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="7c752-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="7c752-163">remediationImpact</span></span> | <span data-ttu-id="7c752-164">String</span><span class="sxs-lookup"><span data-stu-id="7c752-164">String</span></span>  |   <span data-ttu-id="7c752-165">对修正用户影响的说明。</span><span class="sxs-lookup"><span data-stu-id="7c752-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="7c752-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="7c752-166">actionUrl</span></span> | <span data-ttu-id="7c752-167">String</span><span class="sxs-lookup"><span data-stu-id="7c752-167">String</span></span>  |   <span data-ttu-id="7c752-168">可将控件 actioned 到的位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="7c752-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="7c752-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="7c752-169">controlStateUpdates</span></span> | <span data-ttu-id="7c752-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c752-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="7c752-171">用于指示租户已标记控件的位置的标志 (忽略、thirdParty、已审阅) (支持[更新](../api/securescorecontrolprofiles-update.md))。</span><span class="sxs-lookup"><span data-stu-id="7c752-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="7c752-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="7c752-172">vendorInformation</span></span> | [<span data-ttu-id="7c752-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="7c752-173">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="7c752-174">关系</span><span class="sxs-lookup"><span data-stu-id="7c752-174">Relationships</span></span>

<span data-ttu-id="7c752-175">无。</span><span class="sxs-lookup"><span data-stu-id="7c752-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c752-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c752-176">JSON representation</span></span>

<span data-ttu-id="7c752-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c752-177">The following is a JSON representation of the resource.</span></span>

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
