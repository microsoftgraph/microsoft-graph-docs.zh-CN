---
title: unifiedRoleManagementPolicyRule 资源类型
description: unifiedRoleManagementPolicyRule 指定与角色管理策略关联的规则。 它是抽象的。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 420ebfca11d2873ad942782fb8e7d97e893b7185
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299123"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a><span data-ttu-id="44232-104">unifiedRoleManagementPolicyRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="44232-104">unifiedRoleManagementPolicyRule resource type</span></span>

<span data-ttu-id="44232-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44232-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44232-106">unifiedRoleManagementPolicyRule 指定与角色管理策略关联的规则。</span><span class="sxs-lookup"><span data-stu-id="44232-106">A unifiedRoleManagementPolicyRule specifies the rule associated with a role management policy.</span></span> <span data-ttu-id="44232-107">它是抽象的。</span><span class="sxs-lookup"><span data-stu-id="44232-107">It is abstract.</span></span>

## <a name="methods"></a><span data-ttu-id="44232-108">方法</span><span class="sxs-lookup"><span data-stu-id="44232-108">Methods</span></span>
|<span data-ttu-id="44232-109">方法</span><span class="sxs-lookup"><span data-stu-id="44232-109">Method</span></span>|<span data-ttu-id="44232-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="44232-110">Return type</span></span>|<span data-ttu-id="44232-111">说明</span><span class="sxs-lookup"><span data-stu-id="44232-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44232-112">列出 unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="44232-112">List unifiedRoleManagementPolicyRules</span></span>](../api/unifiedrolemanagementpolicyrule-list.md)|<span data-ttu-id="44232-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="44232-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="44232-114">获取 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="44232-114">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>|
|[<span data-ttu-id="44232-115">获取 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="44232-115">Get unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-get.md)|[<span data-ttu-id="44232-116">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="44232-116">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="44232-117">读取 [unifiedRoleManagementPolicyRule 对象的属性和](../resources/unifiedrolemanagementpolicyrule.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="44232-117">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|
|[<span data-ttu-id="44232-118">更新 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="44232-118">Update unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-update.md)|[<span data-ttu-id="44232-119">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="44232-119">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="44232-120">更新 [unifiedRoleManagementPolicyRule 对象](../resources/unifiedrolemanagementpolicyrule.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="44232-120">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44232-121">属性</span><span class="sxs-lookup"><span data-stu-id="44232-121">Properties</span></span>
|<span data-ttu-id="44232-122">属性</span><span class="sxs-lookup"><span data-stu-id="44232-122">Property</span></span>|<span data-ttu-id="44232-123">类型</span><span class="sxs-lookup"><span data-stu-id="44232-123">Type</span></span>|<span data-ttu-id="44232-124">说明</span><span class="sxs-lookup"><span data-stu-id="44232-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44232-125">id</span><span class="sxs-lookup"><span data-stu-id="44232-125">id</span></span>|<span data-ttu-id="44232-126">String</span><span class="sxs-lookup"><span data-stu-id="44232-126">String</span></span>|<span data-ttu-id="44232-127">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="44232-127">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="44232-128">target</span><span class="sxs-lookup"><span data-stu-id="44232-128">target</span></span>|[<span data-ttu-id="44232-129">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="44232-129">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="44232-130">策略规则的目标。</span><span class="sxs-lookup"><span data-stu-id="44232-130">The target for the policy rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44232-131">关系</span><span class="sxs-lookup"><span data-stu-id="44232-131">Relationships</span></span>
<span data-ttu-id="44232-132">无。</span><span class="sxs-lookup"><span data-stu-id="44232-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44232-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44232-133">JSON representation</span></span>
<span data-ttu-id="44232-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44232-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```

