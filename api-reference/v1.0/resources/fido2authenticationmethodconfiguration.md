---
title: fido2AuthenticationMethodConfiguration 资源类型
description: 表示 FIDO2 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 00137618daf327793d7d60d8dadbe8ad89abc840
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468623"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="27def-103">fido2AuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="27def-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="27def-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27def-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27def-105">表示 FIDO2 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="27def-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="27def-106">身份验证方法策略定义配置设置以及能够使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="27def-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="27def-107">方法</span><span class="sxs-lookup"><span data-stu-id="27def-107">Methods</span></span>
|<span data-ttu-id="27def-108">方法</span><span class="sxs-lookup"><span data-stu-id="27def-108">Method</span></span>|<span data-ttu-id="27def-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="27def-109">Return type</span></span>|<span data-ttu-id="27def-110">说明</span><span class="sxs-lookup"><span data-stu-id="27def-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27def-111">获取</span><span class="sxs-lookup"><span data-stu-id="27def-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="27def-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="27def-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="27def-113">读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27def-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="27def-114">更新</span><span class="sxs-lookup"><span data-stu-id="27def-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="27def-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="27def-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="27def-116">更新 fido2AuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27def-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="27def-117">删除</span><span class="sxs-lookup"><span data-stu-id="27def-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="27def-118">无</span><span class="sxs-lookup"><span data-stu-id="27def-118">None</span></span>|<span data-ttu-id="27def-119">将 fido2AuthenticationMethodConfiguration 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="27def-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="27def-120">属性</span><span class="sxs-lookup"><span data-stu-id="27def-120">Properties</span></span>
|<span data-ttu-id="27def-121">属性</span><span class="sxs-lookup"><span data-stu-id="27def-121">Property</span></span>|<span data-ttu-id="27def-122">类型</span><span class="sxs-lookup"><span data-stu-id="27def-122">Type</span></span>|<span data-ttu-id="27def-123">说明</span><span class="sxs-lookup"><span data-stu-id="27def-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27def-124">id</span><span class="sxs-lookup"><span data-stu-id="27def-124">id</span></span>|<span data-ttu-id="27def-125">String</span><span class="sxs-lookup"><span data-stu-id="27def-125">String</span></span>|<span data-ttu-id="27def-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="27def-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="27def-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="27def-127">isAttestationEnforced</span></span>|<span data-ttu-id="27def-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="27def-128">Boolean</span></span>|<span data-ttu-id="27def-129">确定是否必须对 FIDO2 安全密钥注册强制执行证明。</span><span class="sxs-lookup"><span data-stu-id="27def-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="27def-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="27def-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="27def-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="27def-131">Boolean</span></span>|<span data-ttu-id="27def-132">确定用户能否注册新的 FIDO2 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="27def-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="27def-133">keyRestrictions</span><span class="sxs-lookup"><span data-stu-id="27def-133">keyRestrictions</span></span>|[<span data-ttu-id="27def-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="27def-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="27def-135">控制是否对 FIDO2 安全密钥实施密钥限制，允许或禁止验证器证明 GUID (AAGUID) 定义的某些密钥类型，即指示验证器的类型 (例如验证器的 make 和 model) 。</span><span class="sxs-lookup"><span data-stu-id="27def-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="27def-136">state</span><span class="sxs-lookup"><span data-stu-id="27def-136">state</span></span>|<span data-ttu-id="27def-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="27def-137">authenticationMethodState</span></span>|<span data-ttu-id="27def-138">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27def-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27def-139">关系</span><span class="sxs-lookup"><span data-stu-id="27def-139">Relationships</span></span>
|<span data-ttu-id="27def-140">关系</span><span class="sxs-lookup"><span data-stu-id="27def-140">Relationship</span></span>|<span data-ttu-id="27def-141">类型</span><span class="sxs-lookup"><span data-stu-id="27def-141">Type</span></span>|<span data-ttu-id="27def-142">说明</span><span class="sxs-lookup"><span data-stu-id="27def-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27def-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="27def-143">includeTargets</span></span>|<span data-ttu-id="27def-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27def-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="27def-145">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="27def-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27def-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27def-146">JSON representation</span></span>
<span data-ttu-id="27def-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27def-147">The following is a JSON representation of the resource.</span></span>
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
