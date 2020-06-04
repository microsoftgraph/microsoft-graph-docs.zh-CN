---
title: authenticationFlowsPolicy 资源类型
description: '表示在租户级别上自助服务注册体验的策略配置，允许外部用户请求注册以进行审批。 '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 263b92c081545fc3ce337d25b4813d85fe034940
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556398"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="34126-103">authenticationFlowsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="34126-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="34126-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34126-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34126-105">表示在租户级别上[自助服务注册体验的策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行审批。</span><span class="sxs-lookup"><span data-stu-id="34126-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="34126-106">它包含有关 ID、显示名称和说明的信息，并指示是否为策略启用自助服务注册。</span><span class="sxs-lookup"><span data-stu-id="34126-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="34126-107">属性</span><span class="sxs-lookup"><span data-stu-id="34126-107">Properties</span></span>
|<span data-ttu-id="34126-108">属性</span><span class="sxs-lookup"><span data-stu-id="34126-108">Property</span></span>|<span data-ttu-id="34126-109">类型</span><span class="sxs-lookup"><span data-stu-id="34126-109">Type</span></span>|<span data-ttu-id="34126-110">说明</span><span class="sxs-lookup"><span data-stu-id="34126-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="34126-111">id</span><span class="sxs-lookup"><span data-stu-id="34126-111">id</span></span>|<span data-ttu-id="34126-112">字符串</span><span class="sxs-lookup"><span data-stu-id="34126-112">String</span></span>| <span data-ttu-id="34126-113">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="34126-113">Inherited property.</span></span> <span data-ttu-id="34126-114">身份验证流策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="34126-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="34126-115">可选。</span><span class="sxs-lookup"><span data-stu-id="34126-115">Optional.</span></span> <span data-ttu-id="34126-116">只读。</span><span class="sxs-lookup"><span data-stu-id="34126-116">Read-only.</span></span>
|<span data-ttu-id="34126-117">displayName</span><span class="sxs-lookup"><span data-stu-id="34126-117">displayName</span></span>|<span data-ttu-id="34126-118">String</span><span class="sxs-lookup"><span data-stu-id="34126-118">String</span></span>| <span data-ttu-id="34126-119">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="34126-119">Inherited property.</span></span> <span data-ttu-id="34126-120">策略的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="34126-120">The human-readable name of the policy.</span></span> <span data-ttu-id="34126-121">此属性不是键。</span><span class="sxs-lookup"><span data-stu-id="34126-121">This property is not a key.</span></span> <span data-ttu-id="34126-122">可选。</span><span class="sxs-lookup"><span data-stu-id="34126-122">Optional.</span></span> <span data-ttu-id="34126-123">只读。</span><span class="sxs-lookup"><span data-stu-id="34126-123">Read-only.</span></span>|
|<span data-ttu-id="34126-124">说明</span><span class="sxs-lookup"><span data-stu-id="34126-124">description</span></span>|<span data-ttu-id="34126-125">String</span><span class="sxs-lookup"><span data-stu-id="34126-125">String</span></span>|<span data-ttu-id="34126-126">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="34126-126">Inherited property.</span></span> <span data-ttu-id="34126-127">策略说明。</span><span class="sxs-lookup"><span data-stu-id="34126-127">A description of the policy.</span></span> <span data-ttu-id="34126-128">此属性不是键。</span><span class="sxs-lookup"><span data-stu-id="34126-128">This property is not a key.</span></span> <span data-ttu-id="34126-129">可选。</span><span class="sxs-lookup"><span data-stu-id="34126-129">Optional.</span></span> <span data-ttu-id="34126-130">只读。</span><span class="sxs-lookup"><span data-stu-id="34126-130">Read-only.</span></span>|
|<span data-ttu-id="34126-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="34126-131">selfServiceSignUp</span></span>|[<span data-ttu-id="34126-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="34126-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="34126-133">包含可传达是否启用或禁用自助注册的[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md)设置。</span><span class="sxs-lookup"><span data-stu-id="34126-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="34126-134">此属性不是键。</span><span class="sxs-lookup"><span data-stu-id="34126-134">This property is not a key.</span></span> <span data-ttu-id="34126-135">可选。</span><span class="sxs-lookup"><span data-stu-id="34126-135">Optional.</span></span> <span data-ttu-id="34126-136">只读。</span><span class="sxs-lookup"><span data-stu-id="34126-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="34126-137">关系</span><span class="sxs-lookup"><span data-stu-id="34126-137">Relationships</span></span>
<span data-ttu-id="34126-138">无。</span><span class="sxs-lookup"><span data-stu-id="34126-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34126-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34126-139">JSON representation</span></span>
<span data-ttu-id="34126-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34126-140">The following is a JSON representation of the resource.</span></span>
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
