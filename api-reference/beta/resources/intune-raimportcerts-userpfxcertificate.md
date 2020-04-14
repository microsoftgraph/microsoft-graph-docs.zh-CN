---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需的所有信息的实体。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43dc26333b6acf6275a719e7a79c051a134610f7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462375"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="e315a-103">userPFXCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="e315a-103">userPFXCertificate resource type</span></span>

<span data-ttu-id="e315a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e315a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e315a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e315a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e315a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e315a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e315a-107">封装用户的 PFX 证书所需的所有信息的实体。</span><span class="sxs-lookup"><span data-stu-id="e315a-107">Entity that encapsulates all information required for a user's PFX certificates.</span></span>

## <a name="methods"></a><span data-ttu-id="e315a-108">方法</span><span class="sxs-lookup"><span data-stu-id="e315a-108">Methods</span></span>
|<span data-ttu-id="e315a-109">方法</span><span class="sxs-lookup"><span data-stu-id="e315a-109">Method</span></span>|<span data-ttu-id="e315a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e315a-110">Return Type</span></span>|<span data-ttu-id="e315a-111">说明</span><span class="sxs-lookup"><span data-stu-id="e315a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e315a-112">列出 userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="e315a-112">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="e315a-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e315a-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="e315a-114">列出[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e315a-114">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="e315a-115">获取 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-115">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="e315a-116">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-116">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="e315a-117">读取[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e315a-117">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="e315a-118">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-118">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="e315a-119">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-119">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="e315a-120">创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e315a-120">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="e315a-121">删除 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-121">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="e315a-122">无</span><span class="sxs-lookup"><span data-stu-id="e315a-122">None</span></span>|<span data-ttu-id="e315a-123">删除[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="e315a-123">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="e315a-124">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-124">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="e315a-125">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="e315a-125">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="e315a-126">更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e315a-126">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e315a-127">属性</span><span class="sxs-lookup"><span data-stu-id="e315a-127">Properties</span></span>
|<span data-ttu-id="e315a-128">属性</span><span class="sxs-lookup"><span data-stu-id="e315a-128">Property</span></span>|<span data-ttu-id="e315a-129">类型</span><span class="sxs-lookup"><span data-stu-id="e315a-129">Type</span></span>|<span data-ttu-id="e315a-130">说明</span><span class="sxs-lookup"><span data-stu-id="e315a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e315a-131">id</span><span class="sxs-lookup"><span data-stu-id="e315a-131">id</span></span>|<span data-ttu-id="e315a-132">String</span><span class="sxs-lookup"><span data-stu-id="e315a-132">String</span></span>|<span data-ttu-id="e315a-133">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e315a-133">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="e315a-134">为</span><span class="sxs-lookup"><span data-stu-id="e315a-134">thumbprint</span></span>|<span data-ttu-id="e315a-135">String</span><span class="sxs-lookup"><span data-stu-id="e315a-135">String</span></span>|<span data-ttu-id="e315a-136">SHA-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="e315a-136">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="e315a-137">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="e315a-137">intendedPurpose</span></span>|[<span data-ttu-id="e315a-138">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="e315a-138">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="e315a-139">证书的预期目的是从部署的角度来看。</span><span class="sxs-lookup"><span data-stu-id="e315a-139">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="e315a-140">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="e315a-140">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="e315a-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e315a-141">userPrincipalName</span></span>|<span data-ttu-id="e315a-142">String</span><span class="sxs-lookup"><span data-stu-id="e315a-142">String</span></span>|<span data-ttu-id="e315a-143">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e315a-143">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="e315a-144">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e315a-144">startDateTime</span></span>|<span data-ttu-id="e315a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e315a-145">DateTimeOffset</span></span>|<span data-ttu-id="e315a-146">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e315a-146">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="e315a-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e315a-147">expirationDateTime</span></span>|<span data-ttu-id="e315a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e315a-148">DateTimeOffset</span></span>|<span data-ttu-id="e315a-149">证书的有效期到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e315a-149">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="e315a-150">providerName</span><span class="sxs-lookup"><span data-stu-id="e315a-150">providerName</span></span>|<span data-ttu-id="e315a-151">String</span><span class="sxs-lookup"><span data-stu-id="e315a-151">String</span></span>|<span data-ttu-id="e315a-152">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="e315a-152">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="e315a-153">名</span><span class="sxs-lookup"><span data-stu-id="e315a-153">keyName</span></span>|<span data-ttu-id="e315a-154">String</span><span class="sxs-lookup"><span data-stu-id="e315a-154">String</span></span>|<span data-ttu-id="e315a-155">用于对 blob 进行加密的密钥（在提供程序中）的名称。</span><span class="sxs-lookup"><span data-stu-id="e315a-155">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="e315a-156">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="e315a-156">paddingScheme</span></span>|[<span data-ttu-id="e315a-157">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="e315a-157">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="e315a-158">加密/解密过程中提供程序使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="e315a-158">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="e315a-159">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="e315a-159">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="e315a-160">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="e315a-160">encryptedPfxBlob</span></span>|<span data-ttu-id="e315a-161">Binary</span><span class="sxs-lookup"><span data-stu-id="e315a-161">Binary</span></span>|<span data-ttu-id="e315a-162">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="e315a-162">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="e315a-163">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="e315a-163">encryptedPfxPassword</span></span>|<span data-ttu-id="e315a-164">String</span><span class="sxs-lookup"><span data-stu-id="e315a-164">String</span></span>|<span data-ttu-id="e315a-165">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="e315a-165">Encrypted PFX password.</span></span>|
|<span data-ttu-id="e315a-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e315a-166">createdDateTime</span></span>|<span data-ttu-id="e315a-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e315a-167">DateTimeOffset</span></span>|<span data-ttu-id="e315a-168">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e315a-168">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="e315a-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e315a-169">lastModifiedDateTime</span></span>|<span data-ttu-id="e315a-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e315a-170">DateTimeOffset</span></span>|<span data-ttu-id="e315a-171">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e315a-171">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e315a-172">关系</span><span class="sxs-lookup"><span data-stu-id="e315a-172">Relationships</span></span>
<span data-ttu-id="e315a-173">无</span><span class="sxs-lookup"><span data-stu-id="e315a-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e315a-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e315a-174">JSON Representation</span></span>
<span data-ttu-id="e315a-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e315a-175">Here is a JSON representation of the resource.</span></span>
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



