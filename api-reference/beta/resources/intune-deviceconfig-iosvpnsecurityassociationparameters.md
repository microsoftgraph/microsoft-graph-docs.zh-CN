---
title: iosVpnSecurityAssociationParameters 资源类型
description: VPN 安全关联参数
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f52d4d05945a29a1eaa44823d13b41eb560f688a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440098"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="a189a-103">iosVpnSecurityAssociationParameters 资源类型</span><span class="sxs-lookup"><span data-stu-id="a189a-103">iosVpnSecurityAssociationParameters resource type</span></span>

<span data-ttu-id="a189a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a189a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a189a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a189a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a189a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a189a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a189a-107">VPN 安全关联参数</span><span class="sxs-lookup"><span data-stu-id="a189a-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="a189a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a189a-108">Properties</span></span>
|<span data-ttu-id="a189a-109">属性</span><span class="sxs-lookup"><span data-stu-id="a189a-109">Property</span></span>|<span data-ttu-id="a189a-110">类型</span><span class="sxs-lookup"><span data-stu-id="a189a-110">Type</span></span>|<span data-ttu-id="a189a-111">说明</span><span class="sxs-lookup"><span data-stu-id="a189a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a189a-112">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a189a-112">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="a189a-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="a189a-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="a189a-114">加密算法。</span><span class="sxs-lookup"><span data-stu-id="a189a-114">Encryption algorithm.</span></span> <span data-ttu-id="a189a-115">可取值为：`aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`。</span><span class="sxs-lookup"><span data-stu-id="a189a-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="a189a-116">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a189a-116">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="a189a-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="a189a-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="a189a-118">完整性算法。</span><span class="sxs-lookup"><span data-stu-id="a189a-118">Integrity algorithm.</span></span> <span data-ttu-id="a189a-119">可取值为：`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512`。</span><span class="sxs-lookup"><span data-stu-id="a189a-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="a189a-120">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="a189a-120">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="a189a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a189a-121">Int32</span></span>|<span data-ttu-id="a189a-122">Diffie-hellman 组</span><span class="sxs-lookup"><span data-stu-id="a189a-122">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="a189a-123">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a189a-123">lifetimeInMinutes</span></span>|<span data-ttu-id="a189a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a189a-124">Int32</span></span>|<span data-ttu-id="a189a-125">生存时间（分钟）</span><span class="sxs-lookup"><span data-stu-id="a189a-125">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a189a-126">关系</span><span class="sxs-lookup"><span data-stu-id="a189a-126">Relationships</span></span>
<span data-ttu-id="a189a-127">无</span><span class="sxs-lookup"><span data-stu-id="a189a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a189a-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a189a-128">JSON Representation</span></span>
<span data-ttu-id="a189a-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a189a-129">Here is a JSON representation of the resource.</span></span>
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



