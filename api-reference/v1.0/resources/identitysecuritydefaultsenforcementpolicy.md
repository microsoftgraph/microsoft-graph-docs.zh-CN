---
title: identitySecurityDefaultsEnforcementPolicy 资源类型
description: 表示 Azure Active Directory 安全默认值策略。 安全默认值包含预配置的安全设置，可抵御常见攻击。
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2609a75ad90aba9ab545e81207bc0d3ea33f0a8a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944841"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="7e8b0-104">identitySecurityDefaultsEnforcementPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e8b0-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="7e8b0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e8b0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e8b0-106">表示 Azure Active Directory [安全默认值](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 策略。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="7e8b0-107">安全默认值包含预配置的安全设置，可抵御常见攻击。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="7e8b0-108">继承自 [policyBase](../resources/policybase.md)。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7e8b0-109">Methods</span><span class="sxs-lookup"><span data-stu-id="7e8b0-109">Methods</span></span>

| <span data-ttu-id="7e8b0-110">方法</span><span class="sxs-lookup"><span data-stu-id="7e8b0-110">Method</span></span>       | <span data-ttu-id="7e8b0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e8b0-111">Return Type</span></span> | <span data-ttu-id="7e8b0-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e8b0-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7e8b0-113">获取</span><span class="sxs-lookup"><span data-stu-id="7e8b0-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="7e8b0-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="7e8b0-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="7e8b0-115">读取 **identitySecurityDefaultsEnforcementPolicy 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="7e8b0-116">更新</span><span class="sxs-lookup"><span data-stu-id="7e8b0-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="7e8b0-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="7e8b0-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="7e8b0-118">更新 **identitySecurityDefaultsEnforcementPolicy** 对象。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e8b0-119">属性</span><span class="sxs-lookup"><span data-stu-id="7e8b0-119">Properties</span></span>

| <span data-ttu-id="7e8b0-120">属性</span><span class="sxs-lookup"><span data-stu-id="7e8b0-120">Property</span></span>     | <span data-ttu-id="7e8b0-121">类型</span><span class="sxs-lookup"><span data-stu-id="7e8b0-121">Type</span></span>        | <span data-ttu-id="7e8b0-122">说明</span><span class="sxs-lookup"><span data-stu-id="7e8b0-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7e8b0-123">说明</span><span class="sxs-lookup"><span data-stu-id="7e8b0-123">description</span></span>|<span data-ttu-id="7e8b0-124">String</span><span class="sxs-lookup"><span data-stu-id="7e8b0-124">String</span></span>|<span data-ttu-id="7e8b0-125">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-125">Description for this policy.</span></span> <span data-ttu-id="7e8b0-126">只读。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-126">Read-only.</span></span>|
|<span data-ttu-id="7e8b0-127">displayName</span><span class="sxs-lookup"><span data-stu-id="7e8b0-127">displayName</span></span>|<span data-ttu-id="7e8b0-128">String</span><span class="sxs-lookup"><span data-stu-id="7e8b0-128">String</span></span>|<span data-ttu-id="7e8b0-129">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-129">Display name for this policy.</span></span> <span data-ttu-id="7e8b0-130">只读。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-130">Read-only.</span></span>|
|<span data-ttu-id="7e8b0-131">id</span><span class="sxs-lookup"><span data-stu-id="7e8b0-131">id</span></span>|<span data-ttu-id="7e8b0-132">String</span><span class="sxs-lookup"><span data-stu-id="7e8b0-132">String</span></span>|<span data-ttu-id="7e8b0-133">此策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-133">Identifier for this policy.</span></span> <span data-ttu-id="7e8b0-134">只读。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-134">Read-only.</span></span>|
|<span data-ttu-id="7e8b0-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7e8b0-135">isEnabled</span></span>|<span data-ttu-id="7e8b0-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e8b0-136">Boolean</span></span>|<span data-ttu-id="7e8b0-137">如果设置为 `true` ，则为租户启用 Azure Active Directory 安全默认值。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-137">If set to `true`, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e8b0-138">关系</span><span class="sxs-lookup"><span data-stu-id="7e8b0-138">Relationships</span></span>

<span data-ttu-id="7e8b0-139">无。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e8b0-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e8b0-140">JSON representation</span></span>

<span data-ttu-id="7e8b0-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e8b0-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
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
