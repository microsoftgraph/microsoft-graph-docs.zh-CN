---
title: unifiedRoleManagementPolicyAuthenticationContextRule 资源类型
description: unifiedRoleManagementPolicyAuthenticationContextRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5e3db8812b58b8276ab2fdd977e110f30a874c9b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680694"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a><span data-ttu-id="89f8f-104">unifiedRoleManagementPolicyAuthenticationContextRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="89f8f-104">unifiedRoleManagementPolicyAuthenticationContextRule resource type</span></span>

<span data-ttu-id="89f8f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f8f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89f8f-106">unifiedRoleManagementPolicyAuthenticationContextRule 指定与角色管理策略关联的启用规则。</span><span class="sxs-lookup"><span data-stu-id="89f8f-106">A unifiedRoleManagementPolicyAuthenticationContextRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="89f8f-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="89f8f-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="89f8f-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="89f8f-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="89f8f-109">属性</span><span class="sxs-lookup"><span data-stu-id="89f8f-109">Properties</span></span>
|<span data-ttu-id="89f8f-110">属性</span><span class="sxs-lookup"><span data-stu-id="89f8f-110">Property</span></span>|<span data-ttu-id="89f8f-111">类型</span><span class="sxs-lookup"><span data-stu-id="89f8f-111">Type</span></span>|<span data-ttu-id="89f8f-112">说明</span><span class="sxs-lookup"><span data-stu-id="89f8f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f8f-113">claimValue</span><span class="sxs-lookup"><span data-stu-id="89f8f-113">claimValue</span></span>|<span data-ttu-id="89f8f-114">String</span><span class="sxs-lookup"><span data-stu-id="89f8f-114">String</span></span>|<span data-ttu-id="89f8f-115">身份验证上下文声明的值。</span><span class="sxs-lookup"><span data-stu-id="89f8f-115">Value of the authentication context claim.</span></span>|
|<span data-ttu-id="89f8f-116">id</span><span class="sxs-lookup"><span data-stu-id="89f8f-116">id</span></span>|<span data-ttu-id="89f8f-117">String</span><span class="sxs-lookup"><span data-stu-id="89f8f-117">String</span></span>|<span data-ttu-id="89f8f-118">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="89f8f-118">Unique identifier for the rule.</span></span> <span data-ttu-id="89f8f-119">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="89f8f-119">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="89f8f-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="89f8f-120">isEnabled</span></span>|<span data-ttu-id="89f8f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f8f-121">Boolean</span></span>|<span data-ttu-id="89f8f-122">指示设置是否已启用。</span><span class="sxs-lookup"><span data-stu-id="89f8f-122">Indicates if the setting is enabled.</span></span>|
|<span data-ttu-id="89f8f-123">target</span><span class="sxs-lookup"><span data-stu-id="89f8f-123">target</span></span>|[<span data-ttu-id="89f8f-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="89f8f-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="89f8f-125">规则的目标。</span><span class="sxs-lookup"><span data-stu-id="89f8f-125">The target for the rule.</span></span> <span data-ttu-id="89f8f-126">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="89f8f-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f8f-127">关系</span><span class="sxs-lookup"><span data-stu-id="89f8f-127">Relationships</span></span>
<span data-ttu-id="89f8f-128">无。</span><span class="sxs-lookup"><span data-stu-id="89f8f-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f8f-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89f8f-129">JSON representation</span></span>
<span data-ttu-id="89f8f-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89f8f-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

