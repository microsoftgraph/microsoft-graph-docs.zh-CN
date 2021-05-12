---
title: fido2AuthenticationMethod 资源类型
description: 注册到用户的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 87c7f5e0f9ed29e6e1f5aa7c8ec332620bcc8a0a
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335644"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="23bb6-104">fido2AuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="23bb6-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="23bb6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23bb6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23bb6-106">注册到用户的 FIDO2 安全密钥的表示形式。</span><span class="sxs-lookup"><span data-stu-id="23bb6-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="23bb6-107">FIDO2 是一种登录身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="23bb6-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="23bb6-108">方法</span><span class="sxs-lookup"><span data-stu-id="23bb6-108">Methods</span></span>
|<span data-ttu-id="23bb6-109">方法</span><span class="sxs-lookup"><span data-stu-id="23bb6-109">Method</span></span>|<span data-ttu-id="23bb6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="23bb6-110">Return type</span></span>|<span data-ttu-id="23bb6-111">Description</span><span class="sxs-lookup"><span data-stu-id="23bb6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23bb6-112">List</span><span class="sxs-lookup"><span data-stu-id="23bb6-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="23bb6-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23bb6-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="23bb6-114">检索用户的 fido2AuthenticationMethod 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="23bb6-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="23bb6-115">获取</span><span class="sxs-lookup"><span data-stu-id="23bb6-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="23bb6-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="23bb6-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="23bb6-117">读取用户的 fido2AuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23bb6-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="23bb6-118">删除</span><span class="sxs-lookup"><span data-stu-id="23bb6-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="23bb6-119">无</span><span class="sxs-lookup"><span data-stu-id="23bb6-119">None</span></span>|<span data-ttu-id="23bb6-120">删除用户的 fido2AuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="23bb6-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23bb6-121">属性</span><span class="sxs-lookup"><span data-stu-id="23bb6-121">Properties</span></span>
|<span data-ttu-id="23bb6-122">属性</span><span class="sxs-lookup"><span data-stu-id="23bb6-122">Property</span></span>|<span data-ttu-id="23bb6-123">类型</span><span class="sxs-lookup"><span data-stu-id="23bb6-123">Type</span></span>|<span data-ttu-id="23bb6-124">说明</span><span class="sxs-lookup"><span data-stu-id="23bb6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23bb6-125">id</span><span class="sxs-lookup"><span data-stu-id="23bb6-125">id</span></span>|<span data-ttu-id="23bb6-126">String</span><span class="sxs-lookup"><span data-stu-id="23bb6-126">String</span></span>|<span data-ttu-id="23bb6-127">身份验证方法标识符。</span><span class="sxs-lookup"><span data-stu-id="23bb6-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="23bb6-128">displayName</span><span class="sxs-lookup"><span data-stu-id="23bb6-128">displayName</span></span>|<span data-ttu-id="23bb6-129">String</span><span class="sxs-lookup"><span data-stu-id="23bb6-129">String</span></span>|<span data-ttu-id="23bb6-130">用户显示名称的键的键值。</span><span class="sxs-lookup"><span data-stu-id="23bb6-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="23bb6-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23bb6-131">createdDateTime</span></span>|<span data-ttu-id="23bb6-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23bb6-132">DateTimeOffset</span></span>|<span data-ttu-id="23bb6-133">向用户注册此密钥的时间戳。</span><span class="sxs-lookup"><span data-stu-id="23bb6-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="23bb6-134">creationDateTime (已弃) </span><span class="sxs-lookup"><span data-stu-id="23bb6-134">creationDateTime (Deprecated)</span></span>|<span data-ttu-id="23bb6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23bb6-135">DateTimeOffset</span></span>|<span data-ttu-id="23bb6-136">向用户注册此密钥的时间戳。</span><span class="sxs-lookup"><span data-stu-id="23bb6-136">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="23bb6-137">aaGuid</span><span class="sxs-lookup"><span data-stu-id="23bb6-137">aaGuid</span></span>|<span data-ttu-id="23bb6-138">String</span><span class="sxs-lookup"><span data-stu-id="23bb6-138">String</span></span>|<span data-ttu-id="23bb6-139">Authenticator证明 GUID，一个指示验证 (类型的标识符，例如验证器的) 和型号。</span><span class="sxs-lookup"><span data-stu-id="23bb6-139">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="23bb6-140">model</span><span class="sxs-lookup"><span data-stu-id="23bb6-140">model</span></span>|<span data-ttu-id="23bb6-141">String</span><span class="sxs-lookup"><span data-stu-id="23bb6-141">String</span></span>|<span data-ttu-id="23bb6-142">FIDO2 安全密钥的制造商分配模型。</span><span class="sxs-lookup"><span data-stu-id="23bb6-142">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="23bb6-143">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="23bb6-143">attestationCertificates</span></span>|<span data-ttu-id="23bb6-144">String collection</span><span class="sxs-lookup"><span data-stu-id="23bb6-144">String collection</span></span>|<span data-ttu-id="23bb6-145">证明证书 () 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="23bb6-145">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="23bb6-146">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="23bb6-146">attestationLevel</span></span>|<span data-ttu-id="23bb6-147">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="23bb6-147">attestationLevel</span></span>|<span data-ttu-id="23bb6-148">此 FIDO2 安全密钥的证明级别。</span><span class="sxs-lookup"><span data-stu-id="23bb6-148">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="23bb6-149">可取值为：`attested`、`notAttested`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="23bb6-149">Possible values are: `attested`, `notAttested`, `unknownFutureValue`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="23bb6-150">关系</span><span class="sxs-lookup"><span data-stu-id="23bb6-150">Relationships</span></span>
<span data-ttu-id="23bb6-151">无。</span><span class="sxs-lookup"><span data-stu-id="23bb6-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23bb6-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23bb6-152">JSON representation</span></span>
<span data-ttu-id="23bb6-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23bb6-153">The following is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

