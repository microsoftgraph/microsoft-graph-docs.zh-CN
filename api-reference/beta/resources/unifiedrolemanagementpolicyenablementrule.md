---
title: unifiedRoleManagementPolicyEnablementRule 资源类型
description: unifiedRoleManagementPolicyEnablementRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf3ef8e25026c72aab36a9c2fb6241f5bef950da
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680680"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a><span data-ttu-id="543eb-104">unifiedRoleManagementPolicyEnablementRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="543eb-104">unifiedRoleManagementPolicyEnablementRule resource type</span></span>

<span data-ttu-id="543eb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="543eb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="543eb-106">unifiedRoleManagementPolicyEnablementRule 指定与角色管理策略关联的启用规则。</span><span class="sxs-lookup"><span data-stu-id="543eb-106">A unifiedRoleManagementPolicyEnablementRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="543eb-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="543eb-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="543eb-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="543eb-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="543eb-109">属性</span><span class="sxs-lookup"><span data-stu-id="543eb-109">Properties</span></span>
|<span data-ttu-id="543eb-110">属性</span><span class="sxs-lookup"><span data-stu-id="543eb-110">Property</span></span>|<span data-ttu-id="543eb-111">类型</span><span class="sxs-lookup"><span data-stu-id="543eb-111">Type</span></span>|<span data-ttu-id="543eb-112">说明</span><span class="sxs-lookup"><span data-stu-id="543eb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="543eb-113">enabledRules</span><span class="sxs-lookup"><span data-stu-id="543eb-113">enabledRules</span></span>|<span data-ttu-id="543eb-114">String collection</span><span class="sxs-lookup"><span data-stu-id="543eb-114">String collection</span></span>|<span data-ttu-id="543eb-115">启用的规则。</span><span class="sxs-lookup"><span data-stu-id="543eb-115">The rules which are enabled.</span></span> <span data-ttu-id="543eb-116">允许的值包括 MultifactorAuthentication、Justification、Ticketing。</span><span class="sxs-lookup"><span data-stu-id="543eb-116">Allowed values are MultifactorAuthentication, Justification, Ticketing.</span></span>|
|<span data-ttu-id="543eb-117">id</span><span class="sxs-lookup"><span data-stu-id="543eb-117">id</span></span>|<span data-ttu-id="543eb-118">String</span><span class="sxs-lookup"><span data-stu-id="543eb-118">String</span></span>|<span data-ttu-id="543eb-119">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="543eb-119">Unique identifier for the rule.</span></span> <span data-ttu-id="543eb-120">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="543eb-120">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="543eb-121">target</span><span class="sxs-lookup"><span data-stu-id="543eb-121">target</span></span>|[<span data-ttu-id="543eb-122">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="543eb-122">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="543eb-123">规则的目标。</span><span class="sxs-lookup"><span data-stu-id="543eb-123">The target for the rule.</span></span> <span data-ttu-id="543eb-124">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="543eb-124">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="543eb-125">关系</span><span class="sxs-lookup"><span data-stu-id="543eb-125">Relationships</span></span>
<span data-ttu-id="543eb-126">无。</span><span class="sxs-lookup"><span data-stu-id="543eb-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="543eb-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="543eb-127">JSON representation</span></span>
<span data-ttu-id="543eb-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="543eb-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

