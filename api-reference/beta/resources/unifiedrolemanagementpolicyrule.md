---
title: unifiedRoleManagementPolicyRule 资源类型
description: unifiedRoleManagementPolicyRule 指定与角色管理策略关联的规则。 它是抽象的。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa0bc719fe4722692b1ff42861cccede7150780d
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682241"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a><span data-ttu-id="c09f1-104">unifiedRoleManagementPolicyRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c09f1-104">unifiedRoleManagementPolicyRule resource type</span></span>

<span data-ttu-id="c09f1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c09f1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c09f1-106">unifiedRoleManagementPolicyRule 指定与角色管理策略关联的规则。</span><span class="sxs-lookup"><span data-stu-id="c09f1-106">A unifiedRoleManagementPolicyRule specifies the rule associated with a role management policy.</span></span> <span data-ttu-id="c09f1-107">它是抽象的。</span><span class="sxs-lookup"><span data-stu-id="c09f1-107">It is abstract.</span></span>

## <a name="methods"></a><span data-ttu-id="c09f1-108">方法</span><span class="sxs-lookup"><span data-stu-id="c09f1-108">Methods</span></span>
|<span data-ttu-id="c09f1-109">方法</span><span class="sxs-lookup"><span data-stu-id="c09f1-109">Method</span></span>|<span data-ttu-id="c09f1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c09f1-110">Return type</span></span>|<span data-ttu-id="c09f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="c09f1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c09f1-112">列出 unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="c09f1-112">List unifiedRoleManagementPolicyRules</span></span>](../api/unifiedrolemanagementpolicyrule-list.md)|<span data-ttu-id="c09f1-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c09f1-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="c09f1-114">获取 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c09f1-114">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c09f1-115">获取 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c09f1-115">Get unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-get.md)|[<span data-ttu-id="c09f1-116">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c09f1-116">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="c09f1-117">读取 [unifiedRoleManagementPolicyRule 对象的属性和](../resources/unifiedrolemanagementpolicyrule.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c09f1-117">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|
|[<span data-ttu-id="c09f1-118">更新 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c09f1-118">Update unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-update.md)|[<span data-ttu-id="c09f1-119">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c09f1-119">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="c09f1-120">更新 [unifiedRoleManagementPolicyRule 对象](../resources/unifiedrolemanagementpolicyrule.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c09f1-120">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c09f1-121">属性</span><span class="sxs-lookup"><span data-stu-id="c09f1-121">Properties</span></span>
|<span data-ttu-id="c09f1-122">属性</span><span class="sxs-lookup"><span data-stu-id="c09f1-122">Property</span></span>|<span data-ttu-id="c09f1-123">类型</span><span class="sxs-lookup"><span data-stu-id="c09f1-123">Type</span></span>|<span data-ttu-id="c09f1-124">说明</span><span class="sxs-lookup"><span data-stu-id="c09f1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c09f1-125">id</span><span class="sxs-lookup"><span data-stu-id="c09f1-125">id</span></span>|<span data-ttu-id="c09f1-126">String</span><span class="sxs-lookup"><span data-stu-id="c09f1-126">String</span></span>|<span data-ttu-id="c09f1-127">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c09f1-127">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="c09f1-128">target</span><span class="sxs-lookup"><span data-stu-id="c09f1-128">target</span></span>|[<span data-ttu-id="c09f1-129">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="c09f1-129">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="c09f1-130">策略规则的目标。</span><span class="sxs-lookup"><span data-stu-id="c09f1-130">The target for the policy rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c09f1-131">关系</span><span class="sxs-lookup"><span data-stu-id="c09f1-131">Relationships</span></span>
<span data-ttu-id="c09f1-132">无。</span><span class="sxs-lookup"><span data-stu-id="c09f1-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c09f1-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c09f1-133">JSON representation</span></span>
<span data-ttu-id="c09f1-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c09f1-134">The following is a JSON representation of the resource.</span></span>
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

