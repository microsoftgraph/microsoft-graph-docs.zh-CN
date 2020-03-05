---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dee80ebdacfda6c0b633f1aec1dd085d80eb22e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507560"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="bd975-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd975-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="bd975-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bd975-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd975-105">表示在应用策略时控制的条件的类型。</span><span class="sxs-lookup"><span data-stu-id="bd975-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="bd975-106">属性</span><span class="sxs-lookup"><span data-stu-id="bd975-106">Properties</span></span>

| <span data-ttu-id="bd975-107">属性</span><span class="sxs-lookup"><span data-stu-id="bd975-107">Property</span></span>     | <span data-ttu-id="bd975-108">类型</span><span class="sxs-lookup"><span data-stu-id="bd975-108">Type</span></span>        | <span data-ttu-id="bd975-109">说明</span><span class="sxs-lookup"><span data-stu-id="bd975-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bd975-110">来说</span><span class="sxs-lookup"><span data-stu-id="bd975-110">applications</span></span>|[<span data-ttu-id="bd975-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="bd975-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="bd975-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="bd975-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="bd975-113">必填。</span><span class="sxs-lookup"><span data-stu-id="bd975-113">Required.</span></span> |
|<span data-ttu-id="bd975-114">users</span><span class="sxs-lookup"><span data-stu-id="bd975-114">users</span></span>|[<span data-ttu-id="bd975-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="bd975-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="bd975-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="bd975-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="bd975-117">必填。</span><span class="sxs-lookup"><span data-stu-id="bd975-117">Required.</span></span> |
|<span data-ttu-id="bd975-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="bd975-118">clientAppTypes</span></span>|<span data-ttu-id="bd975-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd975-119">String collection</span></span>| <span data-ttu-id="bd975-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="bd975-120">Client application types included in the policy.</span></span> <span data-ttu-id="bd975-121">可取值为：`browser`、`modern`、`easSupported`、`easUnsupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="bd975-121">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="bd975-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="bd975-122">deviceStates</span></span>|[<span data-ttu-id="bd975-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="bd975-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="bd975-124">策略中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="bd975-124">Device states in the policy.</span></span> |
|<span data-ttu-id="bd975-125">位置</span><span class="sxs-lookup"><span data-stu-id="bd975-125">locations</span></span>|[<span data-ttu-id="bd975-126">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="bd975-126">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="bd975-127">策略中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="bd975-127">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="bd975-128">平台</span><span class="sxs-lookup"><span data-stu-id="bd975-128">platforms</span></span>|[<span data-ttu-id="bd975-129">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="bd975-129">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="bd975-130">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="bd975-130">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="bd975-131">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="bd975-131">signInRiskLevels</span></span>|<span data-ttu-id="bd975-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd975-132">String collection</span></span>| <span data-ttu-id="bd975-133">策略中包括的风险级别。</span><span class="sxs-lookup"><span data-stu-id="bd975-133">Risk levels included in the policy.</span></span> <span data-ttu-id="bd975-134">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="bd975-134">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd975-135">关系</span><span class="sxs-lookup"><span data-stu-id="bd975-135">Relationships</span></span>

<span data-ttu-id="bd975-136">无。</span><span class="sxs-lookup"><span data-stu-id="bd975-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd975-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd975-137">JSON representation</span></span>

<span data-ttu-id="bd975-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd975-138">The following is a JSON representation of the resource.</span></span>

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