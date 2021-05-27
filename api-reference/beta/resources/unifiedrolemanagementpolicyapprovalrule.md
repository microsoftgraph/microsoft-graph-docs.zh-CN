---
title: unifiedRoleManagementPolicyApprovalRule 资源类型
description: unifiedRoleManagementPolicyApprovalRule 指定与角色管理策略关联的审批规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 41d9cac01f48d8dcdd59513718053611b023a3a8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680701"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a><span data-ttu-id="b11c5-104">unifiedRoleManagementPolicyApprovalRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="b11c5-104">unifiedRoleManagementPolicyApprovalRule resource type</span></span>

<span data-ttu-id="b11c5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b11c5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b11c5-106">unifiedRoleManagementPolicyApprovalRule 指定与角色管理策略关联的审批规则。</span><span class="sxs-lookup"><span data-stu-id="b11c5-106">A unifiedRoleManagementPolicyApprovalRule specifies the approval rule associated with a role management policy.</span></span> <span data-ttu-id="b11c5-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="b11c5-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="b11c5-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="b11c5-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b11c5-109">属性</span><span class="sxs-lookup"><span data-stu-id="b11c5-109">Properties</span></span>
|<span data-ttu-id="b11c5-110">属性</span><span class="sxs-lookup"><span data-stu-id="b11c5-110">Property</span></span>|<span data-ttu-id="b11c5-111">类型</span><span class="sxs-lookup"><span data-stu-id="b11c5-111">Type</span></span>|<span data-ttu-id="b11c5-112">说明</span><span class="sxs-lookup"><span data-stu-id="b11c5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11c5-113">id</span><span class="sxs-lookup"><span data-stu-id="b11c5-113">id</span></span>|<span data-ttu-id="b11c5-114">String</span><span class="sxs-lookup"><span data-stu-id="b11c5-114">String</span></span>|<span data-ttu-id="b11c5-115">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b11c5-115">Unique identifier for the rule.</span></span> <span data-ttu-id="b11c5-116">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b11c5-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="b11c5-117">setting</span><span class="sxs-lookup"><span data-stu-id="b11c5-117">setting</span></span>|[<span data-ttu-id="b11c5-118">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="b11c5-118">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="b11c5-119">规则的审批设置。</span><span class="sxs-lookup"><span data-stu-id="b11c5-119">The approval setting for the rule.</span></span>|
|<span data-ttu-id="b11c5-120">target</span><span class="sxs-lookup"><span data-stu-id="b11c5-120">target</span></span>|[<span data-ttu-id="b11c5-121">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="b11c5-121">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="b11c5-122">规则规则的目标。</span><span class="sxs-lookup"><span data-stu-id="b11c5-122">The target for the rule rule.</span></span> <span data-ttu-id="b11c5-123">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b11c5-123">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b11c5-124">关系</span><span class="sxs-lookup"><span data-stu-id="b11c5-124">Relationships</span></span>
<span data-ttu-id="b11c5-125">无。</span><span class="sxs-lookup"><span data-stu-id="b11c5-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b11c5-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b11c5-126">JSON representation</span></span>
<span data-ttu-id="b11c5-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b11c5-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "setting": {
    "@odata.type": "microsoft.graph.approvalSettings"
  }
}
```

