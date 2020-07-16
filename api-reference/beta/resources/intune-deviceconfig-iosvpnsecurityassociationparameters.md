---
title: iosVpnSecurityAssociationParameters 资源类型
description: VPN 安全关联参数
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85f69b9cf8e19acf09ca0ca179df6cd7fee2fbd9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793897"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="8c76e-103">iosVpnSecurityAssociationParameters 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c76e-103">iosVpnSecurityAssociationParameters resource type</span></span>

<span data-ttu-id="8c76e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c76e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c76e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c76e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c76e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c76e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c76e-107">VPN 安全关联参数</span><span class="sxs-lookup"><span data-stu-id="8c76e-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="8c76e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c76e-108">Properties</span></span>
|<span data-ttu-id="8c76e-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c76e-109">Property</span></span>|<span data-ttu-id="8c76e-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c76e-110">Type</span></span>|<span data-ttu-id="8c76e-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c76e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c76e-112">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8c76e-112">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="8c76e-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="8c76e-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="8c76e-114">加密算法。</span><span class="sxs-lookup"><span data-stu-id="8c76e-114">Encryption algorithm.</span></span> <span data-ttu-id="8c76e-115">可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`、`aes192`、`aes192Gcm`。</span><span class="sxs-lookup"><span data-stu-id="8c76e-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="8c76e-116">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8c76e-116">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="8c76e-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="8c76e-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="8c76e-118">完整性算法。</span><span class="sxs-lookup"><span data-stu-id="8c76e-118">Integrity algorithm.</span></span> <span data-ttu-id="8c76e-119">可取值为：`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512`、`md5`。</span><span class="sxs-lookup"><span data-stu-id="8c76e-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="8c76e-120">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="8c76e-120">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="8c76e-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8c76e-121">Int32</span></span>|<span data-ttu-id="8c76e-122">Diffie-hellman 组</span><span class="sxs-lookup"><span data-stu-id="8c76e-122">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="8c76e-123">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="8c76e-123">lifetimeInMinutes</span></span>|<span data-ttu-id="8c76e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8c76e-124">Int32</span></span>|<span data-ttu-id="8c76e-125">生存时间（分钟）</span><span class="sxs-lookup"><span data-stu-id="8c76e-125">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c76e-126">关系</span><span class="sxs-lookup"><span data-stu-id="8c76e-126">Relationships</span></span>
<span data-ttu-id="8c76e-127">无</span><span class="sxs-lookup"><span data-stu-id="8c76e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c76e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c76e-128">JSON Representation</span></span>
<span data-ttu-id="8c76e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c76e-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```



