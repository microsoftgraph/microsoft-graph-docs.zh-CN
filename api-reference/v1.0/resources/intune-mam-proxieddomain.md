---
title: proxiedDomain 资源类型
description: 代理域
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e437c6bf035d0f6099531fbe5ebf236d30be3a2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448275"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="1799f-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="1799f-103">proxiedDomain resource type</span></span>

<span data-ttu-id="1799f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1799f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1799f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1799f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1799f-106">代理域</span><span class="sxs-lookup"><span data-stu-id="1799f-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="1799f-107">属性</span><span class="sxs-lookup"><span data-stu-id="1799f-107">Properties</span></span>
|<span data-ttu-id="1799f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1799f-108">Property</span></span>|<span data-ttu-id="1799f-109">类型</span><span class="sxs-lookup"><span data-stu-id="1799f-109">Type</span></span>|<span data-ttu-id="1799f-110">说明</span><span class="sxs-lookup"><span data-stu-id="1799f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1799f-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="1799f-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="1799f-112">String</span><span class="sxs-lookup"><span data-stu-id="1799f-112">String</span></span>|<span data-ttu-id="1799f-113">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="1799f-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="1799f-114">代理</span><span class="sxs-lookup"><span data-stu-id="1799f-114">proxy</span></span>|<span data-ttu-id="1799f-115">String</span><span class="sxs-lookup"><span data-stu-id="1799f-115">String</span></span>|<span data-ttu-id="1799f-116">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="1799f-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="1799f-117">关系</span><span class="sxs-lookup"><span data-stu-id="1799f-117">Relationships</span></span>
<span data-ttu-id="1799f-118">无</span><span class="sxs-lookup"><span data-stu-id="1799f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1799f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1799f-119">JSON Representation</span></span>
<span data-ttu-id="1799f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1799f-120">Here is a JSON representation of the resource.</span></span>
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




