---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需的所有信息的实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5207ebe54ad6dd7f6f5273bfd9062852c4de24f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308140"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="0ecc3-103">userPFXCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ecc3-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="0ecc3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ecc3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ecc3-106">封装用户的 PFX 证书所需的所有信息的实体。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-106">Entity that encapsulates all information required for a user's PFX certificates.</span></span>

## <a name="methods"></a><span data-ttu-id="0ecc3-107">方法</span><span class="sxs-lookup"><span data-stu-id="0ecc3-107">Methods</span></span>
|<span data-ttu-id="0ecc3-108">方法</span><span class="sxs-lookup"><span data-stu-id="0ecc3-108">Method</span></span>|<span data-ttu-id="0ecc3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ecc3-109">Return Type</span></span>|<span data-ttu-id="0ecc3-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ecc3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0ecc3-111">列出 userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="0ecc3-111">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="0ecc3-112">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ecc3-112">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="0ecc3-113">列出[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-113">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="0ecc3-114">获取 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-114">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="0ecc3-115">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-115">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="0ecc3-116">读取[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-116">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="0ecc3-117">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-117">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="0ecc3-118">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-118">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="0ecc3-119">创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-119">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="0ecc3-120">删除 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-120">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="0ecc3-121">无</span><span class="sxs-lookup"><span data-stu-id="0ecc3-121">None</span></span>|<span data-ttu-id="0ecc3-122">删除[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-122">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="0ecc3-123">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-123">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="0ecc3-124">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecc3-124">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="0ecc3-125">更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-125">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ecc3-126">属性</span><span class="sxs-lookup"><span data-stu-id="0ecc3-126">Properties</span></span>
|<span data-ttu-id="0ecc3-127">属性</span><span class="sxs-lookup"><span data-stu-id="0ecc3-127">Property</span></span>|<span data-ttu-id="0ecc3-128">类型</span><span class="sxs-lookup"><span data-stu-id="0ecc3-128">Type</span></span>|<span data-ttu-id="0ecc3-129">说明</span><span class="sxs-lookup"><span data-stu-id="0ecc3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ecc3-130">id</span><span class="sxs-lookup"><span data-stu-id="0ecc3-130">id</span></span>|<span data-ttu-id="0ecc3-131">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-131">String</span></span>|<span data-ttu-id="0ecc3-132">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-132">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="0ecc3-133">为</span><span class="sxs-lookup"><span data-stu-id="0ecc3-133">thumbprint</span></span>|<span data-ttu-id="0ecc3-134">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-134">String</span></span>|<span data-ttu-id="0ecc3-135">SHA-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-135">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="0ecc3-136">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0ecc3-136">intendedPurpose</span></span>|[<span data-ttu-id="0ecc3-137">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0ecc3-137">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="0ecc3-138">证书的预期目的是从部署的角度来看。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-138">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="0ecc3-139">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-139">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="0ecc3-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ecc3-140">userPrincipalName</span></span>|<span data-ttu-id="0ecc3-141">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-141">String</span></span>|<span data-ttu-id="0ecc3-142">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-142">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="0ecc3-143">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecc3-143">startDateTime</span></span>|<span data-ttu-id="0ecc3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecc3-144">DateTimeOffset</span></span>|<span data-ttu-id="0ecc3-145">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-145">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="0ecc3-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecc3-146">expirationDateTime</span></span>|<span data-ttu-id="0ecc3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecc3-147">DateTimeOffset</span></span>|<span data-ttu-id="0ecc3-148">证书的有效期到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-148">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="0ecc3-149">providerName</span><span class="sxs-lookup"><span data-stu-id="0ecc3-149">providerName</span></span>|<span data-ttu-id="0ecc3-150">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-150">String</span></span>|<span data-ttu-id="0ecc3-151">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-151">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="0ecc3-152">名</span><span class="sxs-lookup"><span data-stu-id="0ecc3-152">keyName</span></span>|<span data-ttu-id="0ecc3-153">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-153">String</span></span>|<span data-ttu-id="0ecc3-154">用于对 blob 进行加密的密钥 (在提供程序中) 的名称。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-154">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="0ecc3-155">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="0ecc3-155">paddingScheme</span></span>|[<span data-ttu-id="0ecc3-156">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="0ecc3-156">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="0ecc3-157">加密/解密过程中提供程序使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-157">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="0ecc3-158">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-158">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="0ecc3-159">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="0ecc3-159">encryptedPfxBlob</span></span>|<span data-ttu-id="0ecc3-160">Binary</span><span class="sxs-lookup"><span data-stu-id="0ecc3-160">Binary</span></span>|<span data-ttu-id="0ecc3-161">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-161">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="0ecc3-162">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="0ecc3-162">encryptedPfxPassword</span></span>|<span data-ttu-id="0ecc3-163">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-163">String</span></span>|<span data-ttu-id="0ecc3-164">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-164">Encrypted PFX password.</span></span>|
|<span data-ttu-id="0ecc3-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecc3-165">createdDateTime</span></span>|<span data-ttu-id="0ecc3-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecc3-166">DateTimeOffset</span></span>|<span data-ttu-id="0ecc3-167">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-167">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="0ecc3-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecc3-168">lastModifiedDateTime</span></span>|<span data-ttu-id="0ecc3-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecc3-169">DateTimeOffset</span></span>|<span data-ttu-id="0ecc3-170">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-170">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ecc3-171">关系</span><span class="sxs-lookup"><span data-stu-id="0ecc3-171">Relationships</span></span>
<span data-ttu-id="0ecc3-172">无</span><span class="sxs-lookup"><span data-stu-id="0ecc3-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ecc3-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ecc3-173">JSON Representation</span></span>
<span data-ttu-id="0ecc3-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ecc3-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



