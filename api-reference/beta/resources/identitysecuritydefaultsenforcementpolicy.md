---
title: identitySecurityDefaultsEnforcementPolicy 资源类型
description: 表示 Azure Active Directory 安全默认策略。 安全默认设置包含防止常见攻击的预配置安全设置。
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dea4d94dfc8de8310410498fdf8d83c2a5e8f68
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154927"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="b700f-104">identitySecurityDefaultsEnforcementPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="b700f-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="b700f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b700f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b700f-106">表示 Azure Active Directory [安全默认](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 策略。</span><span class="sxs-lookup"><span data-stu-id="b700f-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="b700f-107">安全默认设置包含防止常见攻击的预配置安全设置。</span><span class="sxs-lookup"><span data-stu-id="b700f-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="b700f-108">继承自 [policyBase](../resources/policybase.md)。</span><span class="sxs-lookup"><span data-stu-id="b700f-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b700f-109">方法</span><span class="sxs-lookup"><span data-stu-id="b700f-109">Methods</span></span>

| <span data-ttu-id="b700f-110">方法</span><span class="sxs-lookup"><span data-stu-id="b700f-110">Method</span></span>       | <span data-ttu-id="b700f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b700f-111">Return Type</span></span> | <span data-ttu-id="b700f-112">说明</span><span class="sxs-lookup"><span data-stu-id="b700f-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b700f-113">Get</span><span class="sxs-lookup"><span data-stu-id="b700f-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="b700f-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b700f-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="b700f-115">读取 **identitySecurityDefaultsEnforcementPolicy 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="b700f-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="b700f-116">更新</span><span class="sxs-lookup"><span data-stu-id="b700f-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="b700f-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b700f-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="b700f-118">更新 **identitySecurityDefaultsEnforcementPolicy** 对象。</span><span class="sxs-lookup"><span data-stu-id="b700f-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b700f-119">属性</span><span class="sxs-lookup"><span data-stu-id="b700f-119">Properties</span></span>

| <span data-ttu-id="b700f-120">属性</span><span class="sxs-lookup"><span data-stu-id="b700f-120">Property</span></span>     | <span data-ttu-id="b700f-121">类型</span><span class="sxs-lookup"><span data-stu-id="b700f-121">Type</span></span>        | <span data-ttu-id="b700f-122">说明</span><span class="sxs-lookup"><span data-stu-id="b700f-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b700f-123">说明</span><span class="sxs-lookup"><span data-stu-id="b700f-123">description</span></span>|<span data-ttu-id="b700f-124">String</span><span class="sxs-lookup"><span data-stu-id="b700f-124">String</span></span>|<span data-ttu-id="b700f-125">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b700f-125">Description for this policy.</span></span> <span data-ttu-id="b700f-126">只读。</span><span class="sxs-lookup"><span data-stu-id="b700f-126">Read-only.</span></span>|
|<span data-ttu-id="b700f-127">displayName</span><span class="sxs-lookup"><span data-stu-id="b700f-127">displayName</span></span>|<span data-ttu-id="b700f-128">String</span><span class="sxs-lookup"><span data-stu-id="b700f-128">String</span></span>|<span data-ttu-id="b700f-129">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b700f-129">Display name for this policy.</span></span> <span data-ttu-id="b700f-130">只读。</span><span class="sxs-lookup"><span data-stu-id="b700f-130">Read-only.</span></span>|
|<span data-ttu-id="b700f-131">id</span><span class="sxs-lookup"><span data-stu-id="b700f-131">id</span></span>|<span data-ttu-id="b700f-132">String</span><span class="sxs-lookup"><span data-stu-id="b700f-132">String</span></span>|<span data-ttu-id="b700f-133">此策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="b700f-133">Identifier for this policy.</span></span> <span data-ttu-id="b700f-134">只读。</span><span class="sxs-lookup"><span data-stu-id="b700f-134">Read-only.</span></span>|
|<span data-ttu-id="b700f-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b700f-135">isEnabled</span></span>|<span data-ttu-id="b700f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="b700f-136">Boolean</span></span>|<span data-ttu-id="b700f-137">如果设置为 true，则为租户启用 Azure Active Directory 安全默认值。</span><span class="sxs-lookup"><span data-stu-id="b700f-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b700f-138">关系</span><span class="sxs-lookup"><span data-stu-id="b700f-138">Relationships</span></span>

<span data-ttu-id="b700f-139">无。</span><span class="sxs-lookup"><span data-stu-id="b700f-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b700f-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b700f-140">JSON representation</span></span>

<span data-ttu-id="b700f-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b700f-141">The following is a JSON representation of the resource.</span></span>

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