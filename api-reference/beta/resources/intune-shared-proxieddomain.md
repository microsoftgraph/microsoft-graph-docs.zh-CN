---
title: proxiedDomain 资源类型
description: 代理域
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bdfdf1fdbea81f415633c810bd21172164f3765f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768056"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="6d710-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d710-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="6d710-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d710-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d710-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d710-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d710-106">代理域</span><span class="sxs-lookup"><span data-stu-id="6d710-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="6d710-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d710-107">Properties</span></span>
|<span data-ttu-id="6d710-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d710-108">Property</span></span>|<span data-ttu-id="6d710-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d710-109">Type</span></span>|<span data-ttu-id="6d710-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d710-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d710-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="6d710-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="6d710-112">String</span><span class="sxs-lookup"><span data-stu-id="6d710-112">String</span></span>|<span data-ttu-id="6d710-113">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="6d710-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="6d710-114">代理</span><span class="sxs-lookup"><span data-stu-id="6d710-114">proxy</span></span>|<span data-ttu-id="6d710-115">String</span><span class="sxs-lookup"><span data-stu-id="6d710-115">String</span></span>|<span data-ttu-id="6d710-116">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="6d710-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d710-117">关系</span><span class="sxs-lookup"><span data-stu-id="6d710-117">Relationships</span></span>
<span data-ttu-id="6d710-118">无</span><span class="sxs-lookup"><span data-stu-id="6d710-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d710-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d710-119">JSON Representation</span></span>
<span data-ttu-id="6d710-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d710-120">Here is a JSON representation of the resource.</span></span>
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



