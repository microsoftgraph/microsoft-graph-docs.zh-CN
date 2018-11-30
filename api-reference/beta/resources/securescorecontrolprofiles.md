---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046876"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="6f63f-104">secureScoreControlProfiles 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f63f-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="6f63f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f63f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f63f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f63f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f63f-107">表示每个控件数据的租户的安全分数。</span><span class="sxs-lookup"><span data-stu-id="6f63f-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="6f63f-108">默认情况下，它返回租户的所有控件并且可以显式拉单个控件。</span><span class="sxs-lookup"><span data-stu-id="6f63f-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="6f63f-109">方法</span><span class="sxs-lookup"><span data-stu-id="6f63f-109">Methods</span></span>

| <span data-ttu-id="6f63f-110">方法</span><span class="sxs-lookup"><span data-stu-id="6f63f-110">Method</span></span>   | <span data-ttu-id="6f63f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6f63f-111">Return Type</span></span>|<span data-ttu-id="6f63f-112">说明</span><span class="sxs-lookup"><span data-stu-id="6f63f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f63f-113">列表 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6f63f-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="6f63f-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6f63f-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="6f63f-115">读取属性和 secureScoreControlProfiles 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="6f63f-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6f63f-116">属性</span><span class="sxs-lookup"><span data-stu-id="6f63f-116">Properties</span></span>

