---
title: stsPolicy 资源类型
description: 表示用于控制 Microsoft identity platform 行为的策略类型的抽象基类型。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb43f538fe961af85c1a92f5e853ae8bca44b418
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581902"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="445d8-103">stsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="445d8-103">stsPolicy resource type</span></span>

<span data-ttu-id="445d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="445d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="445d8-105">表示用于控制 [Microsoft identity platform](/azure/active-directory/develop/) 行为的策略类型的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="445d8-105">Represents an abstract base type for policy types that control [Microsoft identity platform](/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="445d8-106">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="445d8-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="445d8-107">方法</span><span class="sxs-lookup"><span data-stu-id="445d8-107">Methods</span></span>

<span data-ttu-id="445d8-108">无</span><span class="sxs-lookup"><span data-stu-id="445d8-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="445d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="445d8-109">Properties</span></span>

| <span data-ttu-id="445d8-110">属性</span><span class="sxs-lookup"><span data-stu-id="445d8-110">Property</span></span>     | <span data-ttu-id="445d8-111">类型</span><span class="sxs-lookup"><span data-stu-id="445d8-111">Type</span></span>        | <span data-ttu-id="445d8-112">说明</span><span class="sxs-lookup"><span data-stu-id="445d8-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="445d8-113">id</span><span class="sxs-lookup"><span data-stu-id="445d8-113">id</span></span>|<span data-ttu-id="445d8-114">字符串</span><span class="sxs-lookup"><span data-stu-id="445d8-114">String</span></span>| <span data-ttu-id="445d8-115">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="445d8-115">Unique identifier for this policy.</span></span> <span data-ttu-id="445d8-116">只读。</span><span class="sxs-lookup"><span data-stu-id="445d8-116">Read-only.</span></span> <span data-ttu-id="445d8-117">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="445d8-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="445d8-118">description</span><span class="sxs-lookup"><span data-stu-id="445d8-118">description</span></span>|<span data-ttu-id="445d8-119">字符串</span><span class="sxs-lookup"><span data-stu-id="445d8-119">String</span></span>| <span data-ttu-id="445d8-120">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="445d8-120">Description for this policy.</span></span> <span data-ttu-id="445d8-121">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="445d8-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="445d8-122">displayName</span><span class="sxs-lookup"><span data-stu-id="445d8-122">displayName</span></span>|<span data-ttu-id="445d8-123">字符串</span><span class="sxs-lookup"><span data-stu-id="445d8-123">String</span></span>| <span data-ttu-id="445d8-124">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="445d8-124">Display name for this policy.</span></span> <span data-ttu-id="445d8-125">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="445d8-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="445d8-126">定义</span><span class="sxs-lookup"><span data-stu-id="445d8-126">definition</span></span>|<span data-ttu-id="445d8-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="445d8-127">String collection</span></span>| <span data-ttu-id="445d8-128">一个字符串集合，其中包含定义策略的规则和设置的 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="445d8-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="445d8-129">定义的语法因每个派生策略类型而异。</span><span class="sxs-lookup"><span data-stu-id="445d8-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="445d8-130">必填。</span><span class="sxs-lookup"><span data-stu-id="445d8-130">Required.</span></span>|
|<span data-ttu-id="445d8-131">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="445d8-131">isOrganizationDefault</span></span>|<span data-ttu-id="445d8-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="445d8-132">Boolean</span></span>|<span data-ttu-id="445d8-133">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="445d8-133">If set to true, activates this policy.</span></span> <span data-ttu-id="445d8-134">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="445d8-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="445d8-135">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="445d8-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="445d8-136">关系</span><span class="sxs-lookup"><span data-stu-id="445d8-136">Relationships</span></span>

<span data-ttu-id="445d8-137">无</span><span class="sxs-lookup"><span data-stu-id="445d8-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="445d8-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="445d8-138">JSON representation</span></span>

<span data-ttu-id="445d8-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="445d8-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->