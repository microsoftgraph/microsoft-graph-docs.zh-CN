---
title: unifiedRoleManagementPolicyEnablementRule 资源类型
description: unifiedRoleManagementPolicyEnablementRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2cb5770f2fdd50aaf5e82d7c1f8fba505a47151
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299187"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a><span data-ttu-id="13756-104">unifiedRoleManagementPolicyEnablementRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="13756-104">unifiedRoleManagementPolicyEnablementRule resource type</span></span>

<span data-ttu-id="13756-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13756-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13756-106">unifiedRoleManagementPolicyEnablementRule 指定与角色管理策略关联的启用规则。</span><span class="sxs-lookup"><span data-stu-id="13756-106">A unifiedRoleManagementPolicyEnablementRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="13756-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="13756-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="13756-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="13756-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="13756-109">属性</span><span class="sxs-lookup"><span data-stu-id="13756-109">Properties</span></span>
|<span data-ttu-id="13756-110">属性</span><span class="sxs-lookup"><span data-stu-id="13756-110">Property</span></span>|<span data-ttu-id="13756-111">类型</span><span class="sxs-lookup"><span data-stu-id="13756-111">Type</span></span>|<span data-ttu-id="13756-112">说明</span><span class="sxs-lookup"><span data-stu-id="13756-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13756-113">enabledRules</span><span class="sxs-lookup"><span data-stu-id="13756-113">enabledRules</span></span>|<span data-ttu-id="13756-114">String collection</span><span class="sxs-lookup"><span data-stu-id="13756-114">String collection</span></span>|<span data-ttu-id="13756-115">启用的规则。</span><span class="sxs-lookup"><span data-stu-id="13756-115">The rules which are enabled.</span></span> <span data-ttu-id="13756-116">允许的值包括 MultifactorAuthentication、Justification、Ticketing。</span><span class="sxs-lookup"><span data-stu-id="13756-116">Allowed values are MultifactorAuthentication, Justification, Ticketing.</span></span>|
|<span data-ttu-id="13756-117">id</span><span class="sxs-lookup"><span data-stu-id="13756-117">id</span></span>|<span data-ttu-id="13756-118">String</span><span class="sxs-lookup"><span data-stu-id="13756-118">String</span></span>|<span data-ttu-id="13756-119">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="13756-119">Unique identifier for the rule.</span></span> <span data-ttu-id="13756-120">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="13756-120">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="13756-121">target</span><span class="sxs-lookup"><span data-stu-id="13756-121">target</span></span>|[<span data-ttu-id="13756-122">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="13756-122">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="13756-123">规则的目标。</span><span class="sxs-lookup"><span data-stu-id="13756-123">The target for the rule.</span></span> <span data-ttu-id="13756-124">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="13756-124">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="13756-125">关系</span><span class="sxs-lookup"><span data-stu-id="13756-125">Relationships</span></span>
<span data-ttu-id="13756-126">无。</span><span class="sxs-lookup"><span data-stu-id="13756-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13756-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13756-127">JSON representation</span></span>
<span data-ttu-id="13756-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13756-128">The following is a JSON representation of the resource.</span></span>
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

