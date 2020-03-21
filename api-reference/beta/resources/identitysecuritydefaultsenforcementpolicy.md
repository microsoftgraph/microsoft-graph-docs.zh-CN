---
title: identitySecurityDefaultsEnforcementPolicy 资源类型
description: 表示 Azure Active Directory 安全性默认策略。 安全性默认值包含针对常见攻击进行保护的预先配置的安全设置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3cb792b59281c05cc915649bf3b689714438bd93
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895618"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="be585-104">identitySecurityDefaultsEnforcementPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="be585-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="be585-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be585-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be585-106">表示 Azure Active Directory[安全性默认](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)策略。</span><span class="sxs-lookup"><span data-stu-id="be585-106">Represents the Azure Active Directory [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="be585-107">安全性默认值包含针对常见攻击进行保护的预先配置的安全设置。</span><span class="sxs-lookup"><span data-stu-id="be585-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="be585-108">继承自[policyBase](../resources/policybase.md)。</span><span class="sxs-lookup"><span data-stu-id="be585-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="be585-109">方法</span><span class="sxs-lookup"><span data-stu-id="be585-109">Methods</span></span>

| <span data-ttu-id="be585-110">方法</span><span class="sxs-lookup"><span data-stu-id="be585-110">Method</span></span>       | <span data-ttu-id="be585-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="be585-111">Return Type</span></span> | <span data-ttu-id="be585-112">说明</span><span class="sxs-lookup"><span data-stu-id="be585-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="be585-113">Get</span><span class="sxs-lookup"><span data-stu-id="be585-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="be585-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="be585-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="be585-115">读取**identitySecurityDefaultsEnforcementPolicy**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be585-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="be585-116">更新</span><span class="sxs-lookup"><span data-stu-id="be585-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="be585-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="be585-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="be585-118">更新**identitySecurityDefaultsEnforcementPolicy**对象。</span><span class="sxs-lookup"><span data-stu-id="be585-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="be585-119">属性</span><span class="sxs-lookup"><span data-stu-id="be585-119">Properties</span></span>

| <span data-ttu-id="be585-120">属性</span><span class="sxs-lookup"><span data-stu-id="be585-120">Property</span></span>     | <span data-ttu-id="be585-121">类型</span><span class="sxs-lookup"><span data-stu-id="be585-121">Type</span></span>        | <span data-ttu-id="be585-122">说明</span><span class="sxs-lookup"><span data-stu-id="be585-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="be585-123">说明</span><span class="sxs-lookup"><span data-stu-id="be585-123">description</span></span>|<span data-ttu-id="be585-124">String</span><span class="sxs-lookup"><span data-stu-id="be585-124">String</span></span>|<span data-ttu-id="be585-125">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="be585-125">Description for this policy.</span></span> <span data-ttu-id="be585-126">只读。</span><span class="sxs-lookup"><span data-stu-id="be585-126">Read-only.</span></span>|
|<span data-ttu-id="be585-127">displayName</span><span class="sxs-lookup"><span data-stu-id="be585-127">displayName</span></span>|<span data-ttu-id="be585-128">String</span><span class="sxs-lookup"><span data-stu-id="be585-128">String</span></span>|<span data-ttu-id="be585-129">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be585-129">Display name for this policy.</span></span> <span data-ttu-id="be585-130">只读。</span><span class="sxs-lookup"><span data-stu-id="be585-130">Read-only.</span></span>|
|<span data-ttu-id="be585-131">id</span><span class="sxs-lookup"><span data-stu-id="be585-131">id</span></span>|<span data-ttu-id="be585-132">字符串</span><span class="sxs-lookup"><span data-stu-id="be585-132">String</span></span>|<span data-ttu-id="be585-133">此策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="be585-133">Identifier for this policy.</span></span> <span data-ttu-id="be585-134">只读。</span><span class="sxs-lookup"><span data-stu-id="be585-134">Read-only.</span></span>|
|<span data-ttu-id="be585-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="be585-135">isEnabled</span></span>|<span data-ttu-id="be585-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="be585-136">Boolean</span></span>|<span data-ttu-id="be585-137">如果设置为 true，则会为租户启用 Azure Active Directory 安全性默认设置。</span><span class="sxs-lookup"><span data-stu-id="be585-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be585-138">关系</span><span class="sxs-lookup"><span data-stu-id="be585-138">Relationships</span></span>

<span data-ttu-id="be585-139">无。</span><span class="sxs-lookup"><span data-stu-id="be585-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be585-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be585-140">JSON representation</span></span>

<span data-ttu-id="be585-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be585-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySecurityDefaultsEnforcementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
