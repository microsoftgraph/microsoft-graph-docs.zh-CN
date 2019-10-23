---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e81e8b2748a7dc3b6a9ca028472c1f6ab153b0e
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638510"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="9a21d-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a21d-103">conditionalAccessConditionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a21d-104">表示在应用策略时控制的条件的类型。</span><span class="sxs-lookup"><span data-stu-id="9a21d-104">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="9a21d-105">属性</span><span class="sxs-lookup"><span data-stu-id="9a21d-105">Properties</span></span>

| <span data-ttu-id="9a21d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a21d-106">Property</span></span>     | <span data-ttu-id="9a21d-107">类型</span><span class="sxs-lookup"><span data-stu-id="9a21d-107">Type</span></span>        | <span data-ttu-id="9a21d-108">说明</span><span class="sxs-lookup"><span data-stu-id="9a21d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a21d-109">来说</span><span class="sxs-lookup"><span data-stu-id="9a21d-109">applications</span></span>|[<span data-ttu-id="9a21d-110">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="9a21d-110">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="9a21d-111">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="9a21d-111">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="9a21d-112">必填。</span><span class="sxs-lookup"><span data-stu-id="9a21d-112">Required.</span></span> |
|<span data-ttu-id="9a21d-113">users</span><span class="sxs-lookup"><span data-stu-id="9a21d-113">users</span></span>|[<span data-ttu-id="9a21d-114">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="9a21d-114">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="9a21d-115">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="9a21d-115">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="9a21d-116">必填。</span><span class="sxs-lookup"><span data-stu-id="9a21d-116">Required.</span></span> |
|<span data-ttu-id="9a21d-117">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="9a21d-117">clientAppTypes</span></span>|<span data-ttu-id="9a21d-118">String collection</span><span class="sxs-lookup"><span data-stu-id="9a21d-118">String collection</span></span>| <span data-ttu-id="9a21d-119">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="9a21d-119">Client application types included in the policy.</span></span> <span data-ttu-id="9a21d-120">可取值为：`browser`、`modern`、`easSupported`、`easUnsupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="9a21d-120">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="9a21d-121">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9a21d-121">deviceStates</span></span>|[<span data-ttu-id="9a21d-122">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="9a21d-122">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="9a21d-123">策略中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="9a21d-123">Device states in the policy.</span></span> |
|<span data-ttu-id="9a21d-124">locations</span><span class="sxs-lookup"><span data-stu-id="9a21d-124">locations</span></span>|[<span data-ttu-id="9a21d-125">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="9a21d-125">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="9a21d-126">策略中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="9a21d-126">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="9a21d-127">平台</span><span class="sxs-lookup"><span data-stu-id="9a21d-127">platforms</span></span>|[<span data-ttu-id="9a21d-128">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="9a21d-128">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="9a21d-129">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="9a21d-129">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="9a21d-130">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="9a21d-130">signInRiskLevels</span></span>|<span data-ttu-id="9a21d-131">String collection</span><span class="sxs-lookup"><span data-stu-id="9a21d-131">String collection</span></span>| <span data-ttu-id="9a21d-132">策略中包括的风险级别。</span><span class="sxs-lookup"><span data-stu-id="9a21d-132">Risk levels included in the policy.</span></span> <span data-ttu-id="9a21d-133">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="9a21d-133">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a21d-134">关系</span><span class="sxs-lookup"><span data-stu-id="9a21d-134">Relationships</span></span>

<span data-ttu-id="9a21d-135">无。</span><span class="sxs-lookup"><span data-stu-id="9a21d-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a21d-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a21d-136">JSON representation</span></span>

<span data-ttu-id="9a21d-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a21d-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
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