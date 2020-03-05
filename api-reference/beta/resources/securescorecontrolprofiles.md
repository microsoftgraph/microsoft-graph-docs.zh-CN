---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7dfca5eedebe7f2fe524c79cee52e5855af7f291
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520862"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="32358-104">secureScoreControlProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="32358-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="32358-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="32358-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32358-106">表示租户的每个控件数据的安全分数。</span><span class="sxs-lookup"><span data-stu-id="32358-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="32358-107">默认情况下，它将返回租户的所有控件，并可显式提取各个控件。</span><span class="sxs-lookup"><span data-stu-id="32358-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="32358-108">方法</span><span class="sxs-lookup"><span data-stu-id="32358-108">Methods</span></span>

| <span data-ttu-id="32358-109">方法</span><span class="sxs-lookup"><span data-stu-id="32358-109">Method</span></span>   | <span data-ttu-id="32358-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="32358-110">Return Type</span></span>|<span data-ttu-id="32358-111">说明</span><span class="sxs-lookup"><span data-stu-id="32358-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32358-112">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="32358-112">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="32358-113">[secureScoreControlProfile](securescorecontrolprofiles.md)集合</span><span class="sxs-lookup"><span data-stu-id="32358-113">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="32358-114">获取 secureScoreControlProfile 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="32358-114">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="32358-115">属性</span><span class="sxs-lookup"><span data-stu-id="32358-115">Properties</span></span>

