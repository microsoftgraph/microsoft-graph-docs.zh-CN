---
title: airPrintDestination 资源类型
description: 表示 AirPrint 目标。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25d782501033a81ea6324028fadfe75a701b0a07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971570"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="7307b-103">airPrintDestination 资源类型</span><span class="sxs-lookup"><span data-stu-id="7307b-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="7307b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7307b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7307b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7307b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7307b-106">表示 AirPrint 目标。</span><span class="sxs-lookup"><span data-stu-id="7307b-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="7307b-107">属性</span><span class="sxs-lookup"><span data-stu-id="7307b-107">Properties</span></span>
|<span data-ttu-id="7307b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7307b-108">Property</span></span>|<span data-ttu-id="7307b-109">类型</span><span class="sxs-lookup"><span data-stu-id="7307b-109">Type</span></span>|<span data-ttu-id="7307b-110">说明</span><span class="sxs-lookup"><span data-stu-id="7307b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7307b-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="7307b-111">ipAddress</span></span>|<span data-ttu-id="7307b-112">String</span><span class="sxs-lookup"><span data-stu-id="7307b-112">String</span></span>|<span data-ttu-id="7307b-113">AirPrint 目标的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="7307b-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="7307b-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="7307b-114">resourcePath</span></span>|<span data-ttu-id="7307b-115">String</span><span class="sxs-lookup"><span data-stu-id="7307b-115">String</span></span>|<span data-ttu-id="7307b-116">与打印机关联的资源路径。</span><span class="sxs-lookup"><span data-stu-id="7307b-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="7307b-117">这对应于 _ipps Bonjour 记录的 rp 参数。</span><span class="sxs-lookup"><span data-stu-id="7307b-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="7307b-118">例如: printers/Canon_MG5300_series、printers/Xerox_Phaser_7600、ipp/print、Epson_IPP_Printer。</span><span class="sxs-lookup"><span data-stu-id="7307b-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="7307b-119">端口</span><span class="sxs-lookup"><span data-stu-id="7307b-119">port</span></span>|<span data-ttu-id="7307b-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7307b-120">Int32</span></span>|<span data-ttu-id="7307b-121">AirPrint 目标的侦听端口。</span><span class="sxs-lookup"><span data-stu-id="7307b-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="7307b-122">如果未指定此项, AirPrint 将使用默认端口。</span><span class="sxs-lookup"><span data-stu-id="7307b-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="7307b-123">在 iOS 11.0 和更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="7307b-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="7307b-124">forceTls</span><span class="sxs-lookup"><span data-stu-id="7307b-124">forceTls</span></span>|<span data-ttu-id="7307b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7307b-125">Boolean</span></span>|<span data-ttu-id="7307b-126">如果为 true, 则 AirPrint 连接通过传输层安全性 (TLS) 进行保护。</span><span class="sxs-lookup"><span data-stu-id="7307b-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="7307b-127">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="7307b-127">Default is false.</span></span> <span data-ttu-id="7307b-128">在 iOS 11.0 和更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="7307b-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7307b-129">关系</span><span class="sxs-lookup"><span data-stu-id="7307b-129">Relationships</span></span>
<span data-ttu-id="7307b-130">无</span><span class="sxs-lookup"><span data-stu-id="7307b-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7307b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7307b-131">JSON Representation</span></span>
<span data-ttu-id="7307b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7307b-132">Here is a JSON representation of the resource.</span></span>
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





