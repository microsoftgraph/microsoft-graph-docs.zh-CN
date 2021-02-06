---
title: privilegedRoleSettings 资源类型
description: 表示特权角色的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: efc04b9b65719cbd5952dffb545d371172ab95eb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137632"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="e48a1-103">privilegedRoleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e48a1-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="e48a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e48a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e48a1-105">表示特权角色的设置。</span><span class="sxs-lookup"><span data-stu-id="e48a1-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="e48a1-106">方法</span><span class="sxs-lookup"><span data-stu-id="e48a1-106">Methods</span></span>

| <span data-ttu-id="e48a1-107">方法</span><span class="sxs-lookup"><span data-stu-id="e48a1-107">Method</span></span>           | <span data-ttu-id="e48a1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e48a1-108">Return Type</span></span>    |<span data-ttu-id="e48a1-109">说明</span><span class="sxs-lookup"><span data-stu-id="e48a1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e48a1-110">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e48a1-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="e48a1-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e48a1-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="e48a1-112">读取 privilegedRoleSettings 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e48a1-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="e48a1-113">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e48a1-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="e48a1-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e48a1-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="e48a1-115">更新 privilegedRoleSettings 对象。</span><span class="sxs-lookup"><span data-stu-id="e48a1-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="e48a1-116">属性</span><span class="sxs-lookup"><span data-stu-id="e48a1-116">Properties</span></span>
| <span data-ttu-id="e48a1-117">属性</span><span class="sxs-lookup"><span data-stu-id="e48a1-117">Property</span></span>     | <span data-ttu-id="e48a1-118">类型</span><span class="sxs-lookup"><span data-stu-id="e48a1-118">Type</span></span>   |<span data-ttu-id="e48a1-119">说明</span><span class="sxs-lookup"><span data-stu-id="e48a1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e48a1-120">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="e48a1-120">elevationDuration</span></span>|<span data-ttu-id="e48a1-121">duration</span><span class="sxs-lookup"><span data-stu-id="e48a1-121">duration</span></span>|<span data-ttu-id="e48a1-122">角色激活的持续时间。</span><span class="sxs-lookup"><span data-stu-id="e48a1-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="e48a1-123">id</span><span class="sxs-lookup"><span data-stu-id="e48a1-123">id</span></span>|<span data-ttu-id="e48a1-124">string</span><span class="sxs-lookup"><span data-stu-id="e48a1-124">string</span></span>| <span data-ttu-id="e48a1-125">角色设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e48a1-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="e48a1-126">只读。</span><span class="sxs-lookup"><span data-stu-id="e48a1-126">Read-only.</span></span>|
|<span data-ttu-id="e48a1-127">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="e48a1-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="e48a1-128">boolean</span><span class="sxs-lookup"><span data-stu-id="e48a1-128">boolean</span></span>|<span data-ttu-id="e48a1-129">**如此** 如果 mfaOnElevation 是可配置的。</span><span class="sxs-lookup"><span data-stu-id="e48a1-129">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="e48a1-130">**假** 如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="e48a1-130">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="e48a1-131">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="e48a1-131">lastGlobalAdmin</span></span>|<span data-ttu-id="e48a1-132">boolean</span><span class="sxs-lookup"><span data-stu-id="e48a1-132">boolean</span></span>|<span data-ttu-id="e48a1-133">仅内部使用。</span><span class="sxs-lookup"><span data-stu-id="e48a1-133">Internal used only.</span></span>|
|<span data-ttu-id="e48a1-134">maxEationDuration</span><span class="sxs-lookup"><span data-stu-id="e48a1-134">maxElavationDuration</span></span>|<span data-ttu-id="e48a1-135">duration</span><span class="sxs-lookup"><span data-stu-id="e48a1-135">duration</span></span>|<span data-ttu-id="e48a1-136">已激活角色的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="e48a1-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="e48a1-137">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="e48a1-137">mfaOnElevation</span></span>|<span data-ttu-id="e48a1-138">boolean</span><span class="sxs-lookup"><span data-stu-id="e48a1-138">boolean</span></span>|<span data-ttu-id="e48a1-139">如果激活角色需要 MFA，则其 **为 true。**</span><span class="sxs-lookup"><span data-stu-id="e48a1-139">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="e48a1-140">**假** 如果不需要 MFA 来激活角色。</span><span class="sxs-lookup"><span data-stu-id="e48a1-140">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="e48a1-141">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="e48a1-141">minElevationDuration</span></span>|<span data-ttu-id="e48a1-142">duration</span><span class="sxs-lookup"><span data-stu-id="e48a1-142">duration</span></span>|<span data-ttu-id="e48a1-143">已激活角色的最短持续时间。</span><span class="sxs-lookup"><span data-stu-id="e48a1-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="e48a1-144">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="e48a1-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="e48a1-145">boolean</span><span class="sxs-lookup"><span data-stu-id="e48a1-145">boolean</span></span>|<span data-ttu-id="e48a1-146">如果激活角色时向最终用户发送通知，则其为 **true。**</span><span class="sxs-lookup"><span data-stu-id="e48a1-146">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="e48a1-147">**假** 如果角色激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="e48a1-147">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="e48a1-148">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="e48a1-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="e48a1-149">boolean</span><span class="sxs-lookup"><span data-stu-id="e48a1-149">boolean</span></span>|<span data-ttu-id="e48a1-150">**如果** 激活角色时需要票证信息，则其为 true。</span><span class="sxs-lookup"><span data-stu-id="e48a1-150">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="e48a1-151">**假** 如果激活角色时不需要票证信息。</span><span class="sxs-lookup"><span data-stu-id="e48a1-151">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="e48a1-152">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="e48a1-152">approvalOnElevation</span></span>|<span data-ttu-id="e48a1-153">boolean</span><span class="sxs-lookup"><span data-stu-id="e48a1-153">boolean</span></span>|<span data-ttu-id="e48a1-154">**如此** 如果激活角色时需要审批。</span><span class="sxs-lookup"><span data-stu-id="e48a1-154">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="e48a1-155">**假** 如果激活角色时不需要审批。</span><span class="sxs-lookup"><span data-stu-id="e48a1-155">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="e48a1-156">approverIds</span><span class="sxs-lookup"><span data-stu-id="e48a1-156">approverIds</span></span>| <span data-ttu-id="e48a1-157">string 集合</span><span class="sxs-lookup"><span data-stu-id="e48a1-157">string collection</span></span> |<span data-ttu-id="e48a1-158">审批 ID 列表（如果需要审批才能激活）。</span><span class="sxs-lookup"><span data-stu-id="e48a1-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e48a1-159">关系</span><span class="sxs-lookup"><span data-stu-id="e48a1-159">Relationships</span></span>
<span data-ttu-id="e48a1-160">无</span><span class="sxs-lookup"><span data-stu-id="e48a1-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e48a1-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e48a1-161">JSON representation</span></span>

<span data-ttu-id="e48a1-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e48a1-162">Here is a JSON representation of the resource.</span></span>

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


