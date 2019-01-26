---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576057"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="714a7-104">secureScoreControlProfiles 资源类型</span><span class="sxs-lookup"><span data-stu-id="714a7-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="714a7-105">表示每个控件数据的租户的安全分数。</span><span class="sxs-lookup"><span data-stu-id="714a7-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="714a7-106">默认情况下，它返回租户的所有控件并且可以显式拉单个控件。</span><span class="sxs-lookup"><span data-stu-id="714a7-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="714a7-107">方法</span><span class="sxs-lookup"><span data-stu-id="714a7-107">Methods</span></span>

| <span data-ttu-id="714a7-108">方法</span><span class="sxs-lookup"><span data-stu-id="714a7-108">Method</span></span>   | <span data-ttu-id="714a7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="714a7-109">Return Type</span></span>|<span data-ttu-id="714a7-110">说明</span><span class="sxs-lookup"><span data-stu-id="714a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="714a7-111">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="714a7-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="714a7-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="714a7-112">secureScoreControlProfile</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="714a7-113">读取属性和 secureScoreControlProfiles 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="714a7-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="714a7-114">属性</span><span class="sxs-lookup"><span data-stu-id="714a7-114">Properties</span></span>

|<span data-ttu-id="714a7-115">名称</span><span class="sxs-lookup"><span data-stu-id="714a7-115">Name</span></span> |<span data-ttu-id="714a7-116">类型</span><span class="sxs-lookup"><span data-stu-id="714a7-116">Type</span></span> |<span data-ttu-id="714a7-117">说明</span><span class="sxs-lookup"><span data-stu-id="714a7-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="714a7-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="714a7-118">azureTenantId</span></span>   |   <span data-ttu-id="714a7-119">String</span><span class="sxs-lookup"><span data-stu-id="714a7-119">String</span></span>  |   <span data-ttu-id="714a7-120">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="714a7-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="714a7-121">控件名称</span><span class="sxs-lookup"><span data-stu-id="714a7-121">controlName</span></span> |   <span data-ttu-id="714a7-122">String</span><span class="sxs-lookup"><span data-stu-id="714a7-122">String</span></span>  |   <span data-ttu-id="714a7-123">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="714a7-123">Name of the control.</span></span> |
|   <span data-ttu-id="714a7-124">title</span><span class="sxs-lookup"><span data-stu-id="714a7-124">title</span></span>   |   <span data-ttu-id="714a7-125">String</span><span class="sxs-lookup"><span data-stu-id="714a7-125">String</span></span>  |   <span data-ttu-id="714a7-126">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="714a7-126">Title of the control.</span></span>   |
|   <span data-ttu-id="714a7-127">controlCategory</span><span class="sxs-lookup"><span data-stu-id="714a7-127">controlCategory</span></span> |   <span data-ttu-id="714a7-128">String</span><span class="sxs-lookup"><span data-stu-id="714a7-128">String</span></span>  |   <span data-ttu-id="714a7-129">控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="714a7-129">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="714a7-130">actionType</span><span class="sxs-lookup"><span data-stu-id="714a7-130">actionType</span></span>  |   <span data-ttu-id="714a7-131">String</span><span class="sxs-lookup"><span data-stu-id="714a7-131">String</span></span>  |   <span data-ttu-id="714a7-132">控制操作类型 （Config、 审阅、 行为）。</span><span class="sxs-lookup"><span data-stu-id="714a7-132">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="714a7-133">service</span><span class="sxs-lookup"><span data-stu-id="714a7-133">service</span></span> |   <span data-ttu-id="714a7-134">String</span><span class="sxs-lookup"><span data-stu-id="714a7-134">String</span></span>  |   <span data-ttu-id="714a7-135">拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。</span><span class="sxs-lookup"><span data-stu-id="714a7-135">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="714a7-136">maxScore</span><span class="sxs-lookup"><span data-stu-id="714a7-136">maxScore</span></span> |  <span data-ttu-id="714a7-137">双精度</span><span class="sxs-lookup"><span data-stu-id="714a7-137">Double</span></span>  |   <span data-ttu-id="714a7-138">当前在指定日期上获得最大分数。</span><span class="sxs-lookup"><span data-stu-id="714a7-138">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="714a7-139">层</span><span class="sxs-lookup"><span data-stu-id="714a7-139">tier</span></span> |  <span data-ttu-id="714a7-140">String</span><span class="sxs-lookup"><span data-stu-id="714a7-140">String</span></span>  |   <span data-ttu-id="714a7-141">控件层 (核心、 防护深入，高级。)</span><span class="sxs-lookup"><span data-stu-id="714a7-141">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="714a7-142">userImpact</span><span class="sxs-lookup"><span data-stu-id="714a7-142">userImpact</span></span> |    <span data-ttu-id="714a7-143">String</span><span class="sxs-lookup"><span data-stu-id="714a7-143">String</span></span>  | <span data-ttu-id="714a7-144">用户影响实现控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="714a7-144">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="714a7-145">implementationCost</span><span class="sxs-lookup"><span data-stu-id="714a7-145">implementationCost</span></span> |    <span data-ttu-id="714a7-146">String</span><span class="sxs-lookup"><span data-stu-id="714a7-146">String</span></span>  |   <span data-ttu-id="714a7-147">资源成本 implemmentating 控件 （低、 中等，高）。</span><span class="sxs-lookup"><span data-stu-id="714a7-147">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="714a7-148">排名</span><span class="sxs-lookup"><span data-stu-id="714a7-148">rank</span></span> |  <span data-ttu-id="714a7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="714a7-149">Int32</span></span>   |   <span data-ttu-id="714a7-150">Microsoft 的堆栈控件的排名。</span><span class="sxs-lookup"><span data-stu-id="714a7-150">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="714a7-151">威胁</span><span class="sxs-lookup"><span data-stu-id="714a7-151">threats</span></span> |   <span data-ttu-id="714a7-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="714a7-152">String Collection</span></span>   |   <span data-ttu-id="714a7-153">控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。</span><span class="sxs-lookup"><span data-stu-id="714a7-153">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="714a7-154">弃用</span><span class="sxs-lookup"><span data-stu-id="714a7-154">deprecated</span></span> |    <span data-ttu-id="714a7-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="714a7-155">Boolean</span></span> |   <span data-ttu-id="714a7-156">用于指示控件进行折旧计算的标志。</span><span class="sxs-lookup"><span data-stu-id="714a7-156">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="714a7-157">修正</span><span class="sxs-lookup"><span data-stu-id="714a7-157">remediation</span></span> |   <span data-ttu-id="714a7-158">String</span><span class="sxs-lookup"><span data-stu-id="714a7-158">String</span></span>  |   <span data-ttu-id="714a7-159">内容控件的说明将帮助纠正。</span><span class="sxs-lookup"><span data-stu-id="714a7-159">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="714a7-160">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="714a7-160">remediationImpact</span></span> | <span data-ttu-id="714a7-161">String</span><span class="sxs-lookup"><span data-stu-id="714a7-161">String</span></span>  |   <span data-ttu-id="714a7-162">对用户的修正影响的说明。</span><span class="sxs-lookup"><span data-stu-id="714a7-162">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="714a7-163">actionUrl</span><span class="sxs-lookup"><span data-stu-id="714a7-163">actionUrl</span></span> | <span data-ttu-id="714a7-164">String</span><span class="sxs-lookup"><span data-stu-id="714a7-164">String</span></span>  |   <span data-ttu-id="714a7-165">该控件可进行的 URL。</span><span class="sxs-lookup"><span data-stu-id="714a7-165">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="714a7-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="714a7-166">lastModifiedDateTime</span></span> |  <span data-ttu-id="714a7-167">字符串 （方法）</span><span class="sxs-lookup"><span data-stu-id="714a7-167">String (DateTimeOffset)</span></span> |   <span data-ttu-id="714a7-168">上次修改日期</span><span class="sxs-lookup"><span data-stu-id="714a7-168">Date last modified</span></span> |
|   <span data-ttu-id="714a7-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="714a7-169">controlStateUpdates</span></span> |   <span data-ttu-id="714a7-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="714a7-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |  <span data-ttu-id="714a7-171">标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="714a7-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="714a7-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="714a7-172">vendorInformation</span></span> | [<span data-ttu-id="714a7-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="714a7-173">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="714a7-174">包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="714a7-174">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="714a7-175">关系</span><span class="sxs-lookup"><span data-stu-id="714a7-175">Relationships</span></span>

<span data-ttu-id="714a7-176">无。</span><span class="sxs-lookup"><span data-stu-id="714a7-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="714a7-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="714a7-177">JSON representation</span></span>

<span data-ttu-id="714a7-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="714a7-178">The following is a JSON representation of the resource.</span></span>

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
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
