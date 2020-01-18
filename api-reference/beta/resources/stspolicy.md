---
title: stsPolicy 资源类型
description: 表示用于控制 Microsoft identity platform 行为的策略类型的抽象基类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f351d994daba00f4465d934fe570b5db2e704ae9
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234136"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="dbe6c-103">policyBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="dbe6c-103">policyBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbe6c-104">表示用于控制[Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/)行为的策略类型的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-104">Represents an abstract base type for policy types that control [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="dbe6c-105">继承自[policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-105">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dbe6c-106">方法</span><span class="sxs-lookup"><span data-stu-id="dbe6c-106">Methods</span></span>

<span data-ttu-id="dbe6c-107">无</span><span class="sxs-lookup"><span data-stu-id="dbe6c-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="dbe6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="dbe6c-108">Properties</span></span>

| <span data-ttu-id="dbe6c-109">属性</span><span class="sxs-lookup"><span data-stu-id="dbe6c-109">Property</span></span>     | <span data-ttu-id="dbe6c-110">类型</span><span class="sxs-lookup"><span data-stu-id="dbe6c-110">Type</span></span>        | <span data-ttu-id="dbe6c-111">说明</span><span class="sxs-lookup"><span data-stu-id="dbe6c-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dbe6c-112">id</span><span class="sxs-lookup"><span data-stu-id="dbe6c-112">id</span></span>|<span data-ttu-id="dbe6c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="dbe6c-113">String</span></span>| <span data-ttu-id="dbe6c-114">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-114">Unique identifier for this policy.</span></span> <span data-ttu-id="dbe6c-115">只读。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-115">Read-only.</span></span> <span data-ttu-id="dbe6c-116">继承自[policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-116">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="dbe6c-117">说明</span><span class="sxs-lookup"><span data-stu-id="dbe6c-117">description</span></span>|<span data-ttu-id="dbe6c-118">String</span><span class="sxs-lookup"><span data-stu-id="dbe6c-118">String</span></span>| <span data-ttu-id="dbe6c-119">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-119">Description for this policy.</span></span> <span data-ttu-id="dbe6c-120">继承自[policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-120">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="dbe6c-121">displayName</span><span class="sxs-lookup"><span data-stu-id="dbe6c-121">displayName</span></span>|<span data-ttu-id="dbe6c-122">String</span><span class="sxs-lookup"><span data-stu-id="dbe6c-122">String</span></span>| <span data-ttu-id="dbe6c-123">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-123">Display name for this policy.</span></span> <span data-ttu-id="dbe6c-124">继承自[policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-124">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="dbe6c-125">定义</span><span class="sxs-lookup"><span data-stu-id="dbe6c-125">definition</span></span>|<span data-ttu-id="dbe6c-126">String collection</span><span class="sxs-lookup"><span data-stu-id="dbe6c-126">String collection</span></span>| <span data-ttu-id="dbe6c-127">一个字符串集合，其中包含定义策略的规则和设置的 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-127">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="dbe6c-128">定义的语法因每个派生策略类型而异。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-128">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="dbe6c-129">必需。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-129">Required.</span></span>|
|<span data-ttu-id="dbe6c-130">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="dbe6c-130">isOrganizationDefault</span></span>|<span data-ttu-id="dbe6c-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbe6c-131">Boolean</span></span>|<span data-ttu-id="dbe6c-132">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-132">If set to true, activates this policy.</span></span> <span data-ttu-id="dbe6c-133">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-133">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="dbe6c-134">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-134">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbe6c-135">关系</span><span class="sxs-lookup"><span data-stu-id="dbe6c-135">Relationships</span></span>

<span data-ttu-id="dbe6c-136">无</span><span class="sxs-lookup"><span data-stu-id="dbe6c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbe6c-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dbe6c-137">JSON representation</span></span>

<span data-ttu-id="dbe6c-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbe6c-138">The following is a JSON representation of the resource.</span></span>

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