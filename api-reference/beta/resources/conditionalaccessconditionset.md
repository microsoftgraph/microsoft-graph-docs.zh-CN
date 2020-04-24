---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5db4c6367834733a4a5fbbb6c7a8d6b08393160
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805678"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="87f70-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="87f70-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="87f70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87f70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87f70-105">表示在应用策略时控制的条件的类型。</span><span class="sxs-lookup"><span data-stu-id="87f70-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="87f70-106">属性</span><span class="sxs-lookup"><span data-stu-id="87f70-106">Properties</span></span>

| <span data-ttu-id="87f70-107">属性</span><span class="sxs-lookup"><span data-stu-id="87f70-107">Property</span></span>     | <span data-ttu-id="87f70-108">类型</span><span class="sxs-lookup"><span data-stu-id="87f70-108">Type</span></span>        | <span data-ttu-id="87f70-109">说明</span><span class="sxs-lookup"><span data-stu-id="87f70-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87f70-110">来说</span><span class="sxs-lookup"><span data-stu-id="87f70-110">applications</span></span>|[<span data-ttu-id="87f70-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="87f70-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="87f70-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="87f70-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="87f70-113">必需。</span><span class="sxs-lookup"><span data-stu-id="87f70-113">Required.</span></span> |
|<span data-ttu-id="87f70-114">users</span><span class="sxs-lookup"><span data-stu-id="87f70-114">users</span></span>|[<span data-ttu-id="87f70-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="87f70-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="87f70-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="87f70-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="87f70-117">必需。</span><span class="sxs-lookup"><span data-stu-id="87f70-117">Required.</span></span> |
|<span data-ttu-id="87f70-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="87f70-118">clientAppTypes</span></span>|<span data-ttu-id="87f70-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="87f70-119">String collection</span></span>| <span data-ttu-id="87f70-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="87f70-120">Client application types included in the policy.</span></span> <span data-ttu-id="87f70-121">可取值为：`browser`、`modern`、`easSupported`、`easUnsupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="87f70-121">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="87f70-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="87f70-122">deviceStates</span></span>|[<span data-ttu-id="87f70-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="87f70-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="87f70-124">策略中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="87f70-124">Device states in the policy.</span></span> |
|<span data-ttu-id="87f70-125">驱动器</span><span class="sxs-lookup"><span data-stu-id="87f70-125">devices</span></span>|[<span data-ttu-id="87f70-126">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="87f70-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="87f70-127">策略中的设备。</span><span class="sxs-lookup"><span data-stu-id="87f70-127">Devices in the policy.</span></span> |
|<span data-ttu-id="87f70-128">位置</span><span class="sxs-lookup"><span data-stu-id="87f70-128">locations</span></span>|[<span data-ttu-id="87f70-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="87f70-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="87f70-130">策略中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="87f70-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="87f70-131">平台</span><span class="sxs-lookup"><span data-stu-id="87f70-131">platforms</span></span>|[<span data-ttu-id="87f70-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="87f70-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="87f70-133">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="87f70-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="87f70-134">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="87f70-134">signInRiskLevels</span></span>|<span data-ttu-id="87f70-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="87f70-135">String collection</span></span>| <span data-ttu-id="87f70-136">策略中包括的风险级别。</span><span class="sxs-lookup"><span data-stu-id="87f70-136">Risk levels included in the policy.</span></span> <span data-ttu-id="87f70-137">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="87f70-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="87f70-138">**注意：** 我们正在弃用**deviceStates**条件，将来可能会将其删除。</span><span class="sxs-lookup"><span data-stu-id="87f70-138">**Note:** We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="87f70-139">接下来，使用 "**设备**" 条件。</span><span class="sxs-lookup"><span data-stu-id="87f70-139">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="87f70-140">关系</span><span class="sxs-lookup"><span data-stu-id="87f70-140">Relationships</span></span>

<span data-ttu-id="87f70-141">无。</span><span class="sxs-lookup"><span data-stu-id="87f70-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87f70-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87f70-142">JSON representation</span></span>

<span data-ttu-id="87f70-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87f70-143">The following is a JSON representation of the resource.</span></span>

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
