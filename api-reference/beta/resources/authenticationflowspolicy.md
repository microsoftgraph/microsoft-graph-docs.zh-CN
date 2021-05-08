---
title: authenticationFlowsPolicy 资源类型
description: '表示租户级别的自助注册体验策略配置，允许外部用户请求注册以进行批准。 '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cc7f6261e4db4b908d6ab3e0ab3c41504ce8462b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232107"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="1d403-103">authenticationFlowsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d403-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="1d403-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d403-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d403-105">表示租户级别的[自助注册体验策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行批准。</span><span class="sxs-lookup"><span data-stu-id="1d403-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="1d403-106">它包含有关 ID、显示名称和说明的信息，并指示是否对该策略启用了自助注册。</span><span class="sxs-lookup"><span data-stu-id="1d403-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="1d403-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d403-107">Properties</span></span>
|<span data-ttu-id="1d403-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d403-108">Property</span></span>|<span data-ttu-id="1d403-109">类型</span><span class="sxs-lookup"><span data-stu-id="1d403-109">Type</span></span>|<span data-ttu-id="1d403-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d403-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="1d403-111">id</span><span class="sxs-lookup"><span data-stu-id="1d403-111">id</span></span>|<span data-ttu-id="1d403-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1d403-112">String</span></span>| <span data-ttu-id="1d403-113">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="1d403-113">Inherited property.</span></span> <span data-ttu-id="1d403-114">身份验证流策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d403-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="1d403-115">可选。</span><span class="sxs-lookup"><span data-stu-id="1d403-115">Optional.</span></span> <span data-ttu-id="1d403-116">只读。</span><span class="sxs-lookup"><span data-stu-id="1d403-116">Read-only.</span></span>
|<span data-ttu-id="1d403-117">displayName</span><span class="sxs-lookup"><span data-stu-id="1d403-117">displayName</span></span>|<span data-ttu-id="1d403-118">字符串</span><span class="sxs-lookup"><span data-stu-id="1d403-118">String</span></span>| <span data-ttu-id="1d403-119">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="1d403-119">Inherited property.</span></span> <span data-ttu-id="1d403-120">策略的用户可读名称。</span><span class="sxs-lookup"><span data-stu-id="1d403-120">The human-readable name of the policy.</span></span> <span data-ttu-id="1d403-121">此属性不是一个键。</span><span class="sxs-lookup"><span data-stu-id="1d403-121">This property is not a key.</span></span> <span data-ttu-id="1d403-122">可选。</span><span class="sxs-lookup"><span data-stu-id="1d403-122">Optional.</span></span> <span data-ttu-id="1d403-123">只读。</span><span class="sxs-lookup"><span data-stu-id="1d403-123">Read-only.</span></span>|
|<span data-ttu-id="1d403-124">说明</span><span class="sxs-lookup"><span data-stu-id="1d403-124">description</span></span>|<span data-ttu-id="1d403-125">字符串</span><span class="sxs-lookup"><span data-stu-id="1d403-125">String</span></span>|<span data-ttu-id="1d403-126">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="1d403-126">Inherited property.</span></span> <span data-ttu-id="1d403-127">策略说明。</span><span class="sxs-lookup"><span data-stu-id="1d403-127">A description of the policy.</span></span> <span data-ttu-id="1d403-128">此属性不是一个键。</span><span class="sxs-lookup"><span data-stu-id="1d403-128">This property is not a key.</span></span> <span data-ttu-id="1d403-129">可选。</span><span class="sxs-lookup"><span data-stu-id="1d403-129">Optional.</span></span> <span data-ttu-id="1d403-130">只读。</span><span class="sxs-lookup"><span data-stu-id="1d403-130">Read-only.</span></span>|
|<span data-ttu-id="1d403-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="1d403-131">selfServiceSignUp</span></span>|[<span data-ttu-id="1d403-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d403-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="1d403-133">包含用于传达是否已启用或禁用自助注册的 [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) 设置。</span><span class="sxs-lookup"><span data-stu-id="1d403-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="1d403-134">此属性不是一个键。</span><span class="sxs-lookup"><span data-stu-id="1d403-134">This property is not a key.</span></span> <span data-ttu-id="1d403-135">可选。</span><span class="sxs-lookup"><span data-stu-id="1d403-135">Optional.</span></span> <span data-ttu-id="1d403-136">只读。</span><span class="sxs-lookup"><span data-stu-id="1d403-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d403-137">关系</span><span class="sxs-lookup"><span data-stu-id="1d403-137">Relationships</span></span>
<span data-ttu-id="1d403-138">无。</span><span class="sxs-lookup"><span data-stu-id="1d403-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d403-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d403-139">JSON representation</span></span>
<span data-ttu-id="1d403-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d403-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```


