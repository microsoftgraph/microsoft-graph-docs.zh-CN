---
title: airPrintDestination 资源类型
description: 表示 AirPrint 目标。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99693cbdfa77895e0116ac5228fdf58d95afeacb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487359"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="3b1b3-103">airPrintDestination 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b1b3-103">airPrintDestination resource type</span></span>

<span data-ttu-id="3b1b3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3b1b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b1b3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b1b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b1b3-107">表示 AirPrint 目标。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="3b1b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b1b3-108">Properties</span></span>
|<span data-ttu-id="3b1b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b1b3-109">Property</span></span>|<span data-ttu-id="3b1b3-110">类型</span><span class="sxs-lookup"><span data-stu-id="3b1b3-110">Type</span></span>|<span data-ttu-id="3b1b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b1b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b1b3-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3b1b3-112">ipAddress</span></span>|<span data-ttu-id="3b1b3-113">String</span><span class="sxs-lookup"><span data-stu-id="3b1b3-113">String</span></span>|<span data-ttu-id="3b1b3-114">AirPrint 目标的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="3b1b3-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="3b1b3-115">resourcePath</span></span>|<span data-ttu-id="3b1b3-116">String</span><span class="sxs-lookup"><span data-stu-id="3b1b3-116">String</span></span>|<span data-ttu-id="3b1b3-117">与打印机关联的资源路径。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="3b1b3-118">这对应于 _ipps tcp Bonjour record 的 rp 参数。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="3b1b3-119">例如： printers/Canon_MG5300_series、printers/Xerox_Phaser_7600、ipp/print、Epson_IPP_Printer。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="3b1b3-120">端口</span><span class="sxs-lookup"><span data-stu-id="3b1b3-120">port</span></span>|<span data-ttu-id="3b1b3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3b1b3-121">Int32</span></span>|<span data-ttu-id="3b1b3-122">AirPrint 目标的侦听端口。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="3b1b3-123">如果未指定此项，AirPrint 将使用默认端口。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="3b1b3-124">在 iOS 11.0 和更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="3b1b3-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="3b1b3-125">forceTls</span></span>|<span data-ttu-id="3b1b3-126">布尔</span><span class="sxs-lookup"><span data-stu-id="3b1b3-126">Boolean</span></span>|<span data-ttu-id="3b1b3-127">如果为 true，则 AirPrint 连接通过传输层安全性（TLS）进行保护。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="3b1b3-128">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-128">Default is false.</span></span> <span data-ttu-id="3b1b3-129">在 iOS 11.0 和更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b1b3-130">关系</span><span class="sxs-lookup"><span data-stu-id="3b1b3-130">Relationships</span></span>
<span data-ttu-id="3b1b3-131">无</span><span class="sxs-lookup"><span data-stu-id="3b1b3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b1b3-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b1b3-132">JSON Representation</span></span>
<span data-ttu-id="3b1b3-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b1b3-133">Here is a JSON representation of the resource.</span></span>
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



