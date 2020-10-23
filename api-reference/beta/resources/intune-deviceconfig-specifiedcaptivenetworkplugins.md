---
title: specifiedCaptiveNetworkPlugins 资源类型
description: 指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 48eb34968901e388ae90334ed372bd776a48aaff
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693813"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="d0cce-103">specifiedCaptiveNetworkPlugins 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0cce-103">specifiedCaptiveNetworkPlugins resource type</span></span>

<span data-ttu-id="d0cce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0cce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0cce-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0cce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0cce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0cce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0cce-107">指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件</span><span class="sxs-lookup"><span data-stu-id="d0cce-107">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="d0cce-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0cce-108">Properties</span></span>
|<span data-ttu-id="d0cce-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0cce-109">Property</span></span>|<span data-ttu-id="d0cce-110">类型</span><span class="sxs-lookup"><span data-stu-id="d0cce-110">Type</span></span>|<span data-ttu-id="d0cce-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0cce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0cce-112">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="d0cce-112">allowedBundleIdentifiers</span></span>|<span data-ttu-id="d0cce-113">String collection</span><span class="sxs-lookup"><span data-stu-id="d0cce-113">String collection</span></span>|<span data-ttu-id="d0cce-114">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="d0cce-114">Address of the IKEv2 server.</span></span> <span data-ttu-id="d0cce-115">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="d0cce-115">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0cce-116">关系</span><span class="sxs-lookup"><span data-stu-id="d0cce-116">Relationships</span></span>
<span data-ttu-id="d0cce-117">无</span><span class="sxs-lookup"><span data-stu-id="d0cce-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0cce-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0cce-118">JSON Representation</span></span>
<span data-ttu-id="d0cce-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0cce-119">Here is a JSON representation of the resource.</span></span>
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





