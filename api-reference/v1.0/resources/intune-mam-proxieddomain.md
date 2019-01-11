---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eff345414531b0ddda1600bb567aacd4a5436602
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871111"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="57cb4-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="57cb4-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="57cb4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="57cb4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57cb4-105">代理域</span><span class="sxs-lookup"><span data-stu-id="57cb4-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="57cb4-106">属性</span><span class="sxs-lookup"><span data-stu-id="57cb4-106">Properties</span></span>
|<span data-ttu-id="57cb4-107">属性</span><span class="sxs-lookup"><span data-stu-id="57cb4-107">Property</span></span>|<span data-ttu-id="57cb4-108">类型</span><span class="sxs-lookup"><span data-stu-id="57cb4-108">Type</span></span>|<span data-ttu-id="57cb4-109">说明</span><span class="sxs-lookup"><span data-stu-id="57cb4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57cb4-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="57cb4-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="57cb4-111">String</span><span class="sxs-lookup"><span data-stu-id="57cb4-111">String</span></span>|<span data-ttu-id="57cb4-112">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="57cb4-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="57cb4-113">代理</span><span class="sxs-lookup"><span data-stu-id="57cb4-113">proxy</span></span>|<span data-ttu-id="57cb4-114">String</span><span class="sxs-lookup"><span data-stu-id="57cb4-114">String</span></span>|<span data-ttu-id="57cb4-115">代理 IP</span><span class="sxs-lookup"><span data-stu-id="57cb4-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="57cb4-116">关系</span><span class="sxs-lookup"><span data-stu-id="57cb4-116">Relationships</span></span>
<span data-ttu-id="57cb4-117">无</span><span class="sxs-lookup"><span data-stu-id="57cb4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57cb4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57cb4-118">JSON Representation</span></span>
<span data-ttu-id="57cb4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57cb4-119">Here is a JSON representation of the resource.</span></span>
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



