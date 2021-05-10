---
title: unifiedRoleManagementPolicyApprovalRule 资源类型
description: unifiedRoleManagementPolicyApprovalRule 指定与角色管理策略关联的审批规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a23087bada876a76658e616add68e404635461f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299189"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a><span data-ttu-id="1bfaa-104">unifiedRoleManagementPolicyApprovalRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="1bfaa-104">unifiedRoleManagementPolicyApprovalRule resource type</span></span>

<span data-ttu-id="1bfaa-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bfaa-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bfaa-106">unifiedRoleManagementPolicyApprovalRule 指定与角色管理策略关联的审批规则。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-106">A unifiedRoleManagementPolicyApprovalRule specifies the approval rule associated with a role management policy.</span></span> <span data-ttu-id="1bfaa-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="1bfaa-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1bfaa-109">属性</span><span class="sxs-lookup"><span data-stu-id="1bfaa-109">Properties</span></span>
|<span data-ttu-id="1bfaa-110">属性</span><span class="sxs-lookup"><span data-stu-id="1bfaa-110">Property</span></span>|<span data-ttu-id="1bfaa-111">类型</span><span class="sxs-lookup"><span data-stu-id="1bfaa-111">Type</span></span>|<span data-ttu-id="1bfaa-112">说明</span><span class="sxs-lookup"><span data-stu-id="1bfaa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bfaa-113">id</span><span class="sxs-lookup"><span data-stu-id="1bfaa-113">id</span></span>|<span data-ttu-id="1bfaa-114">String</span><span class="sxs-lookup"><span data-stu-id="1bfaa-114">String</span></span>|<span data-ttu-id="1bfaa-115">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-115">Unique identifier for the rule.</span></span> <span data-ttu-id="1bfaa-116">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="1bfaa-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="1bfaa-117">setting</span><span class="sxs-lookup"><span data-stu-id="1bfaa-117">setting</span></span>|[<span data-ttu-id="1bfaa-118">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="1bfaa-118">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="1bfaa-119">规则的审批设置。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-119">The approval setting for the rule.</span></span>|
|<span data-ttu-id="1bfaa-120">target</span><span class="sxs-lookup"><span data-stu-id="1bfaa-120">target</span></span>|[<span data-ttu-id="1bfaa-121">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="1bfaa-121">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="1bfaa-122">规则规则的目标。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-122">The target for the rule rule.</span></span> <span data-ttu-id="1bfaa-123">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="1bfaa-123">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bfaa-124">关系</span><span class="sxs-lookup"><span data-stu-id="1bfaa-124">Relationships</span></span>
<span data-ttu-id="1bfaa-125">无。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bfaa-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1bfaa-126">JSON representation</span></span>
<span data-ttu-id="1bfaa-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bfaa-127">The following is a JSON representation of the resource.</span></span>
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

