---
title: proxiedDomain 资源类型
description: 代理域
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac366425621867e75dfc1a0c1ae8b09336ed0214
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704691"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="e5afb-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5afb-103">proxiedDomain resource type</span></span>

<span data-ttu-id="e5afb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5afb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5afb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5afb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5afb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5afb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5afb-107">代理域</span><span class="sxs-lookup"><span data-stu-id="e5afb-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="e5afb-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5afb-108">Properties</span></span>
|<span data-ttu-id="e5afb-109">属性</span><span class="sxs-lookup"><span data-stu-id="e5afb-109">Property</span></span>|<span data-ttu-id="e5afb-110">类型</span><span class="sxs-lookup"><span data-stu-id="e5afb-110">Type</span></span>|<span data-ttu-id="e5afb-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5afb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5afb-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="e5afb-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="e5afb-113">String</span><span class="sxs-lookup"><span data-stu-id="e5afb-113">String</span></span>|<span data-ttu-id="e5afb-114">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="e5afb-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="e5afb-115">代理</span><span class="sxs-lookup"><span data-stu-id="e5afb-115">proxy</span></span>|<span data-ttu-id="e5afb-116">String</span><span class="sxs-lookup"><span data-stu-id="e5afb-116">String</span></span>|<span data-ttu-id="e5afb-117">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="e5afb-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5afb-118">关系</span><span class="sxs-lookup"><span data-stu-id="e5afb-118">Relationships</span></span>
<span data-ttu-id="e5afb-119">无</span><span class="sxs-lookup"><span data-stu-id="e5afb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5afb-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5afb-120">JSON Representation</span></span>
<span data-ttu-id="e5afb-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5afb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```





