---
title: stsPolicy 资源类型
description: 表示控制 Microsoft 标识平台行为的策略类型的抽象基本类型。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ba7afc9d338a0fd34b5548ca2ade69eebfecf29c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760888"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="ae65f-103">stsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae65f-103">stsPolicy resource type</span></span>

<span data-ttu-id="ae65f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae65f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae65f-105">表示控制 Microsoft 标识平台行为的策略类型的 [抽象基本](/azure/active-directory/develop/) 类型。</span><span class="sxs-lookup"><span data-stu-id="ae65f-105">Represents an abstract base type for policy types that control [Microsoft identity platform](/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="ae65f-106">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="ae65f-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ae65f-107">方法</span><span class="sxs-lookup"><span data-stu-id="ae65f-107">Methods</span></span>

<span data-ttu-id="ae65f-108">无</span><span class="sxs-lookup"><span data-stu-id="ae65f-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="ae65f-109">属性</span><span class="sxs-lookup"><span data-stu-id="ae65f-109">Properties</span></span>

| <span data-ttu-id="ae65f-110">属性</span><span class="sxs-lookup"><span data-stu-id="ae65f-110">Property</span></span>     | <span data-ttu-id="ae65f-111">类型</span><span class="sxs-lookup"><span data-stu-id="ae65f-111">Type</span></span>        | <span data-ttu-id="ae65f-112">说明</span><span class="sxs-lookup"><span data-stu-id="ae65f-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae65f-113">id</span><span class="sxs-lookup"><span data-stu-id="ae65f-113">id</span></span>|<span data-ttu-id="ae65f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="ae65f-114">String</span></span>| <span data-ttu-id="ae65f-115">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ae65f-115">Unique identifier for this policy.</span></span> <span data-ttu-id="ae65f-116">只读。</span><span class="sxs-lookup"><span data-stu-id="ae65f-116">Read-only.</span></span> <span data-ttu-id="ae65f-117">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="ae65f-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="ae65f-118">说明</span><span class="sxs-lookup"><span data-stu-id="ae65f-118">description</span></span>|<span data-ttu-id="ae65f-119">字符串</span><span class="sxs-lookup"><span data-stu-id="ae65f-119">String</span></span>| <span data-ttu-id="ae65f-120">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ae65f-120">Description for this policy.</span></span> <span data-ttu-id="ae65f-121">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="ae65f-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="ae65f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ae65f-122">displayName</span></span>|<span data-ttu-id="ae65f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="ae65f-123">String</span></span>| <span data-ttu-id="ae65f-124">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ae65f-124">Display name for this policy.</span></span> <span data-ttu-id="ae65f-125">继承自 [policyBase](policyBase.md)。</span><span class="sxs-lookup"><span data-stu-id="ae65f-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="ae65f-126">definition</span><span class="sxs-lookup"><span data-stu-id="ae65f-126">definition</span></span>|<span data-ttu-id="ae65f-127">字符串集合</span><span class="sxs-lookup"><span data-stu-id="ae65f-127">String collection</span></span>| <span data-ttu-id="ae65f-128">包含 JSON 字符串的字符串集合，用于定义策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="ae65f-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="ae65f-129">定义的语法因派生的策略类型不同而不同。</span><span class="sxs-lookup"><span data-stu-id="ae65f-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="ae65f-130">必填。</span><span class="sxs-lookup"><span data-stu-id="ae65f-130">Required.</span></span>|
|<span data-ttu-id="ae65f-131">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ae65f-131">isOrganizationDefault</span></span>|<span data-ttu-id="ae65f-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae65f-132">Boolean</span></span>|<span data-ttu-id="ae65f-133">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="ae65f-133">If set to true, activates this policy.</span></span> <span data-ttu-id="ae65f-134">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。</span><span class="sxs-lookup"><span data-stu-id="ae65f-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ae65f-135">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="ae65f-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae65f-136">关系</span><span class="sxs-lookup"><span data-stu-id="ae65f-136">Relationships</span></span>

<span data-ttu-id="ae65f-137">无</span><span class="sxs-lookup"><span data-stu-id="ae65f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae65f-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae65f-138">JSON representation</span></span>

<span data-ttu-id="ae65f-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae65f-139">The following is a JSON representation of the resource.</span></span>

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