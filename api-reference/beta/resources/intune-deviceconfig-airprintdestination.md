---
title: airPrintDestination 资源类型
description: 表示 AirPrint 目标。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e457cf44b5a73f14dfd87fd69f2b9e27cef08c3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731937"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="b66f0-103">airPrintDestination 资源类型</span><span class="sxs-lookup"><span data-stu-id="b66f0-103">airPrintDestination resource type</span></span>

<span data-ttu-id="b66f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b66f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b66f0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b66f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b66f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b66f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b66f0-107">表示 AirPrint 目标。</span><span class="sxs-lookup"><span data-stu-id="b66f0-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="b66f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b66f0-108">Properties</span></span>
|<span data-ttu-id="b66f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="b66f0-109">Property</span></span>|<span data-ttu-id="b66f0-110">类型</span><span class="sxs-lookup"><span data-stu-id="b66f0-110">Type</span></span>|<span data-ttu-id="b66f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b66f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b66f0-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b66f0-112">ipAddress</span></span>|<span data-ttu-id="b66f0-113">String</span><span class="sxs-lookup"><span data-stu-id="b66f0-113">String</span></span>|<span data-ttu-id="b66f0-114">AirPrint 目标的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b66f0-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="b66f0-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="b66f0-115">resourcePath</span></span>|<span data-ttu-id="b66f0-116">String</span><span class="sxs-lookup"><span data-stu-id="b66f0-116">String</span></span>|<span data-ttu-id="b66f0-117">与打印机关联的资源路径。</span><span class="sxs-lookup"><span data-stu-id="b66f0-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="b66f0-118">这对应于 _ipps tcp Bonjour record 的 rp 参数。</span><span class="sxs-lookup"><span data-stu-id="b66f0-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="b66f0-119">例如： printers/Canon_MG5300_series、printers/Xerox_Phaser_7600、ipp/print、Epson_IPP_Printer。</span><span class="sxs-lookup"><span data-stu-id="b66f0-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="b66f0-120">端口</span><span class="sxs-lookup"><span data-stu-id="b66f0-120">port</span></span>|<span data-ttu-id="b66f0-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b66f0-121">Int32</span></span>|<span data-ttu-id="b66f0-122">AirPrint 目标的侦听端口。</span><span class="sxs-lookup"><span data-stu-id="b66f0-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="b66f0-123">如果未指定此项，AirPrint 将使用默认端口。</span><span class="sxs-lookup"><span data-stu-id="b66f0-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="b66f0-124">在 iOS 11.0 和更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="b66f0-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="b66f0-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="b66f0-125">forceTls</span></span>|<span data-ttu-id="b66f0-126">布尔</span><span class="sxs-lookup"><span data-stu-id="b66f0-126">Boolean</span></span>|<span data-ttu-id="b66f0-127">如果为 true，则 AirPrint 连接受传输层安全性 (TLS) 的保护。</span><span class="sxs-lookup"><span data-stu-id="b66f0-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="b66f0-128">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="b66f0-128">Default is false.</span></span> <span data-ttu-id="b66f0-129">在 iOS 11.0 和更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="b66f0-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b66f0-130">关系</span><span class="sxs-lookup"><span data-stu-id="b66f0-130">Relationships</span></span>
<span data-ttu-id="b66f0-131">无</span><span class="sxs-lookup"><span data-stu-id="b66f0-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b66f0-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b66f0-132">JSON Representation</span></span>
<span data-ttu-id="b66f0-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b66f0-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```





