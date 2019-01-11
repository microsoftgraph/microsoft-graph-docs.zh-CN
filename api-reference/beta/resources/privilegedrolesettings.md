---
title: privilegedRoleSettings 资源类型
description: 代表特权角色的设置。
localization_priority: Normal
ms.openlocfilehash: 971c48ce3ecdd2a219a111f3a11884377e20430c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842740"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="41668-103">privilegedRoleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="41668-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="41668-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41668-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41668-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41668-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41668-106">代表特权角色的设置。</span><span class="sxs-lookup"><span data-stu-id="41668-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="41668-107">方法</span><span class="sxs-lookup"><span data-stu-id="41668-107">Methods</span></span>

| <span data-ttu-id="41668-108">方法</span><span class="sxs-lookup"><span data-stu-id="41668-108">Method</span></span>           | <span data-ttu-id="41668-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="41668-109">Return Type</span></span>    |<span data-ttu-id="41668-110">说明</span><span class="sxs-lookup"><span data-stu-id="41668-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41668-111">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="41668-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="41668-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="41668-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="41668-113">读取属性和 privilegedRoleSettings 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="41668-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="41668-114">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="41668-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="41668-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="41668-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="41668-116">更新 privilegedRoleSettings 对象。</span><span class="sxs-lookup"><span data-stu-id="41668-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="41668-117">属性</span><span class="sxs-lookup"><span data-stu-id="41668-117">Properties</span></span>
| <span data-ttu-id="41668-118">属性</span><span class="sxs-lookup"><span data-stu-id="41668-118">Property</span></span>     | <span data-ttu-id="41668-119">类型</span><span class="sxs-lookup"><span data-stu-id="41668-119">Type</span></span>   |<span data-ttu-id="41668-120">Description</span><span class="sxs-lookup"><span data-stu-id="41668-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41668-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="41668-121">elevationDuration</span></span>|<span data-ttu-id="41668-122">duration</span><span class="sxs-lookup"><span data-stu-id="41668-122">duration</span></span>|<span data-ttu-id="41668-123">当激活角色持续时间。</span><span class="sxs-lookup"><span data-stu-id="41668-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="41668-124">id</span><span class="sxs-lookup"><span data-stu-id="41668-124">id</span></span>|<span data-ttu-id="41668-125">string</span><span class="sxs-lookup"><span data-stu-id="41668-125">string</span></span>| <span data-ttu-id="41668-126">角色设置唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="41668-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="41668-127">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="41668-127">Read-only.</span></span>|
|<span data-ttu-id="41668-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="41668-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="41668-129">boolean</span><span class="sxs-lookup"><span data-stu-id="41668-129">boolean</span></span>|<span data-ttu-id="41668-130">**true**如果 mfaOnElevation 可配置。</span><span class="sxs-lookup"><span data-stu-id="41668-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="41668-131">**false**如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="41668-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="41668-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="41668-132">lastGlobalAdmin</span></span>|<span data-ttu-id="41668-133">boolean</span><span class="sxs-lookup"><span data-stu-id="41668-133">boolean</span></span>|<span data-ttu-id="41668-134">仅供内部。</span><span class="sxs-lookup"><span data-stu-id="41668-134">Internal used only.</span></span>|
|<span data-ttu-id="41668-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="41668-135">maxElavationDuration</span></span>|<span data-ttu-id="41668-136">duration</span><span class="sxs-lookup"><span data-stu-id="41668-136">duration</span></span>|<span data-ttu-id="41668-137">激活角色的最大持续时间。</span><span class="sxs-lookup"><span data-stu-id="41668-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="41668-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="41668-138">mfaOnElevation</span></span>|<span data-ttu-id="41668-139">boolean</span><span class="sxs-lookup"><span data-stu-id="41668-139">boolean</span></span>|<span data-ttu-id="41668-140">如果为**true** MFA 需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="41668-141">**false**如果 MFA 不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="41668-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="41668-142">minElevationDuration</span></span>|<span data-ttu-id="41668-143">duration</span><span class="sxs-lookup"><span data-stu-id="41668-143">duration</span></span>|<span data-ttu-id="41668-144">最少持续时间激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="41668-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="41668-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="41668-146">boolean</span><span class="sxs-lookup"><span data-stu-id="41668-146">boolean</span></span>|<span data-ttu-id="41668-147">**true**如果角色激活时向最终用户发送通知。</span><span class="sxs-lookup"><span data-stu-id="41668-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="41668-148">**false**如果角色被激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="41668-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="41668-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="41668-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="41668-150">boolean</span><span class="sxs-lookup"><span data-stu-id="41668-150">boolean</span></span>|<span data-ttu-id="41668-151">如果为**true**时，票证信息是必需激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="41668-152">**false**如果票证信息不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="41668-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="41668-153">approvalOnElevation</span></span>|<span data-ttu-id="41668-154">boolean</span><span class="sxs-lookup"><span data-stu-id="41668-154">boolean</span></span>|<span data-ttu-id="41668-155">**true**如果情况下审批，需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="41668-156">**false**如果审批不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="41668-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="41668-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="41668-157">approverIds</span></span>|<span data-ttu-id="41668-158">array</span><span class="sxs-lookup"><span data-stu-id="41668-158">array</span></span>|<span data-ttu-id="41668-159">审批 id，如果需要激活审核的列表。</span><span class="sxs-lookup"><span data-stu-id="41668-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41668-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="41668-160">Relationships</span></span>
<span data-ttu-id="41668-161">无</span><span class="sxs-lookup"><span data-stu-id="41668-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="41668-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41668-162">JSON representation</span></span>

<span data-ttu-id="41668-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41668-163">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
