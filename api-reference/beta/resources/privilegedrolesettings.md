---
title: privilegedRoleSettings 资源类型
description: 代表特权角色的设置。
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525694"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="c21a6-103">privilegedRoleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c21a6-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c21a6-104">代表特权角色的设置。</span><span class="sxs-lookup"><span data-stu-id="c21a6-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="c21a6-105">方法</span><span class="sxs-lookup"><span data-stu-id="c21a6-105">Methods</span></span>

| <span data-ttu-id="c21a6-106">方法</span><span class="sxs-lookup"><span data-stu-id="c21a6-106">Method</span></span>           | <span data-ttu-id="c21a6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c21a6-107">Return Type</span></span>    |<span data-ttu-id="c21a6-108">说明</span><span class="sxs-lookup"><span data-stu-id="c21a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c21a6-109">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c21a6-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="c21a6-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c21a6-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="c21a6-111">读取属性和 privilegedRoleSettings 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c21a6-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="c21a6-112">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c21a6-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="c21a6-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c21a6-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="c21a6-114">更新 privilegedRoleSettings 对象。</span><span class="sxs-lookup"><span data-stu-id="c21a6-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="c21a6-115">属性</span><span class="sxs-lookup"><span data-stu-id="c21a6-115">Properties</span></span>
| <span data-ttu-id="c21a6-116">属性</span><span class="sxs-lookup"><span data-stu-id="c21a6-116">Property</span></span>     | <span data-ttu-id="c21a6-117">类型</span><span class="sxs-lookup"><span data-stu-id="c21a6-117">Type</span></span>   |<span data-ttu-id="c21a6-118">说明</span><span class="sxs-lookup"><span data-stu-id="c21a6-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c21a6-119">ElevationDuration</span><span class="sxs-lookup"><span data-stu-id="c21a6-119">elevationDuration</span></span>|<span data-ttu-id="c21a6-120">duration</span><span class="sxs-lookup"><span data-stu-id="c21a6-120">duration</span></span>|<span data-ttu-id="c21a6-121">当激活角色持续时间。</span><span class="sxs-lookup"><span data-stu-id="c21a6-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="c21a6-122">id</span><span class="sxs-lookup"><span data-stu-id="c21a6-122">id</span></span>|<span data-ttu-id="c21a6-123">string</span><span class="sxs-lookup"><span data-stu-id="c21a6-123">string</span></span>| <span data-ttu-id="c21a6-124">角色设置唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c21a6-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="c21a6-125">只读。</span><span class="sxs-lookup"><span data-stu-id="c21a6-125">Read-only.</span></span>|
|<span data-ttu-id="c21a6-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="c21a6-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="c21a6-127">布尔</span><span class="sxs-lookup"><span data-stu-id="c21a6-127">boolean</span></span>|<span data-ttu-id="c21a6-128">**true**如果 mfaOnElevation 可配置。</span><span class="sxs-lookup"><span data-stu-id="c21a6-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="c21a6-129">**false**如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="c21a6-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="c21a6-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="c21a6-130">lastGlobalAdmin</span></span>|<span data-ttu-id="c21a6-131">布尔</span><span class="sxs-lookup"><span data-stu-id="c21a6-131">boolean</span></span>|<span data-ttu-id="c21a6-132">仅供内部。</span><span class="sxs-lookup"><span data-stu-id="c21a6-132">Internal used only.</span></span>|
|<span data-ttu-id="c21a6-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="c21a6-133">maxElavationDuration</span></span>|<span data-ttu-id="c21a6-134">duration</span><span class="sxs-lookup"><span data-stu-id="c21a6-134">duration</span></span>|<span data-ttu-id="c21a6-135">激活角色的最大持续时间。</span><span class="sxs-lookup"><span data-stu-id="c21a6-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="c21a6-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="c21a6-136">mfaOnElevation</span></span>|<span data-ttu-id="c21a6-137">布尔</span><span class="sxs-lookup"><span data-stu-id="c21a6-137">boolean</span></span>|<span data-ttu-id="c21a6-138">如果为**true** MFA 需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="c21a6-139">**false**如果 MFA 不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="c21a6-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="c21a6-140">minElevationDuration</span></span>|<span data-ttu-id="c21a6-141">duration</span><span class="sxs-lookup"><span data-stu-id="c21a6-141">duration</span></span>|<span data-ttu-id="c21a6-142">最少持续时间激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="c21a6-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="c21a6-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="c21a6-144">布尔</span><span class="sxs-lookup"><span data-stu-id="c21a6-144">boolean</span></span>|<span data-ttu-id="c21a6-145">**true**如果角色激活时向最终用户发送通知。</span><span class="sxs-lookup"><span data-stu-id="c21a6-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="c21a6-146">**false**如果角色被激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="c21a6-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="c21a6-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="c21a6-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="c21a6-148">布尔</span><span class="sxs-lookup"><span data-stu-id="c21a6-148">boolean</span></span>|<span data-ttu-id="c21a6-149">如果为**true**时，票证信息是必需激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="c21a6-150">**false**如果票证信息不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="c21a6-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="c21a6-151">approvalOnElevation</span></span>|<span data-ttu-id="c21a6-152">布尔</span><span class="sxs-lookup"><span data-stu-id="c21a6-152">boolean</span></span>|<span data-ttu-id="c21a6-153">**true**如果情况下审批，需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="c21a6-154">**false**如果审批不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="c21a6-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="c21a6-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="c21a6-155">approverIds</span></span>|<span data-ttu-id="c21a6-156">array</span><span class="sxs-lookup"><span data-stu-id="c21a6-156">array</span></span>|<span data-ttu-id="c21a6-157">审批 id，如果需要激活审核的列表。</span><span class="sxs-lookup"><span data-stu-id="c21a6-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c21a6-158">关系</span><span class="sxs-lookup"><span data-stu-id="c21a6-158">Relationships</span></span>
<span data-ttu-id="c21a6-159">无</span><span class="sxs-lookup"><span data-stu-id="c21a6-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c21a6-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c21a6-160">JSON representation</span></span>

<span data-ttu-id="c21a6-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c21a6-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
