---
title: networkInterface 资源类型
description: 表示与此主机网络接口卡 (NIC)。
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823301"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="75061-103">networkInterface 资源类型</span><span class="sxs-lookup"><span data-stu-id="75061-103">networkInterface resource type</span></span>

<span data-ttu-id="75061-104">表示与此主机网络接口卡 (NIC)。</span><span class="sxs-lookup"><span data-stu-id="75061-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="75061-105">属性</span><span class="sxs-lookup"><span data-stu-id="75061-105">Properties</span></span>

| <span data-ttu-id="75061-106">属性</span><span class="sxs-lookup"><span data-stu-id="75061-106">Property</span></span>   | <span data-ttu-id="75061-107">类型</span><span class="sxs-lookup"><span data-stu-id="75061-107">Type</span></span> |<span data-ttu-id="75061-108">说明</span><span class="sxs-lookup"><span data-stu-id="75061-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75061-109">说明</span><span class="sxs-lookup"><span data-stu-id="75061-109">description</span></span>|<span data-ttu-id="75061-110">字符串</span><span class="sxs-lookup"><span data-stu-id="75061-110">String</span></span>|<span data-ttu-id="75061-111">NIC 的说明 (例如以太网适配器，无线 LAN 适配器本地区域连接 \* <> # 等。)。</span><span class="sxs-lookup"><span data-stu-id="75061-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="75061-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="75061-112">ipV4Address</span></span>|<span data-ttu-id="75061-113">字符串</span><span class="sxs-lookup"><span data-stu-id="75061-113">String</span></span>|<span data-ttu-id="75061-114">与此网卡关联的最后一个 IPv4 地址</span><span class="sxs-lookup"><span data-stu-id="75061-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="75061-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="75061-115">ipV6Address</span></span>|<span data-ttu-id="75061-116">字符串</span><span class="sxs-lookup"><span data-stu-id="75061-116">String</span></span>|<span data-ttu-id="75061-117">最后一个公用 （也称为全局） IPv6 地址与此网卡。</span><span class="sxs-lookup"><span data-stu-id="75061-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="75061-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="75061-118">localIpV6Address</span></span>|<span data-ttu-id="75061-119">字符串</span><span class="sxs-lookup"><span data-stu-id="75061-119">String</span></span>|<span data-ttu-id="75061-120">最后一个本地 （链接-本地或站点-本地） IPv6 地址与此网卡。</span><span class="sxs-lookup"><span data-stu-id="75061-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="75061-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="75061-121">macAddress</span></span>|<span data-ttu-id="75061-122">字符串</span><span class="sxs-lookup"><span data-stu-id="75061-122">String</span></span>|<span data-ttu-id="75061-123">此主机上的 NIC 的 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="75061-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75061-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75061-124">JSON representation</span></span>

<span data-ttu-id="75061-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75061-125">The following is a JSON representation of the resource.</span></span>

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
