---
title: authenticationFlowsPolicy 资源类型
description: '表示租户级别的自助注册体验策略配置，允许外部用户请求注册以进行批准。 '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a676014ba6d31ffea08331342504629796f49ec8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034129"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="8f2bc-103">authenticationFlowsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f2bc-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="8f2bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f2bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f2bc-105">表示租户级别的[自助注册体验策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行批准。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="8f2bc-106">它包含有关 ID、显示名称和说明的信息，并指示是否对该策略启用了自助注册。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="8f2bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="8f2bc-107">Properties</span></span>
|<span data-ttu-id="8f2bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f2bc-108">Property</span></span>|<span data-ttu-id="8f2bc-109">类型</span><span class="sxs-lookup"><span data-stu-id="8f2bc-109">Type</span></span>|<span data-ttu-id="8f2bc-110">说明</span><span class="sxs-lookup"><span data-stu-id="8f2bc-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="8f2bc-111">id</span><span class="sxs-lookup"><span data-stu-id="8f2bc-111">id</span></span>|<span data-ttu-id="8f2bc-112">字符串</span><span class="sxs-lookup"><span data-stu-id="8f2bc-112">String</span></span>| <span data-ttu-id="8f2bc-113">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-113">Inherited property.</span></span> <span data-ttu-id="8f2bc-114">身份验证流策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="8f2bc-115">可选。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-115">Optional.</span></span> <span data-ttu-id="8f2bc-116">只读。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-116">Read-only.</span></span>
|<span data-ttu-id="8f2bc-117">displayName</span><span class="sxs-lookup"><span data-stu-id="8f2bc-117">displayName</span></span>|<span data-ttu-id="8f2bc-118">字符串</span><span class="sxs-lookup"><span data-stu-id="8f2bc-118">String</span></span>| <span data-ttu-id="8f2bc-119">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-119">Inherited property.</span></span> <span data-ttu-id="8f2bc-120">策略的用户可读名称。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-120">The human-readable name of the policy.</span></span> <span data-ttu-id="8f2bc-121">此属性不是一个键。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-121">This property is not a key.</span></span> <span data-ttu-id="8f2bc-122">可选。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-122">Optional.</span></span> <span data-ttu-id="8f2bc-123">只读。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-123">Read-only.</span></span>|
|<span data-ttu-id="8f2bc-124">说明</span><span class="sxs-lookup"><span data-stu-id="8f2bc-124">description</span></span>|<span data-ttu-id="8f2bc-125">字符串</span><span class="sxs-lookup"><span data-stu-id="8f2bc-125">String</span></span>|<span data-ttu-id="8f2bc-126">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-126">Inherited property.</span></span> <span data-ttu-id="8f2bc-127">策略说明。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-127">A description of the policy.</span></span> <span data-ttu-id="8f2bc-128">此属性不是一个键。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-128">This property is not a key.</span></span> <span data-ttu-id="8f2bc-129">可选。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-129">Optional.</span></span> <span data-ttu-id="8f2bc-130">只读。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-130">Read-only.</span></span>|
|<span data-ttu-id="8f2bc-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="8f2bc-131">selfServiceSignUp</span></span>|[<span data-ttu-id="8f2bc-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f2bc-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="8f2bc-133">包含用于传达是否已启用或禁用自助注册的 [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) 设置。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="8f2bc-134">此属性不是一个键。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-134">This property is not a key.</span></span> <span data-ttu-id="8f2bc-135">可选。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-135">Optional.</span></span> <span data-ttu-id="8f2bc-136">只读。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f2bc-137">关系</span><span class="sxs-lookup"><span data-stu-id="8f2bc-137">Relationships</span></span>
<span data-ttu-id="8f2bc-138">无。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f2bc-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f2bc-139">JSON representation</span></span>
<span data-ttu-id="8f2bc-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f2bc-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```


