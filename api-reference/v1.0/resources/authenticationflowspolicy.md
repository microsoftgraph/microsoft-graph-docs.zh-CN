---
title: authenticationFlowsPolicy 资源类型
description: '表示租户级别的自助注册体验策略配置，允许外部用户请求注册以进行批准。 '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea0ca54c4be4e80043ac9560d2b8dd3744584aa9
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882826"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="c7fdc-103">authenticationFlowsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7fdc-103">authenticationFlowsPolicy resource type</span></span>

<span data-ttu-id="c7fdc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7fdc-105">表示租户级别的[自助注册体验策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行批准。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="c7fdc-106">它包含有关 ID、显示名称和说明的信息，并指示是否对该策略启用了自助注册。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-106">It contains information, such as the identifier, display name, and description, and indicates whether self-service sign-up is enabled for the policy.</span></span>

## <a name="methods"></a><span data-ttu-id="c7fdc-107">方法</span><span class="sxs-lookup"><span data-stu-id="c7fdc-107">Methods</span></span>

| <span data-ttu-id="c7fdc-108">方法</span><span class="sxs-lookup"><span data-stu-id="c7fdc-108">Method</span></span>       | <span data-ttu-id="c7fdc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7fdc-109">Return Type</span></span>  |<span data-ttu-id="c7fdc-110">说明</span><span class="sxs-lookup"><span data-stu-id="c7fdc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7fdc-111">获取身份验证流策略</span><span class="sxs-lookup"><span data-stu-id="c7fdc-111">Get authentication flows policy</span></span>](../api/authenticationflowspolicy-get.md)|<span data-ttu-id="c7fdc-112">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c7fdc-112">authenticationFlowsPolicy</span></span>|<span data-ttu-id="c7fdc-113">获取身份验证流策略配置。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-113">Get the authentication flows policy configuration.</span></span>|
|[<span data-ttu-id="c7fdc-114">更新身份验证流策略</span><span class="sxs-lookup"><span data-stu-id="c7fdc-114">Update authentication flows policy</span></span>](../api/authenticationflowspolicy-update.md)|<span data-ttu-id="c7fdc-115">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c7fdc-115">authenticationFlowsPolicy</span></span>|<span data-ttu-id="c7fdc-116">更新身份验证流策略配置。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-116">Update the authentication flows policy configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7fdc-117">属性</span><span class="sxs-lookup"><span data-stu-id="c7fdc-117">Properties</span></span>

|<span data-ttu-id="c7fdc-118">属性</span><span class="sxs-lookup"><span data-stu-id="c7fdc-118">Property</span></span>|<span data-ttu-id="c7fdc-119">类型</span><span class="sxs-lookup"><span data-stu-id="c7fdc-119">Type</span></span>|<span data-ttu-id="c7fdc-120">说明</span><span class="sxs-lookup"><span data-stu-id="c7fdc-120">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="c7fdc-121">id</span><span class="sxs-lookup"><span data-stu-id="c7fdc-121">id</span></span>|<span data-ttu-id="c7fdc-122">字符串</span><span class="sxs-lookup"><span data-stu-id="c7fdc-122">String</span></span>| <span data-ttu-id="c7fdc-123">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-123">Inherited property.</span></span> <span data-ttu-id="c7fdc-124">身份验证流策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-124">The identifier of the authentication flows policy.</span></span> <span data-ttu-id="c7fdc-125">可选。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-125">Optional.</span></span> <span data-ttu-id="c7fdc-126">只读。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-126">Read-only.</span></span>
|<span data-ttu-id="c7fdc-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c7fdc-127">displayName</span></span>|<span data-ttu-id="c7fdc-128">字符串</span><span class="sxs-lookup"><span data-stu-id="c7fdc-128">String</span></span>| <span data-ttu-id="c7fdc-129">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-129">Inherited property.</span></span> <span data-ttu-id="c7fdc-130">策略的用户可读名称。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-130">The human-readable name of the policy.</span></span> <span data-ttu-id="c7fdc-131">可选。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-131">Optional.</span></span> <span data-ttu-id="c7fdc-132">只读。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-132">Read-only.</span></span>|
|<span data-ttu-id="c7fdc-133">说明</span><span class="sxs-lookup"><span data-stu-id="c7fdc-133">description</span></span>|<span data-ttu-id="c7fdc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c7fdc-134">String</span></span>|<span data-ttu-id="c7fdc-135">继承的属性。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-135">Inherited property.</span></span> <span data-ttu-id="c7fdc-136">策略说明。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-136">A description of the policy.</span></span> <span data-ttu-id="c7fdc-137">可选。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-137">Optional.</span></span> <span data-ttu-id="c7fdc-138">只读。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-138">Read-only.</span></span>|
|<span data-ttu-id="c7fdc-139">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="c7fdc-139">selfServiceSignUp</span></span>|[<span data-ttu-id="c7fdc-140">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7fdc-140">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="c7fdc-141">包含用于传达是否已启用或禁用自助注册的 [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) 设置。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-141">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="c7fdc-142">可选。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-142">Optional.</span></span> <span data-ttu-id="c7fdc-143">只读。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-143">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7fdc-144">关系</span><span class="sxs-lookup"><span data-stu-id="c7fdc-144">Relationships</span></span>

<span data-ttu-id="c7fdc-145">无。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7fdc-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7fdc-146">JSON representation</span></span>

<span data-ttu-id="c7fdc-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7fdc-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
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
