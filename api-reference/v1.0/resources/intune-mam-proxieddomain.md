---
title: proxiedDomain 资源类型
description: 代理域
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 16995c4ffc959c5a63d322da84bdca136a2422f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048405"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="1ece1-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ece1-103">proxiedDomain resource type</span></span>

<span data-ttu-id="1ece1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ece1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ece1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ece1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ece1-106">代理域</span><span class="sxs-lookup"><span data-stu-id="1ece1-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="1ece1-107">属性</span><span class="sxs-lookup"><span data-stu-id="1ece1-107">Properties</span></span>
|<span data-ttu-id="1ece1-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ece1-108">Property</span></span>|<span data-ttu-id="1ece1-109">类型</span><span class="sxs-lookup"><span data-stu-id="1ece1-109">Type</span></span>|<span data-ttu-id="1ece1-110">说明</span><span class="sxs-lookup"><span data-stu-id="1ece1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ece1-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="1ece1-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="1ece1-112">String</span><span class="sxs-lookup"><span data-stu-id="1ece1-112">String</span></span>|<span data-ttu-id="1ece1-113">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="1ece1-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="1ece1-114">代理</span><span class="sxs-lookup"><span data-stu-id="1ece1-114">proxy</span></span>|<span data-ttu-id="1ece1-115">String</span><span class="sxs-lookup"><span data-stu-id="1ece1-115">String</span></span>|<span data-ttu-id="1ece1-116">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="1ece1-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ece1-117">关系</span><span class="sxs-lookup"><span data-stu-id="1ece1-117">Relationships</span></span>
<span data-ttu-id="1ece1-118">无</span><span class="sxs-lookup"><span data-stu-id="1ece1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ece1-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ece1-119">JSON Representation</span></span>
<span data-ttu-id="1ece1-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ece1-120">Here is a JSON representation of the resource.</span></span>
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









