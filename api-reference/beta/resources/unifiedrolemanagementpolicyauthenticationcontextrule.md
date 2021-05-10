---
title: unifiedRoleManagementPolicyAuthenticationContextRule 资源类型
description: unifiedRoleManagementPolicyAuthenticationContextRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6c9eb94272dcc7e9cbbe27657b50d50688ac9d9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299188"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a><span data-ttu-id="51bd3-104">unifiedRoleManagementPolicyAuthenticationContextRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="51bd3-104">unifiedRoleManagementPolicyAuthenticationContextRule resource type</span></span>

<span data-ttu-id="51bd3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51bd3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51bd3-106">unifiedRoleManagementPolicyAuthenticationContextRule 指定与角色管理策略关联的启用规则。</span><span class="sxs-lookup"><span data-stu-id="51bd3-106">A unifiedRoleManagementPolicyAuthenticationContextRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="51bd3-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="51bd3-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="51bd3-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="51bd3-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="51bd3-109">属性</span><span class="sxs-lookup"><span data-stu-id="51bd3-109">Properties</span></span>
|<span data-ttu-id="51bd3-110">属性</span><span class="sxs-lookup"><span data-stu-id="51bd3-110">Property</span></span>|<span data-ttu-id="51bd3-111">类型</span><span class="sxs-lookup"><span data-stu-id="51bd3-111">Type</span></span>|<span data-ttu-id="51bd3-112">说明</span><span class="sxs-lookup"><span data-stu-id="51bd3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51bd3-113">claimValue</span><span class="sxs-lookup"><span data-stu-id="51bd3-113">claimValue</span></span>|<span data-ttu-id="51bd3-114">String</span><span class="sxs-lookup"><span data-stu-id="51bd3-114">String</span></span>|<span data-ttu-id="51bd3-115">身份验证上下文声明的值。</span><span class="sxs-lookup"><span data-stu-id="51bd3-115">Value of the authentication context claim.</span></span>|
|<span data-ttu-id="51bd3-116">id</span><span class="sxs-lookup"><span data-stu-id="51bd3-116">id</span></span>|<span data-ttu-id="51bd3-117">String</span><span class="sxs-lookup"><span data-stu-id="51bd3-117">String</span></span>|<span data-ttu-id="51bd3-118">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="51bd3-118">Unique identifier for the rule.</span></span> <span data-ttu-id="51bd3-119">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="51bd3-119">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="51bd3-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="51bd3-120">isEnabled</span></span>|<span data-ttu-id="51bd3-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="51bd3-121">Boolean</span></span>|<span data-ttu-id="51bd3-122">指示设置是否已启用。</span><span class="sxs-lookup"><span data-stu-id="51bd3-122">Indicates if the setting is enabled.</span></span>|
|<span data-ttu-id="51bd3-123">target</span><span class="sxs-lookup"><span data-stu-id="51bd3-123">target</span></span>|[<span data-ttu-id="51bd3-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="51bd3-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="51bd3-125">规则的目标。</span><span class="sxs-lookup"><span data-stu-id="51bd3-125">The target for the rule.</span></span> <span data-ttu-id="51bd3-126">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="51bd3-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="51bd3-127">关系</span><span class="sxs-lookup"><span data-stu-id="51bd3-127">Relationships</span></span>
<span data-ttu-id="51bd3-128">无。</span><span class="sxs-lookup"><span data-stu-id="51bd3-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51bd3-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51bd3-129">JSON representation</span></span>
<span data-ttu-id="51bd3-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51bd3-130">The following is a JSON representation of the resource.</span></span>
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

