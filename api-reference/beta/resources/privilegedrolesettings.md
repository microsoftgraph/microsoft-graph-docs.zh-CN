---
title: privilegedRoleSettings 资源类型
description: 代表特权角色的设置。
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2018
ms.locfileid: "27049557"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="a0405-103">privilegedRoleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0405-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="a0405-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a0405-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0405-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a0405-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0405-106">代表特权角色的设置。</span><span class="sxs-lookup"><span data-stu-id="a0405-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="a0405-107">方法</span><span class="sxs-lookup"><span data-stu-id="a0405-107">Methods</span></span>

| <span data-ttu-id="a0405-108">方法</span><span class="sxs-lookup"><span data-stu-id="a0405-108">Method</span></span>           | <span data-ttu-id="a0405-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0405-109">Return Type</span></span>    |<span data-ttu-id="a0405-110">说明</span><span class="sxs-lookup"><span data-stu-id="a0405-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0405-111">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="a0405-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="a0405-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="a0405-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="a0405-113">读取属性和 privilegedRoleSettings 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a0405-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="a0405-114">更新 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="a0405-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="a0405-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="a0405-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="a0405-116">更新 privilegedRoleSettings 对象。</span><span class="sxs-lookup"><span data-stu-id="a0405-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="a0405-117">属性</span><span class="sxs-lookup"><span data-stu-id="a0405-117">Properties</span></span>
| <span data-ttu-id="a0405-118">属性</span><span class="sxs-lookup"><span data-stu-id="a0405-118">Property</span></span>     | <span data-ttu-id="a0405-119">类型</span><span class="sxs-lookup"><span data-stu-id="a0405-119">Type</span></span>   |<span data-ttu-id="a0405-120">说明</span><span class="sxs-lookup"><span data-stu-id="a0405-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0405-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="a0405-121">elevationDuration</span></span>|<span data-ttu-id="a0405-122">duration</span><span class="sxs-lookup"><span data-stu-id="a0405-122">duration</span></span>|<span data-ttu-id="a0405-123">当激活角色持续时间。</span><span class="sxs-lookup"><span data-stu-id="a0405-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="a0405-124">id</span><span class="sxs-lookup"><span data-stu-id="a0405-124">id</span></span>|<span data-ttu-id="a0405-125">string</span><span class="sxs-lookup"><span data-stu-id="a0405-125">string</span></span>| <span data-ttu-id="a0405-126">角色设置唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a0405-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="a0405-127">只读。</span><span class="sxs-lookup"><span data-stu-id="a0405-127">Read-only.</span></span>|
|<span data-ttu-id="a0405-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="a0405-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="a0405-129">boolean</span><span class="sxs-lookup"><span data-stu-id="a0405-129">boolean</span></span>|<span data-ttu-id="a0405-130">**true**如果 mfaOnElevation 可配置。</span><span class="sxs-lookup"><span data-stu-id="a0405-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="a0405-131">**false**如果 mfaOnElevation 不可配置。</span><span class="sxs-lookup"><span data-stu-id="a0405-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="a0405-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="a0405-132">lastGlobalAdmin</span></span>|<span data-ttu-id="a0405-133">boolean</span><span class="sxs-lookup"><span data-stu-id="a0405-133">boolean</span></span>|<span data-ttu-id="a0405-134">仅供内部。</span><span class="sxs-lookup"><span data-stu-id="a0405-134">Internal used only.</span></span>|
|<span data-ttu-id="a0405-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="a0405-135">maxElavationDuration</span></span>|<span data-ttu-id="a0405-136">duration</span><span class="sxs-lookup"><span data-stu-id="a0405-136">duration</span></span>|<span data-ttu-id="a0405-137">激活角色的最大持续时间。</span><span class="sxs-lookup"><span data-stu-id="a0405-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="a0405-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="a0405-138">mfaOnElevation</span></span>|<span data-ttu-id="a0405-139">boolean</span><span class="sxs-lookup"><span data-stu-id="a0405-139">boolean</span></span>|<span data-ttu-id="a0405-140">如果为**true** MFA 需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="a0405-141">**false**如果 MFA 不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="a0405-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="a0405-142">minElevationDuration</span></span>|<span data-ttu-id="a0405-143">duration</span><span class="sxs-lookup"><span data-stu-id="a0405-143">duration</span></span>|<span data-ttu-id="a0405-144">最少持续时间激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="a0405-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="a0405-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="a0405-146">boolean</span><span class="sxs-lookup"><span data-stu-id="a0405-146">boolean</span></span>|<span data-ttu-id="a0405-147">**true**如果角色激活时向最终用户发送通知。</span><span class="sxs-lookup"><span data-stu-id="a0405-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="a0405-148">**false**如果角色被激活时不发送通知。</span><span class="sxs-lookup"><span data-stu-id="a0405-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="a0405-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="a0405-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="a0405-150">boolean</span><span class="sxs-lookup"><span data-stu-id="a0405-150">boolean</span></span>|<span data-ttu-id="a0405-151">如果为**true**时，票证信息是必需激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="a0405-152">**false**如果票证信息不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="a0405-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="a0405-153">approvalOnElevation</span></span>|<span data-ttu-id="a0405-154">boolean</span><span class="sxs-lookup"><span data-stu-id="a0405-154">boolean</span></span>|<span data-ttu-id="a0405-155">**true**如果情况下审批，需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="a0405-156">**false**如果审批不需要激活角色。</span><span class="sxs-lookup"><span data-stu-id="a0405-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="a0405-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="a0405-157">approverIds</span></span>|<span data-ttu-id="a0405-158">array</span><span class="sxs-lookup"><span data-stu-id="a0405-158">array</span></span>|<span data-ttu-id="a0405-159">审批 id，如果需要激活审核的列表。</span><span class="sxs-lookup"><span data-stu-id="a0405-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0405-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="a0405-160">Relationships</span></span>
<span data-ttu-id="a0405-161">无</span><span class="sxs-lookup"><span data-stu-id="a0405-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a0405-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0405-162">JSON representation</span></span>

<span data-ttu-id="a0405-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0405-163">Here is a JSON representation of the resource.</span></span>

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