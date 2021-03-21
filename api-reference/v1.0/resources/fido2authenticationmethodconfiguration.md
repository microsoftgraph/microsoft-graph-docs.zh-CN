---
title: fido2AuthenticationMethodConfiguration 资源类型
description: 表示 FIDO2 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7684b8b2c6601b4afdad25b3d3c32b7a6b68667d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964684"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="798d5-103">fido2AuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="798d5-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="798d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="798d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="798d5-105">表示 FIDO2 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="798d5-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="798d5-106">身份验证方法策略定义配置设置以及能够使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="798d5-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="798d5-107">Methods</span><span class="sxs-lookup"><span data-stu-id="798d5-107">Methods</span></span>
|<span data-ttu-id="798d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="798d5-108">Method</span></span>|<span data-ttu-id="798d5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="798d5-109">Return type</span></span>|<span data-ttu-id="798d5-110">说明</span><span class="sxs-lookup"><span data-stu-id="798d5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="798d5-111">获取</span><span class="sxs-lookup"><span data-stu-id="798d5-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="798d5-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="798d5-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="798d5-113">读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="798d5-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="798d5-114">更新</span><span class="sxs-lookup"><span data-stu-id="798d5-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="798d5-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="798d5-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="798d5-116">更新 fido2AuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="798d5-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="798d5-117">删除</span><span class="sxs-lookup"><span data-stu-id="798d5-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="798d5-118">无</span><span class="sxs-lookup"><span data-stu-id="798d5-118">None</span></span>|<span data-ttu-id="798d5-119">将 fido2AuthenticationMethodConfiguration 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="798d5-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="798d5-120">属性</span><span class="sxs-lookup"><span data-stu-id="798d5-120">Properties</span></span>
|<span data-ttu-id="798d5-121">属性</span><span class="sxs-lookup"><span data-stu-id="798d5-121">Property</span></span>|<span data-ttu-id="798d5-122">类型</span><span class="sxs-lookup"><span data-stu-id="798d5-122">Type</span></span>|<span data-ttu-id="798d5-123">说明</span><span class="sxs-lookup"><span data-stu-id="798d5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="798d5-124">id</span><span class="sxs-lookup"><span data-stu-id="798d5-124">id</span></span>|<span data-ttu-id="798d5-125">String</span><span class="sxs-lookup"><span data-stu-id="798d5-125">String</span></span>|<span data-ttu-id="798d5-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="798d5-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="798d5-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="798d5-127">isAttestationEnforced</span></span>|<span data-ttu-id="798d5-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="798d5-128">Boolean</span></span>|<span data-ttu-id="798d5-129">确定是否必须对 FIDO2 安全密钥注册强制执行证明。</span><span class="sxs-lookup"><span data-stu-id="798d5-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="798d5-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="798d5-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="798d5-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="798d5-131">Boolean</span></span>|<span data-ttu-id="798d5-132">确定用户能否注册新的 FIDO2 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="798d5-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="798d5-133">keyRestrictions</span><span class="sxs-lookup"><span data-stu-id="798d5-133">keyRestrictions</span></span>|[<span data-ttu-id="798d5-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="798d5-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="798d5-135">控制是否对 FIDO2 安全密钥实施密钥限制，允许或禁止验证器证明 GUID (AAGUID) 定义的某些密钥类型，即指示验证器的类型 (例如验证器的 make 和 model) 。</span><span class="sxs-lookup"><span data-stu-id="798d5-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="798d5-136">state</span><span class="sxs-lookup"><span data-stu-id="798d5-136">state</span></span>|<span data-ttu-id="798d5-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="798d5-137">authenticationMethodState</span></span>|<span data-ttu-id="798d5-138">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="798d5-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="798d5-139">关系</span><span class="sxs-lookup"><span data-stu-id="798d5-139">Relationships</span></span>
|<span data-ttu-id="798d5-140">关系</span><span class="sxs-lookup"><span data-stu-id="798d5-140">Relationship</span></span>|<span data-ttu-id="798d5-141">类型</span><span class="sxs-lookup"><span data-stu-id="798d5-141">Type</span></span>|<span data-ttu-id="798d5-142">说明</span><span class="sxs-lookup"><span data-stu-id="798d5-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="798d5-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="798d5-143">includeTargets</span></span>|<span data-ttu-id="798d5-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="798d5-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="798d5-145">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="798d5-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="798d5-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="798d5-146">JSON representation</span></span>
<span data-ttu-id="798d5-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="798d5-147">The following is a JSON representation of the resource.</span></span>
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
