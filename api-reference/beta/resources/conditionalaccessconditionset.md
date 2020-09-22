---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba88e9e5fd67bba5dd88fe323f3140bdbebff479
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994293"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="b8d34-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8d34-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="b8d34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8d34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8d34-105">表示在应用策略时控制的条件的类型。</span><span class="sxs-lookup"><span data-stu-id="b8d34-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="b8d34-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8d34-106">Properties</span></span>

| <span data-ttu-id="b8d34-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8d34-107">Property</span></span>     | <span data-ttu-id="b8d34-108">类型</span><span class="sxs-lookup"><span data-stu-id="b8d34-108">Type</span></span>        | <span data-ttu-id="b8d34-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8d34-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8d34-110">来说</span><span class="sxs-lookup"><span data-stu-id="b8d34-110">applications</span></span>|[<span data-ttu-id="b8d34-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="b8d34-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="b8d34-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="b8d34-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="b8d34-113">必需。</span><span class="sxs-lookup"><span data-stu-id="b8d34-113">Required.</span></span> |
|<span data-ttu-id="b8d34-114">users</span><span class="sxs-lookup"><span data-stu-id="b8d34-114">users</span></span>|[<span data-ttu-id="b8d34-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="b8d34-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="b8d34-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="b8d34-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="b8d34-117">必需。</span><span class="sxs-lookup"><span data-stu-id="b8d34-117">Required.</span></span> |
|<span data-ttu-id="b8d34-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="b8d34-118">clientAppTypes</span></span>|<span data-ttu-id="b8d34-119">String collection</span><span class="sxs-lookup"><span data-stu-id="b8d34-119">String collection</span></span>| <span data-ttu-id="b8d34-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="b8d34-120">Client application types included in the policy.</span></span> <span data-ttu-id="b8d34-121">可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="b8d34-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="b8d34-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="b8d34-122">deviceStates</span></span>|[<span data-ttu-id="b8d34-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="b8d34-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="b8d34-124">策略中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="b8d34-124">Device states in the policy.</span></span> |
|<span data-ttu-id="b8d34-125">驱动器</span><span class="sxs-lookup"><span data-stu-id="b8d34-125">devices</span></span>|[<span data-ttu-id="b8d34-126">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="b8d34-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="b8d34-127">策略中的设备。</span><span class="sxs-lookup"><span data-stu-id="b8d34-127">Devices in the policy.</span></span> |
|<span data-ttu-id="b8d34-128">位置</span><span class="sxs-lookup"><span data-stu-id="b8d34-128">locations</span></span>|[<span data-ttu-id="b8d34-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="b8d34-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="b8d34-130">策略中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="b8d34-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="b8d34-131">平台</span><span class="sxs-lookup"><span data-stu-id="b8d34-131">platforms</span></span>|[<span data-ttu-id="b8d34-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="b8d34-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="b8d34-133">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="b8d34-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="b8d34-134">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="b8d34-134">signInRiskLevels</span></span>|<span data-ttu-id="b8d34-135">String collection</span><span class="sxs-lookup"><span data-stu-id="b8d34-135">String collection</span></span>| <span data-ttu-id="b8d34-136">包含在策略中的登录风险级别。</span><span class="sxs-lookup"><span data-stu-id="b8d34-136">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="b8d34-137">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b8d34-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="b8d34-138">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="b8d34-138">userRiskLevels</span></span>|<span data-ttu-id="b8d34-139">String collection</span><span class="sxs-lookup"><span data-stu-id="b8d34-139">String collection</span></span>| <span data-ttu-id="b8d34-140">策略中包括的用户风险级别。</span><span class="sxs-lookup"><span data-stu-id="b8d34-140">User risk levels included in the policy.</span></span> <span data-ttu-id="b8d34-141">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b8d34-141">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="b8d34-142">**注意：**</span><span class="sxs-lookup"><span data-stu-id="b8d34-142">**Note:**</span></span> 

><span data-ttu-id="b8d34-143">**clientAppType** `modern` 即将弃用，并将替换为 `mobileAppsAndDesktopClients` 。</span><span class="sxs-lookup"><span data-stu-id="b8d34-143">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="b8d34-144">**clientAppType** `easUnsupported` 将被弃用，取而代之的是 `exchangeActiveSync` 包括 EAS 支持和不受支持的平台。</span><span class="sxs-lookup"><span data-stu-id="b8d34-144">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="b8d34-145">我们正在弃用 **deviceStates** 条件，将来可能会将其删除。</span><span class="sxs-lookup"><span data-stu-id="b8d34-145">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="b8d34-146">接下来，使用 " **设备** " 条件。</span><span class="sxs-lookup"><span data-stu-id="b8d34-146">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="b8d34-147">关系</span><span class="sxs-lookup"><span data-stu-id="b8d34-147">Relationships</span></span>

<span data-ttu-id="b8d34-148">无。</span><span class="sxs-lookup"><span data-stu-id="b8d34-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8d34-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8d34-149">JSON representation</span></span>

<span data-ttu-id="b8d34-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8d34-150">The following is a JSON representation of the resource.</span></span>

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