|<span data-ttu-id="6f63f-117">名称</span><span class="sxs-lookup"><span data-stu-id="6f63f-117">Name</span></span> |<span data-ttu-id="6f63f-118">类型</span><span class="sxs-lookup"><span data-stu-id="6f63f-118">Type</span></span> |<span data-ttu-id="6f63f-119">说明</span><span class="sxs-lookup"><span data-stu-id="6f63f-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6f63f-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="6f63f-120">azureTenantId</span></span>   |   <span data-ttu-id="6f63f-121">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-121">String</span></span>  |   <span data-ttu-id="6f63f-122">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="6f63f-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="6f63f-123">控件名称</span><span class="sxs-lookup"><span data-stu-id="6f63f-123">controlName</span></span> |   <span data-ttu-id="6f63f-124">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-124">String</span></span>  |   <span data-ttu-id="6f63f-125">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="6f63f-125">Name of the control.</span></span> |
|   <span data-ttu-id="6f63f-126">title</span><span class="sxs-lookup"><span data-stu-id="6f63f-126">title</span></span>   |   <span data-ttu-id="6f63f-127">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-127">String</span></span>  |   <span data-ttu-id="6f63f-128">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="6f63f-128">Title of the control.</span></span>   |
|   <span data-ttu-id="6f63f-129">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6f63f-129">controlCategory</span></span> |   <span data-ttu-id="6f63f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-130">String</span></span>  |   <span data-ttu-id="6f63f-131">控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="6f63f-131">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="6f63f-132">actionType</span><span class="sxs-lookup"><span data-stu-id="6f63f-132">actionType</span></span>  |   <span data-ttu-id="6f63f-133">String</span><span class="sxs-lookup"><span data-stu-id="6f63f-133">String</span></span>  |   <span data-ttu-id="6f63f-134">控制操作类型 （Config、 审阅、 行为）。</span><span class="sxs-lookup"><span data-stu-id="6f63f-134">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="6f63f-135">service</span><span class="sxs-lookup"><span data-stu-id="6f63f-135">service</span></span> |   <span data-ttu-id="6f63f-136">String</span><span class="sxs-lookup"><span data-stu-id="6f63f-136">String</span></span>  |   <span data-ttu-id="6f63f-137">拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。</span><span class="sxs-lookup"><span data-stu-id="6f63f-137">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="6f63f-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="6f63f-138">maxScore</span></span> |  <span data-ttu-id="6f63f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-139">String</span></span>  |   <span data-ttu-id="6f63f-140">当前在指定日期上获得最大分数。</span><span class="sxs-lookup"><span data-stu-id="6f63f-140">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="6f63f-141">层</span><span class="sxs-lookup"><span data-stu-id="6f63f-141">tier</span></span> |  <span data-ttu-id="6f63f-142">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-142">String</span></span>  |   <span data-ttu-id="6f63f-143">控件层 (核心、 防护深入，高级。)</span><span class="sxs-lookup"><span data-stu-id="6f63f-143">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="6f63f-144">userImpact</span><span class="sxs-lookup"><span data-stu-id="6f63f-144">userImpact</span></span> |    <span data-ttu-id="6f63f-145">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-145">String</span></span>  | <span data-ttu-id="6f63f-146">用户影响实现控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="6f63f-146">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="6f63f-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="6f63f-147">implementationCost</span></span> |    <span data-ttu-id="6f63f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-148">String</span></span>  |   <span data-ttu-id="6f63f-149">资源成本 implemmentating 控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="6f63f-149">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="6f63f-150">排名</span><span class="sxs-lookup"><span data-stu-id="6f63f-150">rank</span></span> |  <span data-ttu-id="6f63f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6f63f-151">Int32</span></span>   |   <span data-ttu-id="6f63f-152">Microsoft 的堆栈控件的排名。</span><span class="sxs-lookup"><span data-stu-id="6f63f-152">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="6f63f-153">威胁</span><span class="sxs-lookup"><span data-stu-id="6f63f-153">threats</span></span> |   <span data-ttu-id="6f63f-154">字符串集合</span><span class="sxs-lookup"><span data-stu-id="6f63f-154">String Collection</span></span>   |   <span data-ttu-id="6f63f-155">控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。</span><span class="sxs-lookup"><span data-stu-id="6f63f-155">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="6f63f-156">弃用</span><span class="sxs-lookup"><span data-stu-id="6f63f-156">deprecated</span></span> |    <span data-ttu-id="6f63f-157">布尔</span><span class="sxs-lookup"><span data-stu-id="6f63f-157">Boolean</span></span> |   <span data-ttu-id="6f63f-158">用于指示控件进行折旧计算的标志。</span><span class="sxs-lookup"><span data-stu-id="6f63f-158">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="6f63f-159">修正</span><span class="sxs-lookup"><span data-stu-id="6f63f-159">remediation</span></span> |   <span data-ttu-id="6f63f-160">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-160">String</span></span>  |   <span data-ttu-id="6f63f-161">内容控件的说明将帮助纠正。</span><span class="sxs-lookup"><span data-stu-id="6f63f-161">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="6f63f-162">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="6f63f-162">remediationImpact</span></span> | <span data-ttu-id="6f63f-163">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-163">String</span></span>  |   <span data-ttu-id="6f63f-164">对用户的修正影响的说明。</span><span class="sxs-lookup"><span data-stu-id="6f63f-164">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="6f63f-165">actionUrl</span><span class="sxs-lookup"><span data-stu-id="6f63f-165">actionUrl</span></span> | <span data-ttu-id="6f63f-166">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-166">String</span></span>  |   <span data-ttu-id="6f63f-167">该控件可进行的 URL。</span><span class="sxs-lookup"><span data-stu-id="6f63f-167">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="6f63f-168">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="6f63f-168">controlStateUpdates</span></span> |   <span data-ttu-id="6f63f-169">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-169">String</span></span>  |   <span data-ttu-id="6f63f-170">标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="6f63f-170">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="6f63f-171">tenantNote</span><span class="sxs-lookup"><span data-stu-id="6f63f-171">tenantNote</span></span> |    <span data-ttu-id="6f63f-172">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-172">String</span></span>  |   <span data-ttu-id="6f63f-173">租户可以设置每个控件注释 （支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="6f63f-173">Tenant can set per control comments (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="6f63f-174">assignedTo</span><span class="sxs-lookup"><span data-stu-id="6f63f-174">assignedTo</span></span> |    <span data-ttu-id="6f63f-175">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-175">String</span></span>  |   <span data-ttu-id="6f63f-176">租户可以为控件分配 （支持[更新](../api/securescorecontrolprofiles-update.md)） 个人。</span><span class="sxs-lookup"><span data-stu-id="6f63f-176">Tenant can assign the control to a individual (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="6f63f-177">updatedBy</span><span class="sxs-lookup"><span data-stu-id="6f63f-177">updatedBy</span></span> | <span data-ttu-id="6f63f-178">字符串</span><span class="sxs-lookup"><span data-stu-id="6f63f-178">String</span></span>  |   <span data-ttu-id="6f63f-179">修订的作者到控件的状态的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="6f63f-179">User principal name of who made changes to a control's state.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6f63f-180">Relationships</span><span class="sxs-lookup"><span data-stu-id="6f63f-180">Relationships</span></span>

<span data-ttu-id="6f63f-181">无。</span><span class="sxs-lookup"><span data-stu-id="6f63f-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f63f-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f63f-182">JSON representation</span></span>

<span data-ttu-id="6f63f-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f63f-183">The following is a JSON representation of the resource.</span></span>

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
