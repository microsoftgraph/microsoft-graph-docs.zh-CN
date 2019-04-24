---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465277"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="5181d-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="5181d-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="5181d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5181d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5181d-105">代理域</span><span class="sxs-lookup"><span data-stu-id="5181d-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="5181d-106">属性</span><span class="sxs-lookup"><span data-stu-id="5181d-106">Properties</span></span>
|<span data-ttu-id="5181d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5181d-107">Property</span></span>|<span data-ttu-id="5181d-108">类型</span><span class="sxs-lookup"><span data-stu-id="5181d-108">Type</span></span>|<span data-ttu-id="5181d-109">说明</span><span class="sxs-lookup"><span data-stu-id="5181d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5181d-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="5181d-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="5181d-111">String</span><span class="sxs-lookup"><span data-stu-id="5181d-111">String</span></span>|<span data-ttu-id="5181d-112">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="5181d-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="5181d-113">代理</span><span class="sxs-lookup"><span data-stu-id="5181d-113">proxy</span></span>|<span data-ttu-id="5181d-114">String</span><span class="sxs-lookup"><span data-stu-id="5181d-114">String</span></span>|<span data-ttu-id="5181d-115">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="5181d-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="5181d-116">关系</span><span class="sxs-lookup"><span data-stu-id="5181d-116">Relationships</span></span>
<span data-ttu-id="5181d-117">无</span><span class="sxs-lookup"><span data-stu-id="5181d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5181d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5181d-118">JSON Representation</span></span>
<span data-ttu-id="5181d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5181d-119">Here is a JSON representation of the resource.</span></span>
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



