---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5edabc31761a3abd79a94bb700392923d2d54513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151203"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="433e8-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="433e8-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="433e8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="433e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="433e8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="433e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="433e8-106">代理域</span><span class="sxs-lookup"><span data-stu-id="433e8-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="433e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="433e8-107">Properties</span></span>
|<span data-ttu-id="433e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="433e8-108">Property</span></span>|<span data-ttu-id="433e8-109">类型</span><span class="sxs-lookup"><span data-stu-id="433e8-109">Type</span></span>|<span data-ttu-id="433e8-110">说明</span><span class="sxs-lookup"><span data-stu-id="433e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="433e8-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="433e8-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="433e8-112">String</span><span class="sxs-lookup"><span data-stu-id="433e8-112">String</span></span>|<span data-ttu-id="433e8-113">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="433e8-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="433e8-114">代理</span><span class="sxs-lookup"><span data-stu-id="433e8-114">proxy</span></span>|<span data-ttu-id="433e8-115">String</span><span class="sxs-lookup"><span data-stu-id="433e8-115">String</span></span>|<span data-ttu-id="433e8-116">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="433e8-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="433e8-117">关系</span><span class="sxs-lookup"><span data-stu-id="433e8-117">Relationships</span></span>
<span data-ttu-id="433e8-118">无</span><span class="sxs-lookup"><span data-stu-id="433e8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="433e8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="433e8-119">JSON Representation</span></span>
<span data-ttu-id="433e8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="433e8-120">Here is a JSON representation of the resource.</span></span>
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




