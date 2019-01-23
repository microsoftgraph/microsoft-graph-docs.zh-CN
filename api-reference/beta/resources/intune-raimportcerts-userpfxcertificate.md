---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需的所有信息的实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 95ae97b44a82d5ec87e3e2622a519debcfd8d7c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406036"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="82e62-103">userPFXCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="82e62-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="82e62-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="82e62-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82e62-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="82e62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82e62-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82e62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82e62-107">封装用户的 PFX 证书所需的所有信息的实体。</span><span class="sxs-lookup"><span data-stu-id="82e62-107">Entity that encapsulates all information required for a user's PFX certificates.</span></span>

## <a name="methods"></a><span data-ttu-id="82e62-108">方法</span><span class="sxs-lookup"><span data-stu-id="82e62-108">Methods</span></span>
|<span data-ttu-id="82e62-109">方法</span><span class="sxs-lookup"><span data-stu-id="82e62-109">Method</span></span>|<span data-ttu-id="82e62-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="82e62-110">Return Type</span></span>|<span data-ttu-id="82e62-111">说明</span><span class="sxs-lookup"><span data-stu-id="82e62-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="82e62-112">列表 userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="82e62-112">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="82e62-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合</span><span class="sxs-lookup"><span data-stu-id="82e62-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="82e62-114">列出属性和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="82e62-114">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="82e62-115">获取 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-115">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="82e62-116">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-116">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="82e62-117">读取属性和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="82e62-117">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="82e62-118">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-118">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="82e62-119">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-119">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="82e62-120">创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82e62-120">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="82e62-121">删除 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-121">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="82e62-122">无</span><span class="sxs-lookup"><span data-stu-id="82e62-122">None</span></span>|<span data-ttu-id="82e62-123">删除[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="82e62-123">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="82e62-124">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-124">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="82e62-125">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="82e62-125">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="82e62-126">更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82e62-126">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="82e62-127">属性</span><span class="sxs-lookup"><span data-stu-id="82e62-127">Properties</span></span>
|<span data-ttu-id="82e62-128">属性</span><span class="sxs-lookup"><span data-stu-id="82e62-128">Property</span></span>|<span data-ttu-id="82e62-129">类型</span><span class="sxs-lookup"><span data-stu-id="82e62-129">Type</span></span>|<span data-ttu-id="82e62-130">说明</span><span class="sxs-lookup"><span data-stu-id="82e62-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82e62-131">id</span><span class="sxs-lookup"><span data-stu-id="82e62-131">id</span></span>|<span data-ttu-id="82e62-132">String</span><span class="sxs-lookup"><span data-stu-id="82e62-132">String</span></span>|<span data-ttu-id="82e62-133">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="82e62-133">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="82e62-134">指纹</span><span class="sxs-lookup"><span data-stu-id="82e62-134">thumbprint</span></span>|<span data-ttu-id="82e62-135">String</span><span class="sxs-lookup"><span data-stu-id="82e62-135">String</span></span>|<span data-ttu-id="82e62-136">Sha-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="82e62-136">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="82e62-137">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="82e62-137">intendedPurpose</span></span>|[<span data-ttu-id="82e62-138">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="82e62-138">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="82e62-139">证书的适用于从部署的视图点的用途。</span><span class="sxs-lookup"><span data-stu-id="82e62-139">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="82e62-140">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="82e62-140">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="82e62-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82e62-141">userPrincipalName</span></span>|<span data-ttu-id="82e62-142">String</span><span class="sxs-lookup"><span data-stu-id="82e62-142">String</span></span>|<span data-ttu-id="82e62-143">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="82e62-143">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="82e62-144">startDateTime</span><span class="sxs-lookup"><span data-stu-id="82e62-144">startDateTime</span></span>|<span data-ttu-id="82e62-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82e62-145">DateTimeOffset</span></span>|<span data-ttu-id="82e62-146">证书的有效性开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82e62-146">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="82e62-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="82e62-147">expirationDateTime</span></span>|<span data-ttu-id="82e62-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82e62-148">DateTimeOffset</span></span>|<span data-ttu-id="82e62-149">证书的有效性过期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82e62-149">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="82e62-150">providerName</span><span class="sxs-lookup"><span data-stu-id="82e62-150">providerName</span></span>|<span data-ttu-id="82e62-151">String</span><span class="sxs-lookup"><span data-stu-id="82e62-151">String</span></span>|<span data-ttu-id="82e62-152">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="82e62-152">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="82e62-153">键名</span><span class="sxs-lookup"><span data-stu-id="82e62-153">keyName</span></span>|<span data-ttu-id="82e62-154">String</span><span class="sxs-lookup"><span data-stu-id="82e62-154">String</span></span>|<span data-ttu-id="82e62-155">用于加密 blob （在提供程序） 项的名称。</span><span class="sxs-lookup"><span data-stu-id="82e62-155">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="82e62-156">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="82e62-156">paddingScheme</span></span>|[<span data-ttu-id="82e62-157">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="82e62-157">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="82e62-158">填充在加密/解密过程中使用提供程序的方案。</span><span class="sxs-lookup"><span data-stu-id="82e62-158">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="82e62-159">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="82e62-159">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="82e62-160">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="82e62-160">encryptedPfxBlob</span></span>|<span data-ttu-id="82e62-161">Binary</span><span class="sxs-lookup"><span data-stu-id="82e62-161">Binary</span></span>|<span data-ttu-id="82e62-162">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="82e62-162">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="82e62-163">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="82e62-163">encryptedPfxPassword</span></span>|<span data-ttu-id="82e62-164">String</span><span class="sxs-lookup"><span data-stu-id="82e62-164">String</span></span>|<span data-ttu-id="82e62-165">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="82e62-165">Encrypted PFX password.</span></span>|
|<span data-ttu-id="82e62-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82e62-166">createdDateTime</span></span>|<span data-ttu-id="82e62-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82e62-167">DateTimeOffset</span></span>|<span data-ttu-id="82e62-168">日期/时间时此 PFX 证书已导入。</span><span class="sxs-lookup"><span data-stu-id="82e62-168">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="82e62-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82e62-169">lastModifiedDateTime</span></span>|<span data-ttu-id="82e62-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82e62-170">DateTimeOffset</span></span>|<span data-ttu-id="82e62-171">上次修改此 PFX 证书时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82e62-171">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82e62-172">关系</span><span class="sxs-lookup"><span data-stu-id="82e62-172">Relationships</span></span>
<span data-ttu-id="82e62-173">无</span><span class="sxs-lookup"><span data-stu-id="82e62-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82e62-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82e62-174">JSON Representation</span></span>
<span data-ttu-id="82e62-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82e62-175">Here is a JSON representation of the resource.</span></span>
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




