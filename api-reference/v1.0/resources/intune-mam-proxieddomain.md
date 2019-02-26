---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264041"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="0f12b-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f12b-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="0f12b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f12b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f12b-105">代理域</span><span class="sxs-lookup"><span data-stu-id="0f12b-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="0f12b-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f12b-106">Properties</span></span>
|<span data-ttu-id="0f12b-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f12b-107">Property</span></span>|<span data-ttu-id="0f12b-108">类型</span><span class="sxs-lookup"><span data-stu-id="0f12b-108">Type</span></span>|<span data-ttu-id="0f12b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f12b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f12b-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="0f12b-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="0f12b-111">String</span><span class="sxs-lookup"><span data-stu-id="0f12b-111">String</span></span>|<span data-ttu-id="0f12b-112">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="0f12b-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="0f12b-113">代理</span><span class="sxs-lookup"><span data-stu-id="0f12b-113">proxy</span></span>|<span data-ttu-id="0f12b-114">String</span><span class="sxs-lookup"><span data-stu-id="0f12b-114">String</span></span>|<span data-ttu-id="0f12b-115">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="0f12b-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f12b-116">关系</span><span class="sxs-lookup"><span data-stu-id="0f12b-116">Relationships</span></span>
<span data-ttu-id="0f12b-117">无</span><span class="sxs-lookup"><span data-stu-id="0f12b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f12b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f12b-118">JSON Representation</span></span>
<span data-ttu-id="0f12b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f12b-119">Here is a JSON representation of the resource.</span></span>
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



