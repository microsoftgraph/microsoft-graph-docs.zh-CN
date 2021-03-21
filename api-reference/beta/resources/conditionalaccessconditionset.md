---
title: conditionalAccessConditionSet 资源类型
description: 表示策略应用时所控制的条件类型。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 162943a5f2d51744ae37d6644f8a01eafb31c259
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961291"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="e5d7f-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5d7f-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="e5d7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5d7f-105">表示策略应用时所控制的条件类型。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="e5d7f-106">属性</span><span class="sxs-lookup"><span data-stu-id="e5d7f-106">Properties</span></span>

| <span data-ttu-id="e5d7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5d7f-107">Property</span></span>     | <span data-ttu-id="e5d7f-108">类型</span><span class="sxs-lookup"><span data-stu-id="e5d7f-108">Type</span></span>        | <span data-ttu-id="e5d7f-109">说明</span><span class="sxs-lookup"><span data-stu-id="e5d7f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5d7f-110">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5d7f-110">applications</span></span>|[<span data-ttu-id="e5d7f-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="e5d7f-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="e5d7f-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="e5d7f-113">必填。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-113">Required.</span></span> |
|<span data-ttu-id="e5d7f-114">users</span><span class="sxs-lookup"><span data-stu-id="e5d7f-114">users</span></span>|[<span data-ttu-id="e5d7f-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="e5d7f-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="e5d7f-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="e5d7f-117">必填。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-117">Required.</span></span> |
|<span data-ttu-id="e5d7f-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="e5d7f-118">clientAppTypes</span></span>|<span data-ttu-id="e5d7f-119">conditionalAccessClientApp 集合</span><span class="sxs-lookup"><span data-stu-id="e5d7f-119">conditionalAccessClientApp collection</span></span>| <span data-ttu-id="e5d7f-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-120">Client application types included in the policy.</span></span> <span data-ttu-id="e5d7f-121">可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span> <span data-ttu-id="e5d7f-122">必填。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-122">Required.</span></span>|
|<span data-ttu-id="e5d7f-123">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e5d7f-123">deviceStates</span></span>|[<span data-ttu-id="e5d7f-124">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="e5d7f-124">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="e5d7f-125">策略中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-125">Device states in the policy.</span></span> |
|<span data-ttu-id="e5d7f-126">设备</span><span class="sxs-lookup"><span data-stu-id="e5d7f-126">devices</span></span>|[<span data-ttu-id="e5d7f-127">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="e5d7f-127">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="e5d7f-128">策略中的设备。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-128">Devices in the policy.</span></span> |
|<span data-ttu-id="e5d7f-129">locations</span><span class="sxs-lookup"><span data-stu-id="e5d7f-129">locations</span></span>|[<span data-ttu-id="e5d7f-130">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="e5d7f-130">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="e5d7f-131">策略中包含的位置和从策略中排除的位置。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-131">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="e5d7f-132">平台</span><span class="sxs-lookup"><span data-stu-id="e5d7f-132">platforms</span></span>|[<span data-ttu-id="e5d7f-133">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="e5d7f-133">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="e5d7f-134">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-134">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="e5d7f-135">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="e5d7f-135">signInRiskLevels</span></span>|<span data-ttu-id="e5d7f-136">riskLevel 集合</span><span class="sxs-lookup"><span data-stu-id="e5d7f-136">riskLevel collection</span></span>| <span data-ttu-id="e5d7f-137">策略中包含的登录风险级别。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-137">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="e5d7f-138">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-138">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="e5d7f-139">必填。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-139">Required.</span></span>|
|<span data-ttu-id="e5d7f-140">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="e5d7f-140">userRiskLevels</span></span>|<span data-ttu-id="e5d7f-141">riskLevel 集合</span><span class="sxs-lookup"><span data-stu-id="e5d7f-141">riskLevel collection</span></span>| <span data-ttu-id="e5d7f-142">策略中包含的用户风险级别。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-142">User risk levels included in the policy.</span></span> <span data-ttu-id="e5d7f-143">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-143">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="e5d7f-144">必填。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-144">Required.</span></span>|

><span data-ttu-id="e5d7f-145">**注意：**</span><span class="sxs-lookup"><span data-stu-id="e5d7f-145">**Note:**</span></span>
>* <span data-ttu-id="e5d7f-146">**clientAppType** `modern` 将被弃用，并替换为 `mobileAppsAndDesktopClients` 。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-146">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> <br>
>* <span data-ttu-id="e5d7f-147">**clientAppType** `easUnsupported` 将弃用，支持包括 `exchangeActiveSync` EAS 支持和不受支持的平台。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-147">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> <br>
>* <span data-ttu-id="e5d7f-148">We are deprecating the **deviceStates** condition， and it may be removed in the future.</span><span class="sxs-lookup"><span data-stu-id="e5d7f-148">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="e5d7f-149">今后，使用 **设备** 条件。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-149">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="e5d7f-150">关系</span><span class="sxs-lookup"><span data-stu-id="e5d7f-150">Relationships</span></span>

<span data-ttu-id="e5d7f-151">无。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5d7f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5d7f-152">JSON representation</span></span>

<span data-ttu-id="e5d7f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5d7f-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "devices",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


