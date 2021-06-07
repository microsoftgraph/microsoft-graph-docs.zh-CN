---
title: proxiedDomain 资源类型
description: 代理域
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25914b3cba48120e91352028bb51bcdee8edee2b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752320"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="5a15d-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a15d-103">proxiedDomain resource type</span></span>

<span data-ttu-id="5a15d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a15d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a15d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a15d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a15d-106">代理域</span><span class="sxs-lookup"><span data-stu-id="5a15d-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="5a15d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5a15d-107">Properties</span></span>
|<span data-ttu-id="5a15d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a15d-108">Property</span></span>|<span data-ttu-id="5a15d-109">类型</span><span class="sxs-lookup"><span data-stu-id="5a15d-109">Type</span></span>|<span data-ttu-id="5a15d-110">Description</span><span class="sxs-lookup"><span data-stu-id="5a15d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a15d-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="5a15d-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="5a15d-112">String</span><span class="sxs-lookup"><span data-stu-id="5a15d-112">String</span></span>|<span data-ttu-id="5a15d-113">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="5a15d-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="5a15d-114">代理</span><span class="sxs-lookup"><span data-stu-id="5a15d-114">proxy</span></span>|<span data-ttu-id="5a15d-115">String</span><span class="sxs-lookup"><span data-stu-id="5a15d-115">String</span></span>|<span data-ttu-id="5a15d-116">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="5a15d-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a15d-117">关系</span><span class="sxs-lookup"><span data-stu-id="5a15d-117">Relationships</span></span>
<span data-ttu-id="5a15d-118">无</span><span class="sxs-lookup"><span data-stu-id="5a15d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a15d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a15d-119">JSON Representation</span></span>
<span data-ttu-id="5a15d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a15d-120">Here is a JSON representation of the resource.</span></span>
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




