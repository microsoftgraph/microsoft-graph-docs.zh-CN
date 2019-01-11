---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
localization_priority: Normal
ms.openlocfilehash: 866b2086ff5160744f848292cedf30c3cedf6daa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866218"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="7bd32-104">secureScoreControlProfiles 资源类型</span><span class="sxs-lookup"><span data-stu-id="7bd32-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="7bd32-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7bd32-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bd32-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7bd32-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7bd32-107">表示每个控件数据的租户的安全分数。</span><span class="sxs-lookup"><span data-stu-id="7bd32-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="7bd32-108">默认情况下，它返回租户的所有控件并且可以显式拉单个控件。</span><span class="sxs-lookup"><span data-stu-id="7bd32-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="7bd32-109">方法</span><span class="sxs-lookup"><span data-stu-id="7bd32-109">Methods</span></span>

| <span data-ttu-id="7bd32-110">方法</span><span class="sxs-lookup"><span data-stu-id="7bd32-110">Method</span></span>   | <span data-ttu-id="7bd32-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7bd32-111">Return Type</span></span>|<span data-ttu-id="7bd32-112">说明</span><span class="sxs-lookup"><span data-stu-id="7bd32-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7bd32-113">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="7bd32-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="7bd32-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="7bd32-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="7bd32-115">读取属性和 secureScoreControlProfiles 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="7bd32-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="7bd32-116">属性</span><span class="sxs-lookup"><span data-stu-id="7bd32-116">Properties</span></span>

