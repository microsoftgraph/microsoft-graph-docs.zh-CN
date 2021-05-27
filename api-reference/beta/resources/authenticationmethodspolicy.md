---
title: authenticationMethodsPolicy 资源类型
description: 定义身份验证方法以及允许使用这些方法登录并执行 MFA (多重) 。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fdf86929b4098d9fb62f1426883b55d95c669f32
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682880"
---
# <a name="authenticationmethodspolicy-resource-type"></a><span data-ttu-id="d5da6-103">authenticationMethodsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5da6-103">authenticationMethodsPolicy resource type</span></span>

<span data-ttu-id="d5da6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5da6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5da6-105">定义身份验证方法以及允许使用它们登录和在 Azure AD) 中 (MFA) 执行Azure Active Directory (身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="d5da6-105">Defines authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="d5da6-106">方法</span><span class="sxs-lookup"><span data-stu-id="d5da6-106">Methods</span></span>
|<span data-ttu-id="d5da6-107">方法</span><span class="sxs-lookup"><span data-stu-id="d5da6-107">Method</span></span>|<span data-ttu-id="d5da6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5da6-108">Return type</span></span>|<span data-ttu-id="d5da6-109">说明</span><span class="sxs-lookup"><span data-stu-id="d5da6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5da6-110">获取 authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="d5da6-110">Get authenticationMethodsPolicy</span></span>](../api/authenticationmethodspolicy-get.md)|[<span data-ttu-id="d5da6-111">authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="d5da6-111">authenticationMethodsPolicy</span></span>](../resources/authenticationmethodspolicy.md)|<span data-ttu-id="d5da6-112">读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5da6-112">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>|
|[<span data-ttu-id="d5da6-113">更新 authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="d5da6-113">Update authenticationMethodsPolicy</span></span>](../api/authenticationmethodspolicy-update.md)|[<span data-ttu-id="d5da6-114">authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="d5da6-114">authenticationMethodsPolicy</span></span>](../resources/authenticationmethodspolicy.md)|<span data-ttu-id="d5da6-115">更新 [authenticationMethodsPolicy 对象](../resources/authenticationmethodspolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d5da6-115">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5da6-116">属性</span><span class="sxs-lookup"><span data-stu-id="d5da6-116">Properties</span></span>
|<span data-ttu-id="d5da6-117">属性</span><span class="sxs-lookup"><span data-stu-id="d5da6-117">Property</span></span>|<span data-ttu-id="d5da6-118">类型</span><span class="sxs-lookup"><span data-stu-id="d5da6-118">Type</span></span>|<span data-ttu-id="d5da6-119">说明</span><span class="sxs-lookup"><span data-stu-id="d5da6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5da6-120">说明</span><span class="sxs-lookup"><span data-stu-id="d5da6-120">description</span></span>|<span data-ttu-id="d5da6-121">String</span><span class="sxs-lookup"><span data-stu-id="d5da6-121">String</span></span>|<span data-ttu-id="d5da6-122">策略说明。</span><span class="sxs-lookup"><span data-stu-id="d5da6-122">A description of the policy.</span></span>|
|<span data-ttu-id="d5da6-123">displayName</span><span class="sxs-lookup"><span data-stu-id="d5da6-123">displayName</span></span>|<span data-ttu-id="d5da6-124">String</span><span class="sxs-lookup"><span data-stu-id="d5da6-124">String</span></span>|<span data-ttu-id="d5da6-125">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="d5da6-125">The name of the policy.</span></span>|
|<span data-ttu-id="d5da6-126">id</span><span class="sxs-lookup"><span data-stu-id="d5da6-126">id</span></span>|<span data-ttu-id="d5da6-127">String</span><span class="sxs-lookup"><span data-stu-id="d5da6-127">String</span></span>|<span data-ttu-id="d5da6-128">策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="d5da6-128">The identifier of the policy.</span></span> <span data-ttu-id="d5da6-129">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="d5da6-129">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="d5da6-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5da6-130">lastModifiedDateTime</span></span>|<span data-ttu-id="d5da6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5da6-131">DateTimeOffset</span></span>|<span data-ttu-id="d5da6-132">上次更新策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d5da6-132">The date and time of the last update to the policy.</span></span>|
|<span data-ttu-id="d5da6-133">policyVersion</span><span class="sxs-lookup"><span data-stu-id="d5da6-133">policyVersion</span></span>|<span data-ttu-id="d5da6-134">String</span><span class="sxs-lookup"><span data-stu-id="d5da6-134">String</span></span>|<span data-ttu-id="d5da6-135">使用的策略的版本。</span><span class="sxs-lookup"><span data-stu-id="d5da6-135">The version of the policy in use.</span></span>|
|<span data-ttu-id="d5da6-136">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="d5da6-136">registrationEnforcement</span></span>|[<span data-ttu-id="d5da6-137">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="d5da6-137">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="d5da6-138">在登录时强制注册。</span><span class="sxs-lookup"><span data-stu-id="d5da6-138">Enforce registration at sign-in time.</span></span> <span data-ttu-id="d5da6-139">此属性可用于提醒用户设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d5da6-139">This property can be used to remind users to set up targeted authentication methods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5da6-140">关系</span><span class="sxs-lookup"><span data-stu-id="d5da6-140">Relationships</span></span>
|<span data-ttu-id="d5da6-141">关系</span><span class="sxs-lookup"><span data-stu-id="d5da6-141">Relationship</span></span>|<span data-ttu-id="d5da6-142">类型</span><span class="sxs-lookup"><span data-stu-id="d5da6-142">Type</span></span>|<span data-ttu-id="d5da6-143">说明</span><span class="sxs-lookup"><span data-stu-id="d5da6-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5da6-144">authenticationMethodConfigurations</span><span class="sxs-lookup"><span data-stu-id="d5da6-144">authenticationMethodConfigurations</span></span>|<span data-ttu-id="d5da6-145">[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5da6-145">[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) collection</span></span>|<span data-ttu-id="d5da6-146">表示每个身份验证方法的设置。</span><span class="sxs-lookup"><span data-stu-id="d5da6-146">Represents the settings for each authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5da6-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5da6-147">JSON representation</span></span>
<span data-ttu-id="d5da6-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5da6-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  } 
}
```
