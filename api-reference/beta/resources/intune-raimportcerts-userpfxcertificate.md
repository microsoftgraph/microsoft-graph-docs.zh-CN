---
title: userPFXCertificate 资源类型
description: 封装用户的 PFX 证书所需的所有信息的实体。
localization_priority: Normal
ms.openlocfilehash: 87516c48e53c8117c9efa119fb6cab62844e6b68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809994"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="f6810-103">userPFXCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6810-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="f6810-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f6810-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6810-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6810-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6810-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f6810-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6810-107">封装用户的 PFX 证书所需的所有信息的实体。</span><span class="sxs-lookup"><span data-stu-id="f6810-107">Entity that encapsulates all information required for a user's PFX certificates.</span></span>
## <a name="methods"></a><span data-ttu-id="f6810-108">方法</span><span class="sxs-lookup"><span data-stu-id="f6810-108">Methods</span></span>
|<span data-ttu-id="f6810-109">方法</span><span class="sxs-lookup"><span data-stu-id="f6810-109">Method</span></span>|<span data-ttu-id="f6810-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6810-110">Return Type</span></span>|<span data-ttu-id="f6810-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6810-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6810-112">列表 userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="f6810-112">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="f6810-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6810-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="f6810-114">列出属性和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f6810-114">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="f6810-115">获取 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-115">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="f6810-116">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-116">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="f6810-117">读取属性和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f6810-117">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="f6810-118">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-118">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="f6810-119">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-119">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="f6810-120">创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f6810-120">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="f6810-121">删除 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-121">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="f6810-122">无</span><span class="sxs-lookup"><span data-stu-id="f6810-122">None</span></span>|<span data-ttu-id="f6810-123">删除[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="f6810-123">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="f6810-124">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-124">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="f6810-125">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f6810-125">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="f6810-126">更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f6810-126">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6810-127">属性</span><span class="sxs-lookup"><span data-stu-id="f6810-127">Properties</span></span>
|<span data-ttu-id="f6810-128">属性</span><span class="sxs-lookup"><span data-stu-id="f6810-128">Property</span></span>|<span data-ttu-id="f6810-129">类型</span><span class="sxs-lookup"><span data-stu-id="f6810-129">Type</span></span>|<span data-ttu-id="f6810-130">说明</span><span class="sxs-lookup"><span data-stu-id="f6810-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6810-131">id</span><span class="sxs-lookup"><span data-stu-id="f6810-131">id</span></span>|<span data-ttu-id="f6810-132">字符串</span><span class="sxs-lookup"><span data-stu-id="f6810-132">String</span></span>|<span data-ttu-id="f6810-133">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f6810-133">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="f6810-134">指纹</span><span class="sxs-lookup"><span data-stu-id="f6810-134">thumbprint</span></span>|<span data-ttu-id="f6810-135">字符串</span><span class="sxs-lookup"><span data-stu-id="f6810-135">String</span></span>|<span data-ttu-id="f6810-136">Sha-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="f6810-136">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="f6810-137">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f6810-137">intendedPurpose</span></span>|[<span data-ttu-id="f6810-138">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f6810-138">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="f6810-139">证书的适用于从部署的视图点的用途。</span><span class="sxs-lookup"><span data-stu-id="f6810-139">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="f6810-140">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="f6810-140">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="f6810-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6810-141">userPrincipalName</span></span>|<span data-ttu-id="f6810-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f6810-142">String</span></span>|<span data-ttu-id="f6810-143">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="f6810-143">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="f6810-144">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f6810-144">startDateTime</span></span>|<span data-ttu-id="f6810-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6810-145">DateTimeOffset</span></span>|<span data-ttu-id="f6810-146">证书的有效性开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6810-146">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="f6810-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6810-147">expirationDateTime</span></span>|<span data-ttu-id="f6810-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6810-148">DateTimeOffset</span></span>|<span data-ttu-id="f6810-149">证书的有效性过期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6810-149">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="f6810-150">providerName</span><span class="sxs-lookup"><span data-stu-id="f6810-150">providerName</span></span>|<span data-ttu-id="f6810-151">字符串</span><span class="sxs-lookup"><span data-stu-id="f6810-151">String</span></span>|<span data-ttu-id="f6810-152">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="f6810-152">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="f6810-153">键名</span><span class="sxs-lookup"><span data-stu-id="f6810-153">keyName</span></span>|<span data-ttu-id="f6810-154">字符串</span><span class="sxs-lookup"><span data-stu-id="f6810-154">String</span></span>|<span data-ttu-id="f6810-155">用于加密 blob （在提供程序） 项的名称。</span><span class="sxs-lookup"><span data-stu-id="f6810-155">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="f6810-156">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="f6810-156">paddingScheme</span></span>|[<span data-ttu-id="f6810-157">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="f6810-157">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="f6810-158">填充在加密/解密过程中使用提供程序的方案。</span><span class="sxs-lookup"><span data-stu-id="f6810-158">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="f6810-159">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="f6810-159">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="f6810-160">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="f6810-160">encryptedPfxBlob</span></span>|<span data-ttu-id="f6810-161">Binary</span><span class="sxs-lookup"><span data-stu-id="f6810-161">Binary</span></span>|<span data-ttu-id="f6810-162">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="f6810-162">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="f6810-163">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="f6810-163">encryptedPfxPassword</span></span>|<span data-ttu-id="f6810-164">字符串</span><span class="sxs-lookup"><span data-stu-id="f6810-164">String</span></span>|<span data-ttu-id="f6810-165">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="f6810-165">Encrypted PFX password.</span></span>|
|<span data-ttu-id="f6810-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6810-166">createdDateTime</span></span>|<span data-ttu-id="f6810-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6810-167">DateTimeOffset</span></span>|<span data-ttu-id="f6810-168">日期/时间时此 PFX 证书已导入。</span><span class="sxs-lookup"><span data-stu-id="f6810-168">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="f6810-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6810-169">lastModifiedDateTime</span></span>|<span data-ttu-id="f6810-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6810-170">DateTimeOffset</span></span>|<span data-ttu-id="f6810-171">上次修改此 PFX 证书时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6810-171">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6810-172">Relationships</span><span class="sxs-lookup"><span data-stu-id="f6810-172">Relationships</span></span>
<span data-ttu-id="f6810-173">无</span><span class="sxs-lookup"><span data-stu-id="f6810-173">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6810-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6810-174">JSON Representation</span></span>
<span data-ttu-id="f6810-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6810-175">Here is a JSON representation of the resource.</span></span>
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





