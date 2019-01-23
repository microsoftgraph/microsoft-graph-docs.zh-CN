---
title: airPrintDestination 资源类型
description: 代表一个 AirPrint 目标。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422493"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="61f39-103">airPrintDestination 资源类型</span><span class="sxs-lookup"><span data-stu-id="61f39-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="61f39-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="61f39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61f39-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="61f39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61f39-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61f39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61f39-107">代表一个 AirPrint 目标。</span><span class="sxs-lookup"><span data-stu-id="61f39-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="61f39-108">属性</span><span class="sxs-lookup"><span data-stu-id="61f39-108">Properties</span></span>
|<span data-ttu-id="61f39-109">属性</span><span class="sxs-lookup"><span data-stu-id="61f39-109">Property</span></span>|<span data-ttu-id="61f39-110">类型</span><span class="sxs-lookup"><span data-stu-id="61f39-110">Type</span></span>|<span data-ttu-id="61f39-111">说明</span><span class="sxs-lookup"><span data-stu-id="61f39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61f39-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="61f39-112">ipAddress</span></span>|<span data-ttu-id="61f39-113">String</span><span class="sxs-lookup"><span data-stu-id="61f39-113">String</span></span>|<span data-ttu-id="61f39-114">AirPrint 目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="61f39-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="61f39-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="61f39-115">resourcePath</span></span>|<span data-ttu-id="61f39-116">String</span><span class="sxs-lookup"><span data-stu-id="61f39-116">String</span></span>|<span data-ttu-id="61f39-117">与打印机关联的资源路径。</span><span class="sxs-lookup"><span data-stu-id="61f39-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="61f39-118">这对应于 _ipps.tcp Bonjour 记录的 rp 参数。</span><span class="sxs-lookup"><span data-stu-id="61f39-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="61f39-119">例如： 打印机/Canon_MG5300_series 打印机/Xerox_Phaser_7600、 ipp/打印，Epson_IPP_Printer。</span><span class="sxs-lookup"><span data-stu-id="61f39-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="61f39-120">port</span><span class="sxs-lookup"><span data-stu-id="61f39-120">port</span></span>|<span data-ttu-id="61f39-121">Int32</span><span class="sxs-lookup"><span data-stu-id="61f39-121">Int32</span></span>|<span data-ttu-id="61f39-122">AirPrint 目标侦听端口。</span><span class="sxs-lookup"><span data-stu-id="61f39-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="61f39-123">如果未指定此项 AirPrint 将使用默认端口。</span><span class="sxs-lookup"><span data-stu-id="61f39-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="61f39-124">在 iOS 11.0 中可用和更高版本。</span><span class="sxs-lookup"><span data-stu-id="61f39-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="61f39-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="61f39-125">forceTls</span></span>|<span data-ttu-id="61f39-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="61f39-126">Boolean</span></span>|<span data-ttu-id="61f39-127">如果 true AirPrint 连接受到保护传输层安全性 (TLS)。</span><span class="sxs-lookup"><span data-stu-id="61f39-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="61f39-128">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="61f39-128">Default is false.</span></span> <span data-ttu-id="61f39-129">在 iOS 11.0 中可用和更高版本。</span><span class="sxs-lookup"><span data-stu-id="61f39-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61f39-130">关系</span><span class="sxs-lookup"><span data-stu-id="61f39-130">Relationships</span></span>
<span data-ttu-id="61f39-131">无</span><span class="sxs-lookup"><span data-stu-id="61f39-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61f39-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61f39-132">JSON Representation</span></span>
<span data-ttu-id="61f39-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61f39-133">Here is a JSON representation of the resource.</span></span>
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




