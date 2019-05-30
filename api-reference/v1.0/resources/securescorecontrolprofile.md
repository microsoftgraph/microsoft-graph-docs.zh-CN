---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 98b335d536ab64000b65756f8c60e0f401f028fd
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537196"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="ff4f8-104">secureScoreControlProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff4f8-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="ff4f8-105">表示租户的每个控件数据的安全分数。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="ff4f8-106">默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="ff4f8-107">方法</span><span class="sxs-lookup"><span data-stu-id="ff4f8-107">Methods</span></span>

| <span data-ttu-id="ff4f8-108">方法</span><span class="sxs-lookup"><span data-stu-id="ff4f8-108">Method</span></span>   | <span data-ttu-id="ff4f8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff4f8-109">Return Type</span></span>|<span data-ttu-id="ff4f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="ff4f8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff4f8-111">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="ff4f8-111">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="ff4f8-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="ff4f8-112">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="ff4f8-113">读取 secureScoreControlProfiles 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="ff4f8-114">获取 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="ff4f8-114">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="ff4f8-115">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="ff4f8-115">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="ff4f8-116">读取 secureScoreControlProfiles 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-116">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="ff4f8-117">更新 securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="ff4f8-117">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="ff4f8-118">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="ff4f8-118">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="ff4f8-119">更新 securescorecontrolprofile 对象。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-119">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="ff4f8-120">属性</span><span class="sxs-lookup"><span data-stu-id="ff4f8-120">Properties</span></span>

