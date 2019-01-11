---
title: airPrintDestination 资源类型
description: 代表一个 AirPrint 目标。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6d1548737956d35d42fc077afe92de1885a54581
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878587"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="3a8d9-103">airPrintDestination 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a8d9-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="3a8d9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a8d9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a8d9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a8d9-107">代表一个 AirPrint 目标。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="3a8d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a8d9-108">Properties</span></span>
|<span data-ttu-id="3a8d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="3a8d9-109">Property</span></span>|<span data-ttu-id="3a8d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="3a8d9-110">Type</span></span>|<span data-ttu-id="3a8d9-111">Description</span><span class="sxs-lookup"><span data-stu-id="3a8d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a8d9-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3a8d9-112">ipAddress</span></span>|<span data-ttu-id="3a8d9-113">String</span><span class="sxs-lookup"><span data-stu-id="3a8d9-113">String</span></span>|<span data-ttu-id="3a8d9-114">AirPrint 目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="3a8d9-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="3a8d9-115">resourcePath</span></span>|<span data-ttu-id="3a8d9-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3a8d9-116">String</span></span>|<span data-ttu-id="3a8d9-117">与打印机关联的资源路径。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="3a8d9-118">这对应于 _ipps.tcp Bonjour 记录的 rp 参数。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="3a8d9-119">例如： 打印机/Canon_MG5300_series 打印机/Xerox_Phaser_7600、 ipp/打印，Epson_IPP_Printer。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="3a8d9-120">port</span><span class="sxs-lookup"><span data-stu-id="3a8d9-120">port</span></span>|<span data-ttu-id="3a8d9-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3a8d9-121">Int32</span></span>|<span data-ttu-id="3a8d9-122">AirPrint 目标侦听端口。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="3a8d9-123">如果未指定此项 AirPrint 将使用默认端口。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="3a8d9-124">在 iOS 11.0 中可用和更高版本。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="3a8d9-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="3a8d9-125">forceTls</span></span>|<span data-ttu-id="3a8d9-126">布尔</span><span class="sxs-lookup"><span data-stu-id="3a8d9-126">Boolean</span></span>|<span data-ttu-id="3a8d9-127">如果 true AirPrint 连接受到保护传输层安全性 (TLS)。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="3a8d9-128">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-128">Default is false.</span></span> <span data-ttu-id="3a8d9-129">在 iOS 11.0 中可用和更高版本。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a8d9-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="3a8d9-130">Relationships</span></span>
<span data-ttu-id="3a8d9-131">无</span><span class="sxs-lookup"><span data-stu-id="3a8d9-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a8d9-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a8d9-132">JSON Representation</span></span>
<span data-ttu-id="3a8d9-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a8d9-133">Here is a JSON representation of the resource.</span></span>
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





