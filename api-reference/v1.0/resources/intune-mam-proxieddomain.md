---
title: proxiedDomain 资源类型
description: 代理域
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d4b100fd312576fdb81f09e06b51d7e74bef4c0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366956"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="b3a89-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3a89-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="b3a89-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3a89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3a89-105">代理域</span><span class="sxs-lookup"><span data-stu-id="b3a89-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="b3a89-106">属性</span><span class="sxs-lookup"><span data-stu-id="b3a89-106">Properties</span></span>
|<span data-ttu-id="b3a89-107">属性</span><span class="sxs-lookup"><span data-stu-id="b3a89-107">Property</span></span>|<span data-ttu-id="b3a89-108">类型</span><span class="sxs-lookup"><span data-stu-id="b3a89-108">Type</span></span>|<span data-ttu-id="b3a89-109">说明</span><span class="sxs-lookup"><span data-stu-id="b3a89-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3a89-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="b3a89-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="b3a89-111">String</span><span class="sxs-lookup"><span data-stu-id="b3a89-111">String</span></span>|<span data-ttu-id="b3a89-112">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="b3a89-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="b3a89-113">代理</span><span class="sxs-lookup"><span data-stu-id="b3a89-113">proxy</span></span>|<span data-ttu-id="b3a89-114">String</span><span class="sxs-lookup"><span data-stu-id="b3a89-114">String</span></span>|<span data-ttu-id="b3a89-115">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="b3a89-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3a89-116">关系</span><span class="sxs-lookup"><span data-stu-id="b3a89-116">Relationships</span></span>
<span data-ttu-id="b3a89-117">无</span><span class="sxs-lookup"><span data-stu-id="b3a89-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3a89-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3a89-118">JSON Representation</span></span>
<span data-ttu-id="b3a89-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3a89-119">Here is a JSON representation of the resource.</span></span>
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




