---
title: fido2AuthenticationMethod 资源类型
description: 注册到用户的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c79a704d9a2aa899ffc2a3f4592f76a30d30126
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964685"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="8a3fd-104">fido2AuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a3fd-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="8a3fd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a3fd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a3fd-106">注册到用户的 FIDO2 安全密钥的表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="8a3fd-107">FIDO2 是一种登录身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="8a3fd-108">Methods</span><span class="sxs-lookup"><span data-stu-id="8a3fd-108">Methods</span></span>
|<span data-ttu-id="8a3fd-109">方法</span><span class="sxs-lookup"><span data-stu-id="8a3fd-109">Method</span></span>|<span data-ttu-id="8a3fd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a3fd-110">Return type</span></span>|<span data-ttu-id="8a3fd-111">Description</span><span class="sxs-lookup"><span data-stu-id="8a3fd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a3fd-112">List</span><span class="sxs-lookup"><span data-stu-id="8a3fd-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="8a3fd-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a3fd-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="8a3fd-114">检索用户的 fido2AuthenticationMethod 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="8a3fd-115">获取</span><span class="sxs-lookup"><span data-stu-id="8a3fd-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="8a3fd-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8a3fd-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="8a3fd-117">读取用户的 fido2AuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="8a3fd-118">删除</span><span class="sxs-lookup"><span data-stu-id="8a3fd-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="8a3fd-119">无</span><span class="sxs-lookup"><span data-stu-id="8a3fd-119">None</span></span>|<span data-ttu-id="8a3fd-120">删除用户的 fido2AuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a3fd-121">属性</span><span class="sxs-lookup"><span data-stu-id="8a3fd-121">Properties</span></span>
|<span data-ttu-id="8a3fd-122">属性</span><span class="sxs-lookup"><span data-stu-id="8a3fd-122">Property</span></span>|<span data-ttu-id="8a3fd-123">类型</span><span class="sxs-lookup"><span data-stu-id="8a3fd-123">Type</span></span>|<span data-ttu-id="8a3fd-124">说明</span><span class="sxs-lookup"><span data-stu-id="8a3fd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a3fd-125">id</span><span class="sxs-lookup"><span data-stu-id="8a3fd-125">id</span></span>|<span data-ttu-id="8a3fd-126">String</span><span class="sxs-lookup"><span data-stu-id="8a3fd-126">String</span></span>|<span data-ttu-id="8a3fd-127">身份验证方法标识符。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="8a3fd-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8a3fd-128">displayName</span></span>|<span data-ttu-id="8a3fd-129">String</span><span class="sxs-lookup"><span data-stu-id="8a3fd-129">String</span></span>|<span data-ttu-id="8a3fd-130">用户显示名称的键的键值。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="8a3fd-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a3fd-131">createdDateTime</span></span>|<span data-ttu-id="8a3fd-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a3fd-132">DateTimeOffset</span></span>|<span data-ttu-id="8a3fd-133">向用户注册此密钥的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="8a3fd-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="8a3fd-134">aaGuid</span></span>|<span data-ttu-id="8a3fd-135">String</span><span class="sxs-lookup"><span data-stu-id="8a3fd-135">String</span></span>|<span data-ttu-id="8a3fd-136">验证器证明 GUID，一个指示验证 (类型的标识符，例如验证器的) 和型号。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="8a3fd-137">model</span><span class="sxs-lookup"><span data-stu-id="8a3fd-137">model</span></span>|<span data-ttu-id="8a3fd-138">String</span><span class="sxs-lookup"><span data-stu-id="8a3fd-138">String</span></span>|<span data-ttu-id="8a3fd-139">FIDO2 安全密钥的制造商分配模型。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="8a3fd-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="8a3fd-140">attestationCertificates</span></span>|<span data-ttu-id="8a3fd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8a3fd-141">String collection</span></span>|<span data-ttu-id="8a3fd-142">证明证书 () 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="8a3fd-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="8a3fd-143">attestationLevel</span></span>|<span data-ttu-id="8a3fd-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="8a3fd-144">attestationLevel</span></span>|<span data-ttu-id="8a3fd-145">此 FIDO2 安全密钥的证明级别。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="8a3fd-146">可能的值是： `attested` 或 `notAttested` 。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-146">Possible values are: `attested`, or `notAttested`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8a3fd-147">关系</span><span class="sxs-lookup"><span data-stu-id="8a3fd-147">Relationships</span></span>
<span data-ttu-id="8a3fd-148">无。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a3fd-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a3fd-149">JSON representation</span></span>
<span data-ttu-id="8a3fd-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a3fd-150">The following is a JSON representation of the resource.</span></span>
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

