---
title: specifiedCaptiveNetworkPlugins 资源类型
description: 指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d205218aab1ef6fb5a59280ff25f5a22fde8c0b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636091"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="98675-103">specifiedCaptiveNetworkPlugins 资源类型</span><span class="sxs-lookup"><span data-stu-id="98675-103">specifiedCaptiveNetworkPlugins resource type</span></span>

> <span data-ttu-id="98675-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98675-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98675-106">指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件</span><span class="sxs-lookup"><span data-stu-id="98675-106">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="98675-107">属性</span><span class="sxs-lookup"><span data-stu-id="98675-107">Properties</span></span>
|<span data-ttu-id="98675-108">属性</span><span class="sxs-lookup"><span data-stu-id="98675-108">Property</span></span>|<span data-ttu-id="98675-109">类型</span><span class="sxs-lookup"><span data-stu-id="98675-109">Type</span></span>|<span data-ttu-id="98675-110">Description</span><span class="sxs-lookup"><span data-stu-id="98675-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98675-111">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="98675-111">allowedBundleIdentifiers</span></span>|<span data-ttu-id="98675-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="98675-112">String collection</span></span>|<span data-ttu-id="98675-113">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="98675-113">Address of the IKEv2 server.</span></span> <span data-ttu-id="98675-114">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="98675-114">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="98675-115">关系</span><span class="sxs-lookup"><span data-stu-id="98675-115">Relationships</span></span>
<span data-ttu-id="98675-116">无</span><span class="sxs-lookup"><span data-stu-id="98675-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98675-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98675-117">JSON Representation</span></span>
<span data-ttu-id="98675-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98675-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



