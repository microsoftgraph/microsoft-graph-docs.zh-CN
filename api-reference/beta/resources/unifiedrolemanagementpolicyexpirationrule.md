---
title: unifiedRoleManagementPolicyExpirationRule 资源类型
description: unifiedRoleManagementPolicyExpirationRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 610ecd2e861ac672d0b211e313132caa6946d8ff
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299186"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a><span data-ttu-id="3d0b2-104">unifiedRoleManagementPolicyExpirationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d0b2-104">unifiedRoleManagementPolicyExpirationRule resource type</span></span>

<span data-ttu-id="3d0b2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d0b2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d0b2-106">unifiedRoleManagementPolicyExpirationRule 指定与角色管理策略关联的启用规则。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-106">A unifiedRoleManagementPolicyExpirationRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="3d0b2-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="3d0b2-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3d0b2-109">属性</span><span class="sxs-lookup"><span data-stu-id="3d0b2-109">Properties</span></span>
|<span data-ttu-id="3d0b2-110">属性</span><span class="sxs-lookup"><span data-stu-id="3d0b2-110">Property</span></span>|<span data-ttu-id="3d0b2-111">类型</span><span class="sxs-lookup"><span data-stu-id="3d0b2-111">Type</span></span>|<span data-ttu-id="3d0b2-112">说明</span><span class="sxs-lookup"><span data-stu-id="3d0b2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d0b2-113">id</span><span class="sxs-lookup"><span data-stu-id="3d0b2-113">id</span></span>|<span data-ttu-id="3d0b2-114">String</span><span class="sxs-lookup"><span data-stu-id="3d0b2-114">String</span></span>|<span data-ttu-id="3d0b2-115">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-115">Unique identifier for the rule.</span></span> <span data-ttu-id="3d0b2-116">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="3d0b2-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="3d0b2-117">isExpirationRequired</span><span class="sxs-lookup"><span data-stu-id="3d0b2-117">isExpirationRequired</span></span>|<span data-ttu-id="3d0b2-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0b2-118">Boolean</span></span>|<span data-ttu-id="3d0b2-119">指示资格或分配是否要求过期。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-119">Indicates if expiration is required for eligibility or assignment.</span></span>|
|<span data-ttu-id="3d0b2-120">maximumDuration</span><span class="sxs-lookup"><span data-stu-id="3d0b2-120">maximumDuration</span></span>|<span data-ttu-id="3d0b2-121">期限</span><span class="sxs-lookup"><span data-stu-id="3d0b2-121">Duration</span></span>|<span data-ttu-id="3d0b2-122">符合条件的或非永久性分配所允许的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-122">The maximum duration allowed for eligiblity or assignment which is not permanent.</span></span>|
|<span data-ttu-id="3d0b2-123">target</span><span class="sxs-lookup"><span data-stu-id="3d0b2-123">target</span></span>|[<span data-ttu-id="3d0b2-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="3d0b2-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="3d0b2-125">规则的目标。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-125">The target for the rule.</span></span> <span data-ttu-id="3d0b2-126">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="3d0b2-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d0b2-127">关系</span><span class="sxs-lookup"><span data-stu-id="3d0b2-127">Relationships</span></span>
<span data-ttu-id="3d0b2-128">无。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d0b2-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d0b2-129">JSON representation</span></span>
<span data-ttu-id="3d0b2-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d0b2-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

