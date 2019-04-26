---
title: privilegedRoleSettings 资源类型
description: 表示特权角色的设置。
localization_priority: Normal
ms.openlocfilehash: 6500d5a51fcedce97d71c1c4022c7d941de27b83
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344211"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="00ceb-103">privilegedRoleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="00ceb-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00ceb-104">表示特权角色的设置。</span><span class="sxs-lookup"><span data-stu-id="00ceb-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="00ceb-105">方法</span><span class="sxs-lookup"><span data-stu-id="00ceb-105">Methods</span></span>

| <span data-ttu-id="00ceb-106">方法</span><span class="sxs-lookup"><span data-stu-id="00ceb-106">Method</span></span>           | <span data-ttu-id="00ceb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="00ceb-107">Return Type</span></span>    |<span data-ttu-id="00ceb-108">说明</span><span class="sxs-lookup"><span data-stu-id="00ceb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="00ceb-109">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="00ceb-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="00ceb-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="00ceb-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="00ceb-111">读取 privilegedRoleSettings 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00ceb-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="00ceb-112">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="00ceb-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="00ceb-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="00ceb-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="00ceb-114">更新 privilegedRoleSettings 对象。</span><span class="sxs-lookup"><span data-stu-id="00ceb-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="00ceb-115">属性</span><span class="sxs-lookup"><span data-stu-id="00ceb-115">Properties</span></span>
| <span data-ttu-id="00ceb-116">属性</span><span class="sxs-lookup"><span data-stu-id="00ceb-116">Property</span></span>     | <span data-ttu-id="00ceb-117">类型</span><span class="sxs-lookup"><span data-stu-id="00ceb-117">Type</span></span>   |<span data-ttu-id="00ceb-118">说明</span><span class="sxs-lookup"><span data-stu-id="00ceb-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00ceb-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="00ceb-119">elevationDuration</span></span>|<span data-ttu-id="00ceb-120">duration</span><span class="sxs-lookup"><span data-stu-id="00ceb-120">duration</span></span>|<span data-ttu-id="00ceb-121">激活角色的持续时间。</span><span class="sxs-lookup"><span data-stu-id="00ceb-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="00ceb-122">id</span><span class="sxs-lookup"><span data-stu-id="00ceb-122">id</span></span>|<span data-ttu-id="00ceb-123">string</span><span class="sxs-lookup"><span data-stu-id="00ceb-123">string</span></span>| <span data-ttu-id="00ceb-124">角色设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00ceb-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="00ceb-125">只读。</span><span class="sxs-lookup"><span data-stu-id="00ceb-125">Read-only.</span></span>|
|<span data-ttu-id="00ceb-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="00ceb-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="00ceb-127">boolean</span><span class="sxs-lookup"><span data-stu-id="00ceb-127">boolean</span></span>|<span data-ttu-id="00ceb-128">如果 mfaOnElevation 是可配置的,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="00ceb-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="00ceb-129">**假**如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="00ceb-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="00ceb-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="00ceb-130">lastGlobalAdmin</span></span>|<span data-ttu-id="00ceb-131">boolean</span><span class="sxs-lookup"><span data-stu-id="00ceb-131">boolean</span></span>|<span data-ttu-id="00ceb-132">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="00ceb-132">Internal used only.</span></span>|
|<span data-ttu-id="00ceb-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="00ceb-133">maxElavationDuration</span></span>|<span data-ttu-id="00ceb-134">duration</span><span class="sxs-lookup"><span data-stu-id="00ceb-134">duration</span></span>|<span data-ttu-id="00ceb-135">已激活角色的最大持续时间。</span><span class="sxs-lookup"><span data-stu-id="00ceb-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="00ceb-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="00ceb-136">mfaOnElevation</span></span>|<span data-ttu-id="00ceb-137">boolean</span><span class="sxs-lookup"><span data-stu-id="00ceb-137">boolean</span></span>|<span data-ttu-id="00ceb-138">如果需要 MFA 以激活角色,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="00ceb-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="00ceb-139">**假**如果无需进行 MFA 即可激活角色。</span><span class="sxs-lookup"><span data-stu-id="00ceb-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="00ceb-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="00ceb-140">minElevationDuration</span></span>|<span data-ttu-id="00ceb-141">duration</span><span class="sxs-lookup"><span data-stu-id="00ceb-141">duration</span></span>|<span data-ttu-id="00ceb-142">已激活角色的最短持续时间。</span><span class="sxs-lookup"><span data-stu-id="00ceb-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="00ceb-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="00ceb-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="00ceb-144">boolean</span><span class="sxs-lookup"><span data-stu-id="00ceb-144">boolean</span></span>|<span data-ttu-id="00ceb-145">如果激活角色时向最终用户发送通知,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="00ceb-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="00ceb-146">**假**如果在角色激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="00ceb-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="00ceb-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="00ceb-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="00ceb-148">boolean</span><span class="sxs-lookup"><span data-stu-id="00ceb-148">boolean</span></span>|<span data-ttu-id="00ceb-149">如果激活角色时需要票证信息,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="00ceb-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="00ceb-150">**假**如果激活角色时不需要票证信息。</span><span class="sxs-lookup"><span data-stu-id="00ceb-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="00ceb-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="00ceb-151">approvalOnElevation</span></span>|<span data-ttu-id="00ceb-152">boolean</span><span class="sxs-lookup"><span data-stu-id="00ceb-152">boolean</span></span>|<span data-ttu-id="00ceb-153">如果激活角色时需要进行审批,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="00ceb-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="00ceb-154">**假**如果激活该角色时不需要审批。</span><span class="sxs-lookup"><span data-stu-id="00ceb-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="00ceb-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="00ceb-155">approverIds</span></span>| <span data-ttu-id="00ceb-156">字符串集合</span><span class="sxs-lookup"><span data-stu-id="00ceb-156">string collection</span></span> |<span data-ttu-id="00ceb-157">审批 id 的列表 (如果激活需要审批)。</span><span class="sxs-lookup"><span data-stu-id="00ceb-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00ceb-158">关系</span><span class="sxs-lookup"><span data-stu-id="00ceb-158">Relationships</span></span>
<span data-ttu-id="00ceb-159">无</span><span class="sxs-lookup"><span data-stu-id="00ceb-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="00ceb-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00ceb-160">JSON representation</span></span>

<span data-ttu-id="00ceb-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00ceb-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": ["string"]
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
  "suppressions": []
}
-->
