---
title: fido2AuthenticationMethodConfiguration 资源类型
description: 代表 FIDO2 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b5d823caefba62a66fc9b2a7236c063cfaeee69b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440316"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="64150-103">fido2AuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="64150-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="64150-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64150-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64150-105">表示 FIDO2 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="64150-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="64150-106">身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="64150-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="64150-107">Methods</span><span class="sxs-lookup"><span data-stu-id="64150-107">Methods</span></span>
|<span data-ttu-id="64150-108">方法</span><span class="sxs-lookup"><span data-stu-id="64150-108">Method</span></span>|<span data-ttu-id="64150-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="64150-109">Return type</span></span>|<span data-ttu-id="64150-110">说明</span><span class="sxs-lookup"><span data-stu-id="64150-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="64150-111">获取</span><span class="sxs-lookup"><span data-stu-id="64150-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="64150-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="64150-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="64150-113">读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="64150-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="64150-114">更新</span><span class="sxs-lookup"><span data-stu-id="64150-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="64150-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="64150-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="64150-116">更新 fido2AuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="64150-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="64150-117">删除</span><span class="sxs-lookup"><span data-stu-id="64150-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="64150-118">无</span><span class="sxs-lookup"><span data-stu-id="64150-118">None</span></span>|<span data-ttu-id="64150-119">将 fido2AuthenticationMethodConfiguration 对象恢复为其默认配置。</span><span class="sxs-lookup"><span data-stu-id="64150-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="64150-120">属性</span><span class="sxs-lookup"><span data-stu-id="64150-120">Properties</span></span>
|<span data-ttu-id="64150-121">属性</span><span class="sxs-lookup"><span data-stu-id="64150-121">Property</span></span>|<span data-ttu-id="64150-122">类型</span><span class="sxs-lookup"><span data-stu-id="64150-122">Type</span></span>|<span data-ttu-id="64150-123">说明</span><span class="sxs-lookup"><span data-stu-id="64150-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64150-124">id</span><span class="sxs-lookup"><span data-stu-id="64150-124">id</span></span>|<span data-ttu-id="64150-125">String</span><span class="sxs-lookup"><span data-stu-id="64150-125">String</span></span>|<span data-ttu-id="64150-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="64150-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="64150-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="64150-127">isAttestationEnforced</span></span>|<span data-ttu-id="64150-128">布尔</span><span class="sxs-lookup"><span data-stu-id="64150-128">Boolean</span></span>|<span data-ttu-id="64150-129">确定是否必须对 FIDO2 安全密钥注册强制执行证明。</span><span class="sxs-lookup"><span data-stu-id="64150-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="64150-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="64150-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="64150-131">布尔</span><span class="sxs-lookup"><span data-stu-id="64150-131">Boolean</span></span>|<span data-ttu-id="64150-132">确定用户能否注册新的 FIDO2 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="64150-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="64150-133">keyRestrictions</span><span class="sxs-lookup"><span data-stu-id="64150-133">keyRestrictions</span></span>|[<span data-ttu-id="64150-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="64150-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="64150-135">控制是否对 FIDO2 安全密钥强制执行密钥限制，允许或禁止验证器证明 GUID (AAGUID) 定义的某些密钥类型，AAGUID) 是指示类型 (的标识符，例如验证器的制作和型号) 。</span><span class="sxs-lookup"><span data-stu-id="64150-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="64150-136">state</span><span class="sxs-lookup"><span data-stu-id="64150-136">state</span></span>|<span data-ttu-id="64150-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="64150-137">authenticationMethodState</span></span>|<span data-ttu-id="64150-138">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="64150-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64150-139">关系</span><span class="sxs-lookup"><span data-stu-id="64150-139">Relationships</span></span>
|<span data-ttu-id="64150-140">关系</span><span class="sxs-lookup"><span data-stu-id="64150-140">Relationship</span></span>|<span data-ttu-id="64150-141">类型</span><span class="sxs-lookup"><span data-stu-id="64150-141">Type</span></span>|<span data-ttu-id="64150-142">说明</span><span class="sxs-lookup"><span data-stu-id="64150-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64150-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="64150-143">includeTargets</span></span>|<span data-ttu-id="64150-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="64150-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="64150-145">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="64150-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64150-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64150-146">JSON representation</span></span>
<span data-ttu-id="64150-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64150-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  },
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