|<span data-ttu-id="ff4f8-121">名称</span><span class="sxs-lookup"><span data-stu-id="ff4f8-121">Name</span></span> |<span data-ttu-id="ff4f8-122">类型</span><span class="sxs-lookup"><span data-stu-id="ff4f8-122">Type</span></span> |<span data-ttu-id="ff4f8-123">说明</span><span class="sxs-lookup"><span data-stu-id="ff4f8-123">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ff4f8-124">id</span><span class="sxs-lookup"><span data-stu-id="ff4f8-124">id</span></span>|<span data-ttu-id="ff4f8-125">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-125">String</span></span>|<span data-ttu-id="ff4f8-126">提供程序生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-126">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="ff4f8-127">只读。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-127">Read-only.</span></span> <span data-ttu-id="ff4f8-128">必需。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-128">Required.</span></span>|
|<span data-ttu-id="ff4f8-129">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="ff4f8-129">azureTenantId</span></span>|<span data-ttu-id="ff4f8-130">字符串</span><span class="sxs-lookup"><span data-stu-id="ff4f8-130">String</span></span>|<span data-ttu-id="ff4f8-131">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-131">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="ff4f8-132">actionType</span><span class="sxs-lookup"><span data-stu-id="ff4f8-132">actionType</span></span>|<span data-ttu-id="ff4f8-133">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-133">String</span></span>|<span data-ttu-id="ff4f8-134">控制操作类型 (Config、审阅、行为)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-134">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="ff4f8-135">actionUrl</span><span class="sxs-lookup"><span data-stu-id="ff4f8-135">actionUrl</span></span>|<span data-ttu-id="ff4f8-136">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-136">String</span></span>|<span data-ttu-id="ff4f8-137">可将控件 actioned 到的位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-137">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="ff4f8-138">controlCategory</span><span class="sxs-lookup"><span data-stu-id="ff4f8-138">controlCategory</span></span>|<span data-ttu-id="ff4f8-139">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-139">String</span></span>|<span data-ttu-id="ff4f8-140">控制措施类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-140">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="ff4f8-141">title</span><span class="sxs-lookup"><span data-stu-id="ff4f8-141">title</span></span>|<span data-ttu-id="ff4f8-142">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-142">String</span></span>|<span data-ttu-id="ff4f8-143">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-143">Title of the control.</span></span>|
|<span data-ttu-id="ff4f8-144">被</span><span class="sxs-lookup"><span data-stu-id="ff4f8-144">deprecated</span></span>|<span data-ttu-id="ff4f8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff4f8-145">Boolean</span></span>|<span data-ttu-id="ff4f8-146">指示是否已对控件进行折旧的标志。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-146">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="ff4f8-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="ff4f8-147">implementationCost</span></span>|<span data-ttu-id="ff4f8-148">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-148">String</span></span>|<span data-ttu-id="ff4f8-149">Implemmentating 控件的资源成本 (low、适中、high)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-149">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="ff4f8-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff4f8-150">lastModifiedDateTime</span></span>|<span data-ttu-id="ff4f8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff4f8-151">DateTimeOffset</span></span>|<span data-ttu-id="ff4f8-152">上次修改控件配置文件实体的时间。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-152">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="ff4f8-153">时间戳类型表示日期和时间</span><span class="sxs-lookup"><span data-stu-id="ff4f8-153">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="ff4f8-154">maxScore</span><span class="sxs-lookup"><span data-stu-id="ff4f8-154">maxScore</span></span>|<span data-ttu-id="ff4f8-155">双精度</span><span class="sxs-lookup"><span data-stu-id="ff4f8-155">Double</span></span>|<span data-ttu-id="ff4f8-156">控件的最大实现得分。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-156">max attainable score for the control.</span></span>|
|<span data-ttu-id="ff4f8-157">排名</span><span class="sxs-lookup"><span data-stu-id="ff4f8-157">rank</span></span>|<span data-ttu-id="ff4f8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4f8-158">Int32</span></span>|<span data-ttu-id="ff4f8-159">Microsoft 的控制堆栈排名。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-159">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="ff4f8-160">纠正</span><span class="sxs-lookup"><span data-stu-id="ff4f8-160">remediation</span></span>|<span data-ttu-id="ff4f8-161">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-161">String</span></span>|<span data-ttu-id="ff4f8-162">对控件将有助于修正的内容的说明。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-162">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="ff4f8-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="ff4f8-163">remediationImpact</span></span>|<span data-ttu-id="ff4f8-164">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-164">String</span></span>|<span data-ttu-id="ff4f8-165">对修正用户影响的说明。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-165">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="ff4f8-166">service</span><span class="sxs-lookup"><span data-stu-id="ff4f8-166">service</span></span>|<span data-ttu-id="ff4f8-167">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-167">String</span></span>|<span data-ttu-id="ff4f8-168">拥有控件的服务 (Exchange、Sharepoint、Azure AD)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-168">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="ff4f8-169">病毒</span><span class="sxs-lookup"><span data-stu-id="ff4f8-169">threats</span></span>|<span data-ttu-id="ff4f8-170">String collection</span><span class="sxs-lookup"><span data-stu-id="ff4f8-170">String collection</span></span>|<span data-ttu-id="ff4f8-171">控制缓解的威胁列表 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、</span><span class="sxs-lookup"><span data-stu-id="ff4f8-171">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="ff4f8-172">elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-172">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="ff4f8-173">单层</span><span class="sxs-lookup"><span data-stu-id="ff4f8-173">tier</span></span>|<span data-ttu-id="ff4f8-174">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-174">String</span></span>|<span data-ttu-id="ff4f8-175">控制层 (Core, 纵深防御, 高级。)</span><span class="sxs-lookup"><span data-stu-id="ff4f8-175">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="ff4f8-176">userImpact</span><span class="sxs-lookup"><span data-stu-id="ff4f8-176">userImpact</span></span>|<span data-ttu-id="ff4f8-177">String</span><span class="sxs-lookup"><span data-stu-id="ff4f8-177">String</span></span>|<span data-ttu-id="ff4f8-178">实施控制的用户影响 (低、中等、高)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-178">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="ff4f8-179">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="ff4f8-179">complianceInformation</span></span>|<span data-ttu-id="ff4f8-180">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff4f8-180">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="ff4f8-181">与安全得分控制相关联的合规性信息的集合</span><span class="sxs-lookup"><span data-stu-id="ff4f8-181">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="ff4f8-182">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="ff4f8-182">controlStateUpdates</span></span>|<span data-ttu-id="ff4f8-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff4f8-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="ff4f8-184">用于指示租户已标记控件的位置的标志 (忽略、thirdParty、已审阅) (支持[更新](../api/securescorecontrolprofile-update.md))。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-184">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="ff4f8-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="ff4f8-185">vendorInformation</span></span>|[<span data-ttu-id="ff4f8-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="ff4f8-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="ff4f8-187">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息的复杂类型 (例如, 供应商 = Microsoft; provider = SecureScore)。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-187">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="ff4f8-188">必需。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-188">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4f8-189">关系</span><span class="sxs-lookup"><span data-stu-id="ff4f8-189">Relationships</span></span>

<span data-ttu-id="ff4f8-190">无。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-190">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff4f8-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff4f8-191">JSON representation</span></span>

<span data-ttu-id="ff4f8-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff4f8-192">The following is a JSON representation of the resource.</span></span>

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
