---
title: iosVpnSecurityAssociationParameters 资源类型
description: VPN 安全关联参数
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3da905a68222b60bef7225f34afc2b4a0b39a50
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790494"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="359af-103">iosVpnSecurityAssociationParameters 资源类型</span><span class="sxs-lookup"><span data-stu-id="359af-103">iosVpnSecurityAssociationParameters resource type</span></span>

> <span data-ttu-id="359af-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="359af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="359af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="359af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="359af-106">VPN 安全关联参数</span><span class="sxs-lookup"><span data-stu-id="359af-106">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="359af-107">属性</span><span class="sxs-lookup"><span data-stu-id="359af-107">Properties</span></span>
|<span data-ttu-id="359af-108">属性</span><span class="sxs-lookup"><span data-stu-id="359af-108">Property</span></span>|<span data-ttu-id="359af-109">类型</span><span class="sxs-lookup"><span data-stu-id="359af-109">Type</span></span>|<span data-ttu-id="359af-110">说明</span><span class="sxs-lookup"><span data-stu-id="359af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="359af-111">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="359af-111">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="359af-112">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="359af-112">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="359af-113">加密算法。</span><span class="sxs-lookup"><span data-stu-id="359af-113">Encryption algorithm.</span></span> <span data-ttu-id="359af-114">可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`。</span><span class="sxs-lookup"><span data-stu-id="359af-114">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="359af-115">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="359af-115">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="359af-116">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="359af-116">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="359af-117">完整性算法。</span><span class="sxs-lookup"><span data-stu-id="359af-117">Integrity algorithm.</span></span> <span data-ttu-id="359af-118">可取值为：`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512`。</span><span class="sxs-lookup"><span data-stu-id="359af-118">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="359af-119">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="359af-119">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="359af-120">Int32</span><span class="sxs-lookup"><span data-stu-id="359af-120">Int32</span></span>|<span data-ttu-id="359af-121">Diffie-hellman 组</span><span class="sxs-lookup"><span data-stu-id="359af-121">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="359af-122">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="359af-122">lifetimeInMinutes</span></span>|<span data-ttu-id="359af-123">Int32</span><span class="sxs-lookup"><span data-stu-id="359af-123">Int32</span></span>|<span data-ttu-id="359af-124">生存时间（分钟）</span><span class="sxs-lookup"><span data-stu-id="359af-124">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="359af-125">关系</span><span class="sxs-lookup"><span data-stu-id="359af-125">Relationships</span></span>
<span data-ttu-id="359af-126">无</span><span class="sxs-lookup"><span data-stu-id="359af-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="359af-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="359af-127">JSON Representation</span></span>
<span data-ttu-id="359af-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="359af-128">Here is a JSON representation of the resource.</span></span>
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



