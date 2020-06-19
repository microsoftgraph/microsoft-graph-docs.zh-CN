---
title: cryptographySuite 资源类型
description: VPN 安全关联参数
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c09525fdc65a64272901a8823fe9a3fffbecb62
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790255"
---
# <a name="cryptographysuite-resource-type"></a><span data-ttu-id="97c0b-103">cryptographySuite 资源类型</span><span class="sxs-lookup"><span data-stu-id="97c0b-103">cryptographySuite resource type</span></span>

<span data-ttu-id="97c0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97c0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97c0b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97c0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97c0b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97c0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97c0b-107">VPN 安全关联参数</span><span class="sxs-lookup"><span data-stu-id="97c0b-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="97c0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="97c0b-108">Properties</span></span>
|<span data-ttu-id="97c0b-109">属性</span><span class="sxs-lookup"><span data-stu-id="97c0b-109">Property</span></span>|<span data-ttu-id="97c0b-110">类型</span><span class="sxs-lookup"><span data-stu-id="97c0b-110">Type</span></span>|<span data-ttu-id="97c0b-111">说明</span><span class="sxs-lookup"><span data-stu-id="97c0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c0b-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="97c0b-112">encryptionMethod</span></span>|[<span data-ttu-id="97c0b-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="97c0b-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="97c0b-114">加密方法。</span><span class="sxs-lookup"><span data-stu-id="97c0b-114">Encryption Method.</span></span> <span data-ttu-id="97c0b-115">可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`、`aes192`、`aes192Gcm`。</span><span class="sxs-lookup"><span data-stu-id="97c0b-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="97c0b-116">integrityCheckMethod</span><span class="sxs-lookup"><span data-stu-id="97c0b-116">integrityCheckMethod</span></span>|[<span data-ttu-id="97c0b-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="97c0b-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="97c0b-118">完整性检查方法。</span><span class="sxs-lookup"><span data-stu-id="97c0b-118">Integrity Check Method.</span></span> <span data-ttu-id="97c0b-119">可取值为：`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512`、`md5`。</span><span class="sxs-lookup"><span data-stu-id="97c0b-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="97c0b-120">dhGroup</span><span class="sxs-lookup"><span data-stu-id="97c0b-120">dhGroup</span></span>|[<span data-ttu-id="97c0b-121">diffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="97c0b-121">diffieHellmanGroup</span></span>](../resources/intune-deviceconfig-diffiehellmangroup.md)|<span data-ttu-id="97c0b-122">Diffie-hellman 组。</span><span class="sxs-lookup"><span data-stu-id="97c0b-122">Diffie Hellman Group.</span></span> <span data-ttu-id="97c0b-123">可取值为：`group1`、`group2`、`group14`、`ecp256`、`ecp384`、`group24`。</span><span class="sxs-lookup"><span data-stu-id="97c0b-123">Possible values are: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span></span>|
|<span data-ttu-id="97c0b-124">cipherTransformConstants</span><span class="sxs-lookup"><span data-stu-id="97c0b-124">cipherTransformConstants</span></span>|[<span data-ttu-id="97c0b-125">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="97c0b-125">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="97c0b-126">密码转换常量。</span><span class="sxs-lookup"><span data-stu-id="97c0b-126">Cipher Transform Constants.</span></span> <span data-ttu-id="97c0b-127">可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`、`aes192`、`aes192Gcm`。</span><span class="sxs-lookup"><span data-stu-id="97c0b-127">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="97c0b-128">authenticationTransformConstants</span><span class="sxs-lookup"><span data-stu-id="97c0b-128">authenticationTransformConstants</span></span>|[<span data-ttu-id="97c0b-129">authenticationTransformConstant</span><span class="sxs-lookup"><span data-stu-id="97c0b-129">authenticationTransformConstant</span></span>](../resources/intune-deviceconfig-authenticationtransformconstant.md)|<span data-ttu-id="97c0b-130">身份验证转换常量。</span><span class="sxs-lookup"><span data-stu-id="97c0b-130">Authentication Transform Constants.</span></span> <span data-ttu-id="97c0b-131">可取值为：`md5_96`、`sha1_96`、`sha_256_128`、`aes128Gcm`、`aes192Gcm`、`aes256Gcm`。</span><span class="sxs-lookup"><span data-stu-id="97c0b-131">Possible values are: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="97c0b-132">pfsGroup</span><span class="sxs-lookup"><span data-stu-id="97c0b-132">pfsGroup</span></span>|[<span data-ttu-id="97c0b-133">perfectForwardSecrecyGroup</span><span class="sxs-lookup"><span data-stu-id="97c0b-133">perfectForwardSecrecyGroup</span></span>](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|<span data-ttu-id="97c0b-134">"完全转发" 保密组。</span><span class="sxs-lookup"><span data-stu-id="97c0b-134">Perfect Forward Secrecy Group.</span></span> <span data-ttu-id="97c0b-135">可取值为：`pfs1`、`pfs2`、`pfs2048`、`ecp256`、`ecp384`、`pfsMM`、`pfs24`。</span><span class="sxs-lookup"><span data-stu-id="97c0b-135">Possible values are: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97c0b-136">关系</span><span class="sxs-lookup"><span data-stu-id="97c0b-136">Relationships</span></span>
<span data-ttu-id="97c0b-137">无</span><span class="sxs-lookup"><span data-stu-id="97c0b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97c0b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97c0b-138">JSON Representation</span></span>
<span data-ttu-id="97c0b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97c0b-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cryptographySuite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cryptographySuite",
  "encryptionMethod": "String",
  "integrityCheckMethod": "String",
  "dhGroup": "String",
  "cipherTransformConstants": "String",
  "authenticationTransformConstants": "String",
  "pfsGroup": "String"
}
```



