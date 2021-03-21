---
title: conditionalAccessConditionSet 资源类型
description: 表示策略应用时所控制的条件类型。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d448b2d54fbc94c63588712f06492ce7d38a33a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962495"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="1f254-103">conditionalAccessConditionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f254-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="1f254-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f254-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f254-105">表示策略应用时所控制的条件类型。</span><span class="sxs-lookup"><span data-stu-id="1f254-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="1f254-106">属性</span><span class="sxs-lookup"><span data-stu-id="1f254-106">Properties</span></span>

| <span data-ttu-id="1f254-107">属性</span><span class="sxs-lookup"><span data-stu-id="1f254-107">Property</span></span>     | <span data-ttu-id="1f254-108">类型</span><span class="sxs-lookup"><span data-stu-id="1f254-108">Type</span></span>        | <span data-ttu-id="1f254-109">说明</span><span class="sxs-lookup"><span data-stu-id="1f254-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f254-110">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f254-110">applications</span></span>|[<span data-ttu-id="1f254-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="1f254-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="1f254-112">策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="1f254-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="1f254-113">必填。</span><span class="sxs-lookup"><span data-stu-id="1f254-113">Required.</span></span> |
|<span data-ttu-id="1f254-114">users</span><span class="sxs-lookup"><span data-stu-id="1f254-114">users</span></span>|[<span data-ttu-id="1f254-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="1f254-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="1f254-116">策略中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="1f254-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="1f254-117">必填。</span><span class="sxs-lookup"><span data-stu-id="1f254-117">Required.</span></span> |
|<span data-ttu-id="1f254-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="1f254-118">clientAppTypes</span></span>|<span data-ttu-id="1f254-119">conditionalAccessClientApp 集合</span><span class="sxs-lookup"><span data-stu-id="1f254-119">conditionalAccessClientApp collection</span></span>| <span data-ttu-id="1f254-120">策略中包含的客户端应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="1f254-120">Client application types included in the policy.</span></span> <span data-ttu-id="1f254-121">可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。</span><span class="sxs-lookup"><span data-stu-id="1f254-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span> <span data-ttu-id="1f254-122">必填。</span><span class="sxs-lookup"><span data-stu-id="1f254-122">Required.</span></span>|
|<span data-ttu-id="1f254-123">locations</span><span class="sxs-lookup"><span data-stu-id="1f254-123">locations</span></span>|[<span data-ttu-id="1f254-124">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="1f254-124">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="1f254-125">策略中包含的位置和从策略中排除的位置。</span><span class="sxs-lookup"><span data-stu-id="1f254-125">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="1f254-126">平台</span><span class="sxs-lookup"><span data-stu-id="1f254-126">platforms</span></span>|[<span data-ttu-id="1f254-127">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="1f254-127">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="1f254-128">策略中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="1f254-128">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="1f254-129">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="1f254-129">signInRiskLevels</span></span>|<span data-ttu-id="1f254-130">riskLevel 集合</span><span class="sxs-lookup"><span data-stu-id="1f254-130">riskLevel collection</span></span>| <span data-ttu-id="1f254-131">策略中包含的登录风险级别。</span><span class="sxs-lookup"><span data-stu-id="1f254-131">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="1f254-132">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1f254-132">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="1f254-133">必填。</span><span class="sxs-lookup"><span data-stu-id="1f254-133">Required.</span></span>|
|<span data-ttu-id="1f254-134">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="1f254-134">userRiskLevels</span></span>|<span data-ttu-id="1f254-135">riskLevel 集合</span><span class="sxs-lookup"><span data-stu-id="1f254-135">riskLevel collection</span></span>| <span data-ttu-id="1f254-136">策略中包含的用户风险级别。</span><span class="sxs-lookup"><span data-stu-id="1f254-136">User risk levels included in the policy.</span></span> <span data-ttu-id="1f254-137">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1f254-137">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="1f254-138">必填。</span><span class="sxs-lookup"><span data-stu-id="1f254-138">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f254-139">关系</span><span class="sxs-lookup"><span data-stu-id="1f254-139">Relationships</span></span>

<span data-ttu-id="1f254-140">无。</span><span class="sxs-lookup"><span data-stu-id="1f254-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f254-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f254-141">JSON representation</span></span>

<span data-ttu-id="1f254-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f254-142">The following is a JSON representation of the resource.</span></span>

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

