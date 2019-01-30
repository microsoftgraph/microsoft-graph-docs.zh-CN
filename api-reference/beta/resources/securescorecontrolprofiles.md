---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641608"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="6c465-104">secureScoreControlProfiles 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c465-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c465-105">表示每个控件数据的租户的安全分数。</span><span class="sxs-lookup"><span data-stu-id="6c465-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="6c465-106">默认情况下，它返回租户的所有控件并且可以显式拉单个控件。</span><span class="sxs-lookup"><span data-stu-id="6c465-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="6c465-107">方法</span><span class="sxs-lookup"><span data-stu-id="6c465-107">Methods</span></span>

| <span data-ttu-id="6c465-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c465-108">Method</span></span>   | <span data-ttu-id="6c465-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c465-109">Return Type</span></span>|<span data-ttu-id="6c465-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c465-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c465-111">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6c465-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="6c465-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6c465-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="6c465-113">读取属性和 secureScoreControlProfiles 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="6c465-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6c465-114">属性</span><span class="sxs-lookup"><span data-stu-id="6c465-114">Properties</span></span>

|<span data-ttu-id="6c465-115">名称</span><span class="sxs-lookup"><span data-stu-id="6c465-115">Name</span></span> |<span data-ttu-id="6c465-116">类型</span><span class="sxs-lookup"><span data-stu-id="6c465-116">Type</span></span> |<span data-ttu-id="6c465-117">说明</span><span class="sxs-lookup"><span data-stu-id="6c465-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6c465-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="6c465-118">azureTenantId</span></span>   |   <span data-ttu-id="6c465-119">String</span><span class="sxs-lookup"><span data-stu-id="6c465-119">String</span></span>  |   <span data-ttu-id="6c465-120">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="6c465-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="6c465-121">控件名称</span><span class="sxs-lookup"><span data-stu-id="6c465-121">controlName</span></span> |   <span data-ttu-id="6c465-122">String</span><span class="sxs-lookup"><span data-stu-id="6c465-122">String</span></span>  |   <span data-ttu-id="6c465-123">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="6c465-123">Name of the control.</span></span> |
|   <span data-ttu-id="6c465-124">title</span><span class="sxs-lookup"><span data-stu-id="6c465-124">title</span></span>   |   <span data-ttu-id="6c465-125">String</span><span class="sxs-lookup"><span data-stu-id="6c465-125">String</span></span>  |   <span data-ttu-id="6c465-126">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="6c465-126">Title of the control.</span></span>   |
| <span data-ttu-id="6c465-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="6c465-127">complianceInformation</span></span> | <span data-ttu-id="6c465-128">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c465-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="6c465-129">与关联的合规性信息的集合安全分数控件</span><span class="sxs-lookup"><span data-stu-id="6c465-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="6c465-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6c465-130">controlCategory</span></span> |   <span data-ttu-id="6c465-131">String</span><span class="sxs-lookup"><span data-stu-id="6c465-131">String</span></span>  |   <span data-ttu-id="6c465-132">控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="6c465-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="6c465-133">actionType</span><span class="sxs-lookup"><span data-stu-id="6c465-133">actionType</span></span>  |   <span data-ttu-id="6c465-134">String</span><span class="sxs-lookup"><span data-stu-id="6c465-134">String</span></span>  |   <span data-ttu-id="6c465-135">控制操作类型 （Config、 审阅、 行为）。</span><span class="sxs-lookup"><span data-stu-id="6c465-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="6c465-136">service</span><span class="sxs-lookup"><span data-stu-id="6c465-136">service</span></span> |   <span data-ttu-id="6c465-137">String</span><span class="sxs-lookup"><span data-stu-id="6c465-137">String</span></span>  |   <span data-ttu-id="6c465-138">拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。</span><span class="sxs-lookup"><span data-stu-id="6c465-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="6c465-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="6c465-139">maxScore</span></span> |  <span data-ttu-id="6c465-140">String</span><span class="sxs-lookup"><span data-stu-id="6c465-140">String</span></span>  |   <span data-ttu-id="6c465-141">当前在指定日期上获得最大分数。</span><span class="sxs-lookup"><span data-stu-id="6c465-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="6c465-142">层</span><span class="sxs-lookup"><span data-stu-id="6c465-142">tier</span></span> |  <span data-ttu-id="6c465-143">String</span><span class="sxs-lookup"><span data-stu-id="6c465-143">String</span></span>  |   <span data-ttu-id="6c465-144">控件层 (核心、 防护深入，高级。)</span><span class="sxs-lookup"><span data-stu-id="6c465-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="6c465-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="6c465-145">userImpact</span></span> |    <span data-ttu-id="6c465-146">String</span><span class="sxs-lookup"><span data-stu-id="6c465-146">String</span></span>  | <span data-ttu-id="6c465-147">用户影响实现控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="6c465-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="6c465-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="6c465-148">implementationCost</span></span> |    <span data-ttu-id="6c465-149">String</span><span class="sxs-lookup"><span data-stu-id="6c465-149">String</span></span>  |   <span data-ttu-id="6c465-150">资源成本 implemmentating 控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="6c465-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="6c465-151">排名</span><span class="sxs-lookup"><span data-stu-id="6c465-151">rank</span></span> |  <span data-ttu-id="6c465-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6c465-152">Int32</span></span>   |   <span data-ttu-id="6c465-153">Microsoft 的堆栈控件的排名。</span><span class="sxs-lookup"><span data-stu-id="6c465-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="6c465-154">威胁</span><span class="sxs-lookup"><span data-stu-id="6c465-154">threats</span></span> |   <span data-ttu-id="6c465-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="6c465-155">String Collection</span></span>   |   <span data-ttu-id="6c465-156">控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。</span><span class="sxs-lookup"><span data-stu-id="6c465-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="6c465-157">弃用</span><span class="sxs-lookup"><span data-stu-id="6c465-157">deprecated</span></span> |    <span data-ttu-id="6c465-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="6c465-158">Boolean</span></span> |   <span data-ttu-id="6c465-159">用于指示控件进行折旧计算的标志。</span><span class="sxs-lookup"><span data-stu-id="6c465-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="6c465-160">修正</span><span class="sxs-lookup"><span data-stu-id="6c465-160">remediation</span></span> |   <span data-ttu-id="6c465-161">String</span><span class="sxs-lookup"><span data-stu-id="6c465-161">String</span></span>  |   <span data-ttu-id="6c465-162">内容控件的说明将帮助纠正。</span><span class="sxs-lookup"><span data-stu-id="6c465-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="6c465-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="6c465-163">remediationImpact</span></span> | <span data-ttu-id="6c465-164">String</span><span class="sxs-lookup"><span data-stu-id="6c465-164">String</span></span>  |   <span data-ttu-id="6c465-165">对用户的修正影响的说明。</span><span class="sxs-lookup"><span data-stu-id="6c465-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="6c465-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="6c465-166">actionUrl</span></span> | <span data-ttu-id="6c465-167">String</span><span class="sxs-lookup"><span data-stu-id="6c465-167">String</span></span>  |   <span data-ttu-id="6c465-168">该控件可进行的 URL。</span><span class="sxs-lookup"><span data-stu-id="6c465-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="6c465-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="6c465-169">controlStateUpdates</span></span> |   <span data-ttu-id="6c465-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c465-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="6c465-171">标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="6c465-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c465-172">关系</span><span class="sxs-lookup"><span data-stu-id="6c465-172">Relationships</span></span>

<span data-ttu-id="6c465-173">无。</span><span class="sxs-lookup"><span data-stu-id="6c465-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c465-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c465-174">JSON representation</span></span>

<span data-ttu-id="6c465-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c465-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