|<span data-ttu-id="32358-116">名称</span><span class="sxs-lookup"><span data-stu-id="32358-116">Name</span></span> |<span data-ttu-id="32358-117">类型</span><span class="sxs-lookup"><span data-stu-id="32358-117">Type</span></span> |<span data-ttu-id="32358-118">说明</span><span class="sxs-lookup"><span data-stu-id="32358-118">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="32358-119">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="32358-119">azureTenantId</span></span>   |   <span data-ttu-id="32358-120">字符串</span><span class="sxs-lookup"><span data-stu-id="32358-120">String</span></span>  |   <span data-ttu-id="32358-121">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="32358-121">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="32358-122">controlName</span><span class="sxs-lookup"><span data-stu-id="32358-122">controlName</span></span> |   <span data-ttu-id="32358-123">String</span><span class="sxs-lookup"><span data-stu-id="32358-123">String</span></span>  |   <span data-ttu-id="32358-124">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="32358-124">Name of the control.</span></span> |
|   <span data-ttu-id="32358-125">title</span><span class="sxs-lookup"><span data-stu-id="32358-125">title</span></span>   |   <span data-ttu-id="32358-126">String</span><span class="sxs-lookup"><span data-stu-id="32358-126">String</span></span>  |   <span data-ttu-id="32358-127">控件的标题。</span><span class="sxs-lookup"><span data-stu-id="32358-127">Title of the control.</span></span>   |
| <span data-ttu-id="32358-128">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="32358-128">complianceInformation</span></span> | <span data-ttu-id="32358-129">[complianceInformation](complianceinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="32358-129">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="32358-130">与安全得分控制相关联的合规性信息的集合</span><span class="sxs-lookup"><span data-stu-id="32358-130">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="32358-131">controlCategory</span><span class="sxs-lookup"><span data-stu-id="32358-131">controlCategory</span></span> |   <span data-ttu-id="32358-132">String</span><span class="sxs-lookup"><span data-stu-id="32358-132">String</span></span>  |   <span data-ttu-id="32358-133">控制措施类别（帐户、数据、设备、应用程序、基础结构）。</span><span class="sxs-lookup"><span data-stu-id="32358-133">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="32358-134">actionType</span><span class="sxs-lookup"><span data-stu-id="32358-134">actionType</span></span>  |   <span data-ttu-id="32358-135">String</span><span class="sxs-lookup"><span data-stu-id="32358-135">String</span></span>  |   <span data-ttu-id="32358-136">控制操作类型（Config、审阅、行为）。</span><span class="sxs-lookup"><span data-stu-id="32358-136">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="32358-137">service</span><span class="sxs-lookup"><span data-stu-id="32358-137">service</span></span> |   <span data-ttu-id="32358-138">String</span><span class="sxs-lookup"><span data-stu-id="32358-138">String</span></span>  |   <span data-ttu-id="32358-139">拥有控件的服务（Exchange、Sharepoint、Azure AD）。</span><span class="sxs-lookup"><span data-stu-id="32358-139">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="32358-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="32358-140">maxScore</span></span> |  <span data-ttu-id="32358-141">String</span><span class="sxs-lookup"><span data-stu-id="32358-141">String</span></span>  |   <span data-ttu-id="32358-142">指定日期的当前获得的最大分数。</span><span class="sxs-lookup"><span data-stu-id="32358-142">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="32358-143">单层</span><span class="sxs-lookup"><span data-stu-id="32358-143">tier</span></span> |  <span data-ttu-id="32358-144">String</span><span class="sxs-lookup"><span data-stu-id="32358-144">String</span></span>  |   <span data-ttu-id="32358-145">控制层（Core，纵深防御，高级。）</span><span class="sxs-lookup"><span data-stu-id="32358-145">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="32358-146">userImpact</span><span class="sxs-lookup"><span data-stu-id="32358-146">userImpact</span></span> |    <span data-ttu-id="32358-147">String</span><span class="sxs-lookup"><span data-stu-id="32358-147">String</span></span>  | <span data-ttu-id="32358-148">实施控制的用户影响（低、中等、高）。</span><span class="sxs-lookup"><span data-stu-id="32358-148">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="32358-149">implementationCost</span><span class="sxs-lookup"><span data-stu-id="32358-149">implementationCost</span></span> |    <span data-ttu-id="32358-150">String</span><span class="sxs-lookup"><span data-stu-id="32358-150">String</span></span>  |   <span data-ttu-id="32358-151">Implemmentating 控件的资源成本（low、适中、high）。</span><span class="sxs-lookup"><span data-stu-id="32358-151">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="32358-152">排名</span><span class="sxs-lookup"><span data-stu-id="32358-152">rank</span></span> |  <span data-ttu-id="32358-153">Int32</span><span class="sxs-lookup"><span data-stu-id="32358-153">Int32</span></span>   |   <span data-ttu-id="32358-154">Microsoft 的控制堆栈排名。</span><span class="sxs-lookup"><span data-stu-id="32358-154">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="32358-155">病毒</span><span class="sxs-lookup"><span data-stu-id="32358-155">threats</span></span> |   <span data-ttu-id="32358-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="32358-156">String Collection</span></span>   |   <span data-ttu-id="32358-157">控制缓解的威胁列表（accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗）。</span><span class="sxs-lookup"><span data-stu-id="32358-157">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="32358-158">被</span><span class="sxs-lookup"><span data-stu-id="32358-158">deprecated</span></span> |    <span data-ttu-id="32358-159">布尔</span><span class="sxs-lookup"><span data-stu-id="32358-159">Boolean</span></span> |   <span data-ttu-id="32358-160">指示是否已对控件进行折旧的标志。</span><span class="sxs-lookup"><span data-stu-id="32358-160">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="32358-161">纠正</span><span class="sxs-lookup"><span data-stu-id="32358-161">remediation</span></span> |   <span data-ttu-id="32358-162">String</span><span class="sxs-lookup"><span data-stu-id="32358-162">String</span></span>  |   <span data-ttu-id="32358-163">对控件将有助于修正的内容的说明。</span><span class="sxs-lookup"><span data-stu-id="32358-163">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="32358-164">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="32358-164">remediationImpact</span></span> | <span data-ttu-id="32358-165">String</span><span class="sxs-lookup"><span data-stu-id="32358-165">String</span></span>  |   <span data-ttu-id="32358-166">对修正用户影响的说明。</span><span class="sxs-lookup"><span data-stu-id="32358-166">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="32358-167">actionUrl</span><span class="sxs-lookup"><span data-stu-id="32358-167">actionUrl</span></span> | <span data-ttu-id="32358-168">String</span><span class="sxs-lookup"><span data-stu-id="32358-168">String</span></span>  |   <span data-ttu-id="32358-169">可将控件 actioned 到的位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="32358-169">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="32358-170">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="32358-170">controlStateUpdates</span></span> | <span data-ttu-id="32358-171">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合</span><span class="sxs-lookup"><span data-stu-id="32358-171">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="32358-172">用于指示租户已标记控件的位置的标志（忽略、thirdParty、已审阅）（支持[更新](../api/securescorecontrolprofiles-update.md)）。</span><span class="sxs-lookup"><span data-stu-id="32358-172">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="32358-173">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="32358-173">vendorInformation</span></span> | [<span data-ttu-id="32358-174">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="32358-174">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="32358-175">关系</span><span class="sxs-lookup"><span data-stu-id="32358-175">Relationships</span></span>

<span data-ttu-id="32358-176">无。</span><span class="sxs-lookup"><span data-stu-id="32358-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32358-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32358-177">JSON representation</span></span>

<span data-ttu-id="32358-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32358-178">The following is a JSON representation of the resource.</span></span>

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
