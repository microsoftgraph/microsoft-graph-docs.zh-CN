---
title: fido2AuthenticationMethod 资源类型
description: 注册到用户的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8e1dceac5e7c901cdeeba7788c6a1541fdc26867
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469148"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="22ec8-104">fido2AuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="22ec8-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="22ec8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22ec8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22ec8-106">注册到用户的 FIDO2 安全密钥的表示形式。</span><span class="sxs-lookup"><span data-stu-id="22ec8-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="22ec8-107">FIDO2 是一种登录身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="22ec8-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="22ec8-108">方法</span><span class="sxs-lookup"><span data-stu-id="22ec8-108">Methods</span></span>
|<span data-ttu-id="22ec8-109">方法</span><span class="sxs-lookup"><span data-stu-id="22ec8-109">Method</span></span>|<span data-ttu-id="22ec8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="22ec8-110">Return type</span></span>|<span data-ttu-id="22ec8-111">Description</span><span class="sxs-lookup"><span data-stu-id="22ec8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22ec8-112">List</span><span class="sxs-lookup"><span data-stu-id="22ec8-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="22ec8-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22ec8-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="22ec8-114">检索用户的 fido2AuthenticationMethod 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="22ec8-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="22ec8-115">获取</span><span class="sxs-lookup"><span data-stu-id="22ec8-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="22ec8-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22ec8-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="22ec8-117">读取用户的 fido2AuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22ec8-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="22ec8-118">删除</span><span class="sxs-lookup"><span data-stu-id="22ec8-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="22ec8-119">无</span><span class="sxs-lookup"><span data-stu-id="22ec8-119">None</span></span>|<span data-ttu-id="22ec8-120">删除用户的 fido2AuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="22ec8-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22ec8-121">属性</span><span class="sxs-lookup"><span data-stu-id="22ec8-121">Properties</span></span>
|<span data-ttu-id="22ec8-122">属性</span><span class="sxs-lookup"><span data-stu-id="22ec8-122">Property</span></span>|<span data-ttu-id="22ec8-123">类型</span><span class="sxs-lookup"><span data-stu-id="22ec8-123">Type</span></span>|<span data-ttu-id="22ec8-124">说明</span><span class="sxs-lookup"><span data-stu-id="22ec8-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ec8-125">id</span><span class="sxs-lookup"><span data-stu-id="22ec8-125">id</span></span>|<span data-ttu-id="22ec8-126">String</span><span class="sxs-lookup"><span data-stu-id="22ec8-126">String</span></span>|<span data-ttu-id="22ec8-127">身份验证方法标识符。</span><span class="sxs-lookup"><span data-stu-id="22ec8-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="22ec8-128">displayName</span><span class="sxs-lookup"><span data-stu-id="22ec8-128">displayName</span></span>|<span data-ttu-id="22ec8-129">String</span><span class="sxs-lookup"><span data-stu-id="22ec8-129">String</span></span>|<span data-ttu-id="22ec8-130">用户显示名称的键的键值。</span><span class="sxs-lookup"><span data-stu-id="22ec8-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="22ec8-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22ec8-131">createdDateTime</span></span>|<span data-ttu-id="22ec8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ec8-132">DateTimeOffset</span></span>|<span data-ttu-id="22ec8-133">向用户注册此密钥的时间戳。</span><span class="sxs-lookup"><span data-stu-id="22ec8-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="22ec8-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="22ec8-134">aaGuid</span></span>|<span data-ttu-id="22ec8-135">String</span><span class="sxs-lookup"><span data-stu-id="22ec8-135">String</span></span>|<span data-ttu-id="22ec8-136">验证器证明 GUID，一个指示验证 (类型的标识符，例如验证器的) 和型号。</span><span class="sxs-lookup"><span data-stu-id="22ec8-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="22ec8-137">model</span><span class="sxs-lookup"><span data-stu-id="22ec8-137">model</span></span>|<span data-ttu-id="22ec8-138">String</span><span class="sxs-lookup"><span data-stu-id="22ec8-138">String</span></span>|<span data-ttu-id="22ec8-139">FIDO2 安全密钥的制造商分配模型。</span><span class="sxs-lookup"><span data-stu-id="22ec8-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="22ec8-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="22ec8-140">attestationCertificates</span></span>|<span data-ttu-id="22ec8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="22ec8-141">String collection</span></span>|<span data-ttu-id="22ec8-142">证明证书 () 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="22ec8-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="22ec8-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="22ec8-143">attestationLevel</span></span>|<span data-ttu-id="22ec8-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="22ec8-144">attestationLevel</span></span>|<span data-ttu-id="22ec8-145">此 FIDO2 安全密钥的证明级别。</span><span class="sxs-lookup"><span data-stu-id="22ec8-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="22ec8-146">可能的值是： `attested` 或 `notAttested` 。</span><span class="sxs-lookup"><span data-stu-id="22ec8-146">Possible values are: `attested`, or `notAttested`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="22ec8-147">关系</span><span class="sxs-lookup"><span data-stu-id="22ec8-147">Relationships</span></span>
<span data-ttu-id="22ec8-148">无。</span><span class="sxs-lookup"><span data-stu-id="22ec8-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22ec8-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22ec8-149">JSON representation</span></span>
<span data-ttu-id="22ec8-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22ec8-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