|<span data-ttu-id="7bd32-117">名称</span><span class="sxs-lookup"><span data-stu-id="7bd32-117">Name</span></span> |<span data-ttu-id="7bd32-118">类型</span><span class="sxs-lookup"><span data-stu-id="7bd32-118">Type</span></span> |<span data-ttu-id="7bd32-119">Description</span><span class="sxs-lookup"><span data-stu-id="7bd32-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="7bd32-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="7bd32-120">azureTenantId</span></span>   |   <span data-ttu-id="7bd32-121">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-121">String</span></span>  |   <span data-ttu-id="7bd32-122">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="7bd32-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="7bd32-123">控件名称</span><span class="sxs-lookup"><span data-stu-id="7bd32-123">controlName</span></span> |   <span data-ttu-id="7bd32-124">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-124">String</span></span>  |   <span data-ttu-id="7bd32-125">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="7bd32-125">Name of the control.</span></span> |
|   <span data-ttu-id="7bd32-126">title</span><span class="sxs-lookup"><span data-stu-id="7bd32-126">title</span></span>   |   <span data-ttu-id="7bd32-127">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-127">String</span></span>  |   <span data-ttu-id="7bd32-128">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="7bd32-128">Title of the control.</span></span>   |
| <span data-ttu-id="7bd32-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="7bd32-129">complianceInformation</span></span> | <span data-ttu-id="7bd32-130">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bd32-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="7bd32-131">与关联的合规性信息的集合安全分数控件</span><span class="sxs-lookup"><span data-stu-id="7bd32-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="7bd32-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="7bd32-132">controlCategory</span></span> |   <span data-ttu-id="7bd32-133">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-133">String</span></span>  |   <span data-ttu-id="7bd32-134">控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="7bd32-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="7bd32-135">actionType</span><span class="sxs-lookup"><span data-stu-id="7bd32-135">actionType</span></span>  |   <span data-ttu-id="7bd32-136">String</span><span class="sxs-lookup"><span data-stu-id="7bd32-136">String</span></span>  |   <span data-ttu-id="7bd32-137">控制操作类型 （Config、 审阅、 行为）。</span><span class="sxs-lookup"><span data-stu-id="7bd32-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="7bd32-138">service</span><span class="sxs-lookup"><span data-stu-id="7bd32-138">service</span></span> |   <span data-ttu-id="7bd32-139">String</span><span class="sxs-lookup"><span data-stu-id="7bd32-139">String</span></span>  |   <span data-ttu-id="7bd32-140">拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。</span><span class="sxs-lookup"><span data-stu-id="7bd32-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="7bd32-141">maxScore</span><span class="sxs-lookup"><span data-stu-id="7bd32-141">maxScore</span></span> |  <span data-ttu-id="7bd32-142">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-142">String</span></span>  |   <span data-ttu-id="7bd32-143">当前在指定日期上获得最大分数。</span><span class="sxs-lookup"><span data-stu-id="7bd32-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="7bd32-144">层</span><span class="sxs-lookup"><span data-stu-id="7bd32-144">tier</span></span> |  <span data-ttu-id="7bd32-145">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-145">String</span></span>  |   <span data-ttu-id="7bd32-146">控件层 (核心、 防护深入，高级。)</span><span class="sxs-lookup"><span data-stu-id="7bd32-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="7bd32-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="7bd32-147">userImpact</span></span> |    <span data-ttu-id="7bd32-148">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-148">String</span></span>  | <span data-ttu-id="7bd32-149">用户影响实现控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="7bd32-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="7bd32-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="7bd32-150">implementationCost</span></span> |    <span data-ttu-id="7bd32-151">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-151">String</span></span>  |   <span data-ttu-id="7bd32-152">资源成本 implemmentating 控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="7bd32-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="7bd32-153">排名</span><span class="sxs-lookup"><span data-stu-id="7bd32-153">rank</span></span> |  <span data-ttu-id="7bd32-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd32-154">Int32</span></span>   |   <span data-ttu-id="7bd32-155">Microsoft 的堆栈控件的排名。</span><span class="sxs-lookup"><span data-stu-id="7bd32-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="7bd32-156">威胁</span><span class="sxs-lookup"><span data-stu-id="7bd32-156">threats</span></span> |   <span data-ttu-id="7bd32-157">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7bd32-157">String Collection</span></span>   |   <span data-ttu-id="7bd32-158">控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。</span><span class="sxs-lookup"><span data-stu-id="7bd32-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="7bd32-159">弃用</span><span class="sxs-lookup"><span data-stu-id="7bd32-159">deprecated</span></span> |    <span data-ttu-id="7bd32-160">布尔</span><span class="sxs-lookup"><span data-stu-id="7bd32-160">Boolean</span></span> |   <span data-ttu-id="7bd32-161">用于指示控件进行折旧计算的标志。</span><span class="sxs-lookup"><span data-stu-id="7bd32-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="7bd32-162">修正</span><span class="sxs-lookup"><span data-stu-id="7bd32-162">remediation</span></span> |   <span data-ttu-id="7bd32-163">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-163">String</span></span>  |   <span data-ttu-id="7bd32-164">内容控件的说明将帮助纠正。</span><span class="sxs-lookup"><span data-stu-id="7bd32-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="7bd32-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="7bd32-165">remediationImpact</span></span> | <span data-ttu-id="7bd32-166">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-166">String</span></span>  |   <span data-ttu-id="7bd32-167">对用户的修正影响的说明。</span><span class="sxs-lookup"><span data-stu-id="7bd32-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="7bd32-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="7bd32-168">actionUrl</span></span> | <span data-ttu-id="7bd32-169">字符串</span><span class="sxs-lookup"><span data-stu-id="7bd32-169">String</span></span>  |   <span data-ttu-id="7bd32-170">该控件可进行的 URL。</span><span class="sxs-lookup"><span data-stu-id="7bd32-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="7bd32-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="7bd32-171">controlStateUpdates</span></span> |   <span data-ttu-id="7bd32-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bd32-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="7bd32-173">标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="7bd32-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="7bd32-174">Relationships</span><span class="sxs-lookup"><span data-stu-id="7bd32-174">Relationships</span></span>

<span data-ttu-id="7bd32-175">无。</span><span class="sxs-lookup"><span data-stu-id="7bd32-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bd32-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7bd32-176">JSON representation</span></span>

<span data-ttu-id="7bd32-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bd32-177">The following is a JSON representation of the resource.</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
