---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3163bbefef420a878364f52f9dabc8dee1e7cae
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013672"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="3a199-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a199-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="3a199-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a199-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a199-105">表示在应用策略时控制的条件类型。</span><span class="sxs-lookup"><span data-stu-id="3a199-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="3a199-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a199-106">Properties</span></span>

| <span data-ttu-id="3a199-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a199-107">Property</span></span>     | <span data-ttu-id="3a199-108">类型</span><span class="sxs-lookup"><span data-stu-id="3a199-108">Type</span></span>        | <span data-ttu-id="3a199-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a199-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a199-110">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a199-110">applications</span></span>|[<span data-ttu-id="3a199-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="3a199-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="3a199-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="3a199-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="3a199-113">必填。</span><span class="sxs-lookup"><span data-stu-id="3a199-113">Required.</span></span> |
|<span data-ttu-id="3a199-114">users</span><span class="sxs-lookup"><span data-stu-id="3a199-114">users</span></span>|[<span data-ttu-id="3a199-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="3a199-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="3a199-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="3a199-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="3a199-117">必填。</span><span class="sxs-lookup"><span data-stu-id="3a199-117">Required.</span></span> |
|<span data-ttu-id="3a199-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="3a199-118">clientAppTypes</span></span>|<span data-ttu-id="3a199-119">String collection</span><span class="sxs-lookup"><span data-stu-id="3a199-119">String collection</span></span>| <span data-ttu-id="3a199-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="3a199-120">Client application types included in the policy.</span></span> <span data-ttu-id="3a199-121">可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="3a199-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="3a199-122">locations</span><span class="sxs-lookup"><span data-stu-id="3a199-122">locations</span></span>|[<span data-ttu-id="3a199-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="3a199-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="3a199-124">策略中包含的位置和从策略中排除的位置。</span><span class="sxs-lookup"><span data-stu-id="3a199-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="3a199-125">平台</span><span class="sxs-lookup"><span data-stu-id="3a199-125">platforms</span></span>|[<span data-ttu-id="3a199-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="3a199-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="3a199-127">策略中包含的平台和从策略中排除的平台。</span><span class="sxs-lookup"><span data-stu-id="3a199-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="3a199-128">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="3a199-128">signInRiskLevels</span></span>|<span data-ttu-id="3a199-129">String collection</span><span class="sxs-lookup"><span data-stu-id="3a199-129">String collection</span></span>| <span data-ttu-id="3a199-130">策略中包含的登录风险级别。</span><span class="sxs-lookup"><span data-stu-id="3a199-130">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="3a199-131">可取值为：`low`、`medium`、`high`、`none`。</span><span class="sxs-lookup"><span data-stu-id="3a199-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="3a199-132">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="3a199-132">userRiskLevels</span></span>|<span data-ttu-id="3a199-133">String collection</span><span class="sxs-lookup"><span data-stu-id="3a199-133">String collection</span></span>| <span data-ttu-id="3a199-134">策略中包含的用户风险级别。</span><span class="sxs-lookup"><span data-stu-id="3a199-134">User risk levels included in the policy.</span></span> <span data-ttu-id="3a199-135">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="3a199-135">Possible values are: `low`, `medium`, `high`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a199-136">关系</span><span class="sxs-lookup"><span data-stu-id="3a199-136">Relationships</span></span>

<span data-ttu-id="3a199-137">无。</span><span class="sxs-lookup"><span data-stu-id="3a199-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a199-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a199-138">JSON representation</span></span>

<span data-ttu-id="3a199-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a199-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
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
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
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

