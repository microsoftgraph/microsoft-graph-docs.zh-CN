---
title: networkInterface 资源类型
description: 表示与此主机关联 (NIC) 的网络接口卡。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d7b712c50d8cc19951f583cb8c9af7e185dba7ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029160"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="d9951-103">networkInterface 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9951-103">networkInterface resource type</span></span>

<span data-ttu-id="d9951-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9951-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9951-105">表示与此主机关联 (NIC) 的网络接口卡。</span><span class="sxs-lookup"><span data-stu-id="d9951-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="d9951-106">属性</span><span class="sxs-lookup"><span data-stu-id="d9951-106">Properties</span></span>

| <span data-ttu-id="d9951-107">属性</span><span class="sxs-lookup"><span data-stu-id="d9951-107">Property</span></span>   | <span data-ttu-id="d9951-108">类型</span><span class="sxs-lookup"><span data-stu-id="d9951-108">Type</span></span> |<span data-ttu-id="d9951-109">说明</span><span class="sxs-lookup"><span data-stu-id="d9951-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9951-110">说明</span><span class="sxs-lookup"><span data-stu-id="d9951-110">description</span></span>|<span data-ttu-id="d9951-111">String</span><span class="sxs-lookup"><span data-stu-id="d9951-111">String</span></span>|<span data-ttu-id="d9951-112">NIC 的说明 (例如，以太网适配器、无线局域网适配器本地区域连接 \* < # > 等 ) 。</span><span class="sxs-lookup"><span data-stu-id="d9951-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="d9951-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="d9951-113">ipV4Address</span></span>|<span data-ttu-id="d9951-114">String</span><span class="sxs-lookup"><span data-stu-id="d9951-114">String</span></span>|<span data-ttu-id="d9951-115">与此 NIC 关联的最后一个 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="d9951-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="d9951-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="d9951-116">ipV6Address</span></span>|<span data-ttu-id="d9951-117">String</span><span class="sxs-lookup"><span data-stu-id="d9951-117">String</span></span>|<span data-ttu-id="d9951-118">最后一个公共 (也称为全局) 与此 NIC 关联的 IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="d9951-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="d9951-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="d9951-119">localIpV6Address</span></span>|<span data-ttu-id="d9951-120">String</span><span class="sxs-lookup"><span data-stu-id="d9951-120">String</span></span>|<span data-ttu-id="d9951-121">上次本地 (与此 NIC 关联的本地或站点本地) IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="d9951-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="d9951-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="d9951-122">macAddress</span></span>|<span data-ttu-id="d9951-123">String</span><span class="sxs-lookup"><span data-stu-id="d9951-123">String</span></span>|<span data-ttu-id="d9951-124">此主机上的 NIC 的 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="d9951-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9951-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9951-125">JSON representation</span></span>

<span data-ttu-id="d9951-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9951-126">The following is a JSON representation of the resource.</span></span>

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


