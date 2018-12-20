---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
ms.openlocfilehash: 3e7dc463d7521e1980b41034ae4121ab610dd8f5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380581"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="238d0-104">secureScoreControlProfiles 资源类型</span><span class="sxs-lookup"><span data-stu-id="238d0-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="238d0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="238d0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="238d0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="238d0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="238d0-107">表示每个控件数据的租户的安全分数。</span><span class="sxs-lookup"><span data-stu-id="238d0-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="238d0-108">默认情况下，它返回租户的所有控件并且可以显式拉单个控件。</span><span class="sxs-lookup"><span data-stu-id="238d0-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="238d0-109">方法</span><span class="sxs-lookup"><span data-stu-id="238d0-109">Methods</span></span>

| <span data-ttu-id="238d0-110">方法</span><span class="sxs-lookup"><span data-stu-id="238d0-110">Method</span></span>   | <span data-ttu-id="238d0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="238d0-111">Return Type</span></span>|<span data-ttu-id="238d0-112">说明</span><span class="sxs-lookup"><span data-stu-id="238d0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="238d0-113">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="238d0-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="238d0-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="238d0-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="238d0-115">读取属性和 secureScoreControlProfiles 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="238d0-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="238d0-116">属性</span><span class="sxs-lookup"><span data-stu-id="238d0-116">Properties</span></span>

|<span data-ttu-id="238d0-117">名称</span><span class="sxs-lookup"><span data-stu-id="238d0-117">Name</span></span> |<span data-ttu-id="238d0-118">类型</span><span class="sxs-lookup"><span data-stu-id="238d0-118">Type</span></span> |<span data-ttu-id="238d0-119">说明</span><span class="sxs-lookup"><span data-stu-id="238d0-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="238d0-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="238d0-120">azureTenantId</span></span>   |   <span data-ttu-id="238d0-121">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-121">String</span></span>  |   <span data-ttu-id="238d0-122">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="238d0-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="238d0-123">控件名称</span><span class="sxs-lookup"><span data-stu-id="238d0-123">controlName</span></span> |   <span data-ttu-id="238d0-124">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-124">String</span></span>  |   <span data-ttu-id="238d0-125">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="238d0-125">Name of the control.</span></span> |
|   <span data-ttu-id="238d0-126">title</span><span class="sxs-lookup"><span data-stu-id="238d0-126">title</span></span>   |   <span data-ttu-id="238d0-127">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-127">String</span></span>  |   <span data-ttu-id="238d0-128">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="238d0-128">Title of the control.</span></span>   |
| <span data-ttu-id="238d0-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="238d0-129">complianceInformation</span></span> | <span data-ttu-id="238d0-130">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="238d0-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="238d0-131">与关联的合规性信息的集合安全分数控件</span><span class="sxs-lookup"><span data-stu-id="238d0-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="238d0-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="238d0-132">controlCategory</span></span> |   <span data-ttu-id="238d0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-133">String</span></span>  |   <span data-ttu-id="238d0-134">控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="238d0-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="238d0-135">actionType</span><span class="sxs-lookup"><span data-stu-id="238d0-135">actionType</span></span>  |   <span data-ttu-id="238d0-136">String</span><span class="sxs-lookup"><span data-stu-id="238d0-136">String</span></span>  |   <span data-ttu-id="238d0-137">控制操作类型 （Config、 审阅、 行为）。</span><span class="sxs-lookup"><span data-stu-id="238d0-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="238d0-138">service</span><span class="sxs-lookup"><span data-stu-id="238d0-138">service</span></span> |   <span data-ttu-id="238d0-139">String</span><span class="sxs-lookup"><span data-stu-id="238d0-139">String</span></span>  |   <span data-ttu-id="238d0-140">拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。</span><span class="sxs-lookup"><span data-stu-id="238d0-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="238d0-141">maxScore</span><span class="sxs-lookup"><span data-stu-id="238d0-141">maxScore</span></span> |  <span data-ttu-id="238d0-142">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-142">String</span></span>  |   <span data-ttu-id="238d0-143">当前在指定日期上获得最大分数。</span><span class="sxs-lookup"><span data-stu-id="238d0-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="238d0-144">层</span><span class="sxs-lookup"><span data-stu-id="238d0-144">tier</span></span> |  <span data-ttu-id="238d0-145">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-145">String</span></span>  |   <span data-ttu-id="238d0-146">控件层 (核心、 防护深入，高级。)</span><span class="sxs-lookup"><span data-stu-id="238d0-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="238d0-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="238d0-147">userImpact</span></span> |    <span data-ttu-id="238d0-148">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-148">String</span></span>  | <span data-ttu-id="238d0-149">用户影响实现控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="238d0-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="238d0-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="238d0-150">implementationCost</span></span> |    <span data-ttu-id="238d0-151">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-151">String</span></span>  |   <span data-ttu-id="238d0-152">资源成本 implemmentating 控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="238d0-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="238d0-153">排名</span><span class="sxs-lookup"><span data-stu-id="238d0-153">rank</span></span> |  <span data-ttu-id="238d0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="238d0-154">Int32</span></span>   |   <span data-ttu-id="238d0-155">Microsoft 的堆栈控件的排名。</span><span class="sxs-lookup"><span data-stu-id="238d0-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="238d0-156">威胁</span><span class="sxs-lookup"><span data-stu-id="238d0-156">threats</span></span> |   <span data-ttu-id="238d0-157">字符串集合</span><span class="sxs-lookup"><span data-stu-id="238d0-157">String Collection</span></span>   |   <span data-ttu-id="238d0-158">控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。</span><span class="sxs-lookup"><span data-stu-id="238d0-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="238d0-159">弃用</span><span class="sxs-lookup"><span data-stu-id="238d0-159">deprecated</span></span> |    <span data-ttu-id="238d0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="238d0-160">Boolean</span></span> |   <span data-ttu-id="238d0-161">用于指示控件进行折旧计算的标志。</span><span class="sxs-lookup"><span data-stu-id="238d0-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="238d0-162">修正</span><span class="sxs-lookup"><span data-stu-id="238d0-162">remediation</span></span> |   <span data-ttu-id="238d0-163">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-163">String</span></span>  |   <span data-ttu-id="238d0-164">内容控件的说明将帮助纠正。</span><span class="sxs-lookup"><span data-stu-id="238d0-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="238d0-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="238d0-165">remediationImpact</span></span> | <span data-ttu-id="238d0-166">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-166">String</span></span>  |   <span data-ttu-id="238d0-167">对用户的修正影响的说明。</span><span class="sxs-lookup"><span data-stu-id="238d0-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="238d0-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="238d0-168">actionUrl</span></span> | <span data-ttu-id="238d0-169">字符串</span><span class="sxs-lookup"><span data-stu-id="238d0-169">String</span></span>  |   <span data-ttu-id="238d0-170">该控件可进行的 URL。</span><span class="sxs-lookup"><span data-stu-id="238d0-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="238d0-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="238d0-171">controlStateUpdates</span></span> |   <span data-ttu-id="238d0-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="238d0-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="238d0-173">标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="238d0-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="238d0-174">Relationships</span><span class="sxs-lookup"><span data-stu-id="238d0-174">Relationships</span></span>

<span data-ttu-id="238d0-175">无。</span><span class="sxs-lookup"><span data-stu-id="238d0-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="238d0-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="238d0-176">JSON representation</span></span>

<span data-ttu-id="238d0-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="238d0-177">The following is a JSON representation of the resource.</span></span>

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
