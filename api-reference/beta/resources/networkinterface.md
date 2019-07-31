---
title: networkInterface 资源类型
description: 表示与此主机相关联的网络接口卡 (NIC)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef932729149ea21580ff5a8f1cc3f52e253bfc50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009613"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="85545-103">networkInterface 资源类型</span><span class="sxs-lookup"><span data-stu-id="85545-103">networkInterface resource type</span></span>

<span data-ttu-id="85545-104">表示与此主机相关联的网络接口卡 (NIC)。</span><span class="sxs-lookup"><span data-stu-id="85545-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="85545-105">属性</span><span class="sxs-lookup"><span data-stu-id="85545-105">Properties</span></span>

| <span data-ttu-id="85545-106">属性</span><span class="sxs-lookup"><span data-stu-id="85545-106">Property</span></span>   | <span data-ttu-id="85545-107">类型</span><span class="sxs-lookup"><span data-stu-id="85545-107">Type</span></span> |<span data-ttu-id="85545-108">说明</span><span class="sxs-lookup"><span data-stu-id="85545-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85545-109">说明</span><span class="sxs-lookup"><span data-stu-id="85545-109">description</span></span>|<span data-ttu-id="85545-110">String</span><span class="sxs-lookup"><span data-stu-id="85545-110">String</span></span>|<span data-ttu-id="85545-111">NIC 的说明 (例如, 以太网适配器、无线局域网适配器本地区域连接 \* < # > 等)。</span><span class="sxs-lookup"><span data-stu-id="85545-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="85545-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="85545-112">ipV4Address</span></span>|<span data-ttu-id="85545-113">String</span><span class="sxs-lookup"><span data-stu-id="85545-113">String</span></span>|<span data-ttu-id="85545-114">与此 NIC 关联的最后一个 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="85545-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="85545-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="85545-115">ipV6Address</span></span>|<span data-ttu-id="85545-116">String</span><span class="sxs-lookup"><span data-stu-id="85545-116">String</span></span>|<span data-ttu-id="85545-117">与此 NIC 关联的最后一个公共 (也称为全局) IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="85545-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="85545-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="85545-118">localIpV6Address</span></span>|<span data-ttu-id="85545-119">String</span><span class="sxs-lookup"><span data-stu-id="85545-119">String</span></span>|<span data-ttu-id="85545-120">与此 NIC 关联的最后一个本地 (链接本地或站点本地) IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="85545-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="85545-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="85545-121">macAddress</span></span>|<span data-ttu-id="85545-122">String</span><span class="sxs-lookup"><span data-stu-id="85545-122">String</span></span>|<span data-ttu-id="85545-123">此主机上的 NIC 的 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="85545-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85545-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85545-124">JSON representation</span></span>

<span data-ttu-id="85545-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85545-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
