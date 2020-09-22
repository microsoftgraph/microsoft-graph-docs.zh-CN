---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1fd96fb7bfa54ff059afa83b7ea922737dc90809
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018926"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="f22ba-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="f22ba-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="f22ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f22ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f22ba-105">表示在应用策略时控制的条件的类型。</span><span class="sxs-lookup"><span data-stu-id="f22ba-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="f22ba-106">属性</span><span class="sxs-lookup"><span data-stu-id="f22ba-106">Properties</span></span>

| <span data-ttu-id="f22ba-107">属性</span><span class="sxs-lookup"><span data-stu-id="f22ba-107">Property</span></span>     | <span data-ttu-id="f22ba-108">类型</span><span class="sxs-lookup"><span data-stu-id="f22ba-108">Type</span></span>        | <span data-ttu-id="f22ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="f22ba-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f22ba-110">来说</span><span class="sxs-lookup"><span data-stu-id="f22ba-110">applications</span></span>|[<span data-ttu-id="f22ba-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="f22ba-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="f22ba-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="f22ba-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="f22ba-113">必需。</span><span class="sxs-lookup"><span data-stu-id="f22ba-113">Required.</span></span> |
|<span data-ttu-id="f22ba-114">users</span><span class="sxs-lookup"><span data-stu-id="f22ba-114">users</span></span>|[<span data-ttu-id="f22ba-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="f22ba-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="f22ba-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="f22ba-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="f22ba-117">必需。</span><span class="sxs-lookup"><span data-stu-id="f22ba-117">Required.</span></span> |
|<span data-ttu-id="f22ba-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="f22ba-118">clientAppTypes</span></span>|<span data-ttu-id="f22ba-119">String collection</span><span class="sxs-lookup"><span data-stu-id="f22ba-119">String collection</span></span>| <span data-ttu-id="f22ba-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="f22ba-120">Client application types included in the policy.</span></span> <span data-ttu-id="f22ba-121">可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="f22ba-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="f22ba-122">位置</span><span class="sxs-lookup"><span data-stu-id="f22ba-122">locations</span></span>|[<span data-ttu-id="f22ba-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="f22ba-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="f22ba-124">策略中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="f22ba-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="f22ba-125">平台</span><span class="sxs-lookup"><span data-stu-id="f22ba-125">platforms</span></span>|[<span data-ttu-id="f22ba-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="f22ba-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="f22ba-127">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="f22ba-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="f22ba-128">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="f22ba-128">signInRiskLevels</span></span>|<span data-ttu-id="f22ba-129">String collection</span><span class="sxs-lookup"><span data-stu-id="f22ba-129">String collection</span></span>| <span data-ttu-id="f22ba-130">策略中包括的风险级别。</span><span class="sxs-lookup"><span data-stu-id="f22ba-130">Risk levels included in the policy.</span></span> <span data-ttu-id="f22ba-131">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="f22ba-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f22ba-132">关系</span><span class="sxs-lookup"><span data-stu-id="f22ba-132">Relationships</span></span>

<span data-ttu-id="f22ba-133">无。</span><span class="sxs-lookup"><span data-stu-id="f22ba-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f22ba-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f22ba-134">JSON representation</span></span>

<span data-ttu-id="f22ba-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f22ba-135">The following is a JSON representation of the resource.</span></span>

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

