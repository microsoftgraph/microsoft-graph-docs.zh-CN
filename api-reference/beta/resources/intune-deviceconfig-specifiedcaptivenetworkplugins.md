---
title: specifiedCaptiveNetworkPlugins 资源类型
description: 指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6752e045817e9a03eefae178d7df15d152f0ea58
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412767"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="8e2c9-103">specifiedCaptiveNetworkPlugins 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e2c9-103">specifiedCaptiveNetworkPlugins resource type</span></span>

<span data-ttu-id="8e2c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e2c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e2c9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e2c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e2c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e2c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e2c9-107">指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件</span><span class="sxs-lookup"><span data-stu-id="8e2c9-107">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="8e2c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e2c9-108">Properties</span></span>
|<span data-ttu-id="8e2c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e2c9-109">Property</span></span>|<span data-ttu-id="8e2c9-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e2c9-110">Type</span></span>|<span data-ttu-id="8e2c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e2c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e2c9-112">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="8e2c9-112">allowedBundleIdentifiers</span></span>|<span data-ttu-id="8e2c9-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="8e2c9-113">String collection</span></span>|<span data-ttu-id="8e2c9-114">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="8e2c9-114">Address of the IKEv2 server.</span></span> <span data-ttu-id="8e2c9-115">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="8e2c9-115">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e2c9-116">关系</span><span class="sxs-lookup"><span data-stu-id="8e2c9-116">Relationships</span></span>
<span data-ttu-id="8e2c9-117">无</span><span class="sxs-lookup"><span data-stu-id="8e2c9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e2c9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e2c9-118">JSON Representation</span></span>
<span data-ttu-id="8e2c9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e2c9-119">Here is a JSON representation of the resource.</span></span>
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



