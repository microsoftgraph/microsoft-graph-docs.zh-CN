---
title: networkInterface 资源类型
description: 表示与此主机相关联的网络接口卡（NIC）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5fd40bec964a73579863b8222cd4c90d58991502
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522573"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="40b3c-103">networkInterface 资源类型</span><span class="sxs-lookup"><span data-stu-id="40b3c-103">networkInterface resource type</span></span>

<span data-ttu-id="40b3c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="40b3c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40b3c-105">表示与此主机相关联的网络接口卡（NIC）。</span><span class="sxs-lookup"><span data-stu-id="40b3c-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="40b3c-106">属性</span><span class="sxs-lookup"><span data-stu-id="40b3c-106">Properties</span></span>

| <span data-ttu-id="40b3c-107">属性</span><span class="sxs-lookup"><span data-stu-id="40b3c-107">Property</span></span>   | <span data-ttu-id="40b3c-108">类型</span><span class="sxs-lookup"><span data-stu-id="40b3c-108">Type</span></span> |<span data-ttu-id="40b3c-109">说明</span><span class="sxs-lookup"><span data-stu-id="40b3c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b3c-110">说明</span><span class="sxs-lookup"><span data-stu-id="40b3c-110">description</span></span>|<span data-ttu-id="40b3c-111">String</span><span class="sxs-lookup"><span data-stu-id="40b3c-111">String</span></span>|<span data-ttu-id="40b3c-112">NIC 的说明（例如，以太网适配器、无线局域网适配器本地区域连接 \* < # > 等）。</span><span class="sxs-lookup"><span data-stu-id="40b3c-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="40b3c-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="40b3c-113">ipV4Address</span></span>|<span data-ttu-id="40b3c-114">String</span><span class="sxs-lookup"><span data-stu-id="40b3c-114">String</span></span>|<span data-ttu-id="40b3c-115">与此 NIC 关联的最后一个 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="40b3c-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="40b3c-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="40b3c-116">ipV6Address</span></span>|<span data-ttu-id="40b3c-117">String</span><span class="sxs-lookup"><span data-stu-id="40b3c-117">String</span></span>|<span data-ttu-id="40b3c-118">与此 NIC 关联的最后一个公共（也称为全局） IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="40b3c-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="40b3c-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="40b3c-119">localIpV6Address</span></span>|<span data-ttu-id="40b3c-120">String</span><span class="sxs-lookup"><span data-stu-id="40b3c-120">String</span></span>|<span data-ttu-id="40b3c-121">与此 NIC 关联的最后一个本地（链接本地或站点本地） IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="40b3c-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="40b3c-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="40b3c-122">macAddress</span></span>|<span data-ttu-id="40b3c-123">String</span><span class="sxs-lookup"><span data-stu-id="40b3c-123">String</span></span>|<span data-ttu-id="40b3c-124">此主机上的 NIC 的 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="40b3c-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40b3c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40b3c-125">JSON representation</span></span>

<span data-ttu-id="40b3c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40b3c-126">The following is a JSON representation of the resource.</span></span>

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
