---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 993201181a9256b54663ce279c914e3669f4dc91
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384470"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="ee68d-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee68d-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="ee68d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee68d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee68d-105">表示在应用策略时控制的条件的类型。</span><span class="sxs-lookup"><span data-stu-id="ee68d-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="ee68d-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee68d-106">Properties</span></span>

| <span data-ttu-id="ee68d-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee68d-107">Property</span></span>     | <span data-ttu-id="ee68d-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee68d-108">Type</span></span>        | <span data-ttu-id="ee68d-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee68d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee68d-110">来说</span><span class="sxs-lookup"><span data-stu-id="ee68d-110">applications</span></span>|[<span data-ttu-id="ee68d-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="ee68d-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="ee68d-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="ee68d-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="ee68d-113">必需。</span><span class="sxs-lookup"><span data-stu-id="ee68d-113">Required.</span></span> |
|<span data-ttu-id="ee68d-114">users</span><span class="sxs-lookup"><span data-stu-id="ee68d-114">users</span></span>|[<span data-ttu-id="ee68d-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="ee68d-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="ee68d-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="ee68d-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="ee68d-117">必需。</span><span class="sxs-lookup"><span data-stu-id="ee68d-117">Required.</span></span> |
|<span data-ttu-id="ee68d-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="ee68d-118">clientAppTypes</span></span>|<span data-ttu-id="ee68d-119">String collection</span><span class="sxs-lookup"><span data-stu-id="ee68d-119">String collection</span></span>| <span data-ttu-id="ee68d-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="ee68d-120">Client application types included in the policy.</span></span> <span data-ttu-id="ee68d-121">可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="ee68d-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="ee68d-122">locations</span><span class="sxs-lookup"><span data-stu-id="ee68d-122">locations</span></span>|[<span data-ttu-id="ee68d-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="ee68d-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="ee68d-124">策略中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="ee68d-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="ee68d-125">平台</span><span class="sxs-lookup"><span data-stu-id="ee68d-125">platforms</span></span>|[<span data-ttu-id="ee68d-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="ee68d-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="ee68d-127">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="ee68d-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="ee68d-128">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="ee68d-128">signInRiskLevels</span></span>|<span data-ttu-id="ee68d-129">String collection</span><span class="sxs-lookup"><span data-stu-id="ee68d-129">String collection</span></span>| <span data-ttu-id="ee68d-130">策略中包括的风险级别。</span><span class="sxs-lookup"><span data-stu-id="ee68d-130">Risk levels included in the policy.</span></span> <span data-ttu-id="ee68d-131">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="ee68d-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee68d-132">关系</span><span class="sxs-lookup"><span data-stu-id="ee68d-132">Relationships</span></span>

<span data-ttu-id="ee68d-133">无。</span><span class="sxs-lookup"><span data-stu-id="ee68d-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee68d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee68d-134">JSON representation</span></span>

<span data-ttu-id="ee68d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee68d-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
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
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
