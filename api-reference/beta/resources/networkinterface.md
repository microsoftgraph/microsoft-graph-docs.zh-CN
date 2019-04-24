---
title: networkInterface 资源类型
description: 表示与此主机相关联的网络接口卡 (NIC)。
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457065"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="3502d-103">networkInterface 资源类型</span><span class="sxs-lookup"><span data-stu-id="3502d-103">networkInterface resource type</span></span>

<span data-ttu-id="3502d-104">表示与此主机相关联的网络接口卡 (NIC)。</span><span class="sxs-lookup"><span data-stu-id="3502d-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="3502d-105">属性</span><span class="sxs-lookup"><span data-stu-id="3502d-105">Properties</span></span>

| <span data-ttu-id="3502d-106">属性</span><span class="sxs-lookup"><span data-stu-id="3502d-106">Property</span></span>   | <span data-ttu-id="3502d-107">类型</span><span class="sxs-lookup"><span data-stu-id="3502d-107">Type</span></span> |<span data-ttu-id="3502d-108">描述</span><span class="sxs-lookup"><span data-stu-id="3502d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3502d-109">说明</span><span class="sxs-lookup"><span data-stu-id="3502d-109">description</span></span>|<span data-ttu-id="3502d-110">字符串</span><span class="sxs-lookup"><span data-stu-id="3502d-110">String</span></span>|<span data-ttu-id="3502d-111">NIC 的说明 (例如, 以太网适配器、无线局域网适配器本地区域连接 \* < # > 等)。</span><span class="sxs-lookup"><span data-stu-id="3502d-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="3502d-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="3502d-112">ipV4Address</span></span>|<span data-ttu-id="3502d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3502d-113">String</span></span>|<span data-ttu-id="3502d-114">与此 NIC 关联的最后一个 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="3502d-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="3502d-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="3502d-115">ipV6Address</span></span>|<span data-ttu-id="3502d-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3502d-116">String</span></span>|<span data-ttu-id="3502d-117">与此 NIC 关联的最后一个公共 (也称为全局) IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="3502d-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="3502d-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="3502d-118">localIpV6Address</span></span>|<span data-ttu-id="3502d-119">字符串</span><span class="sxs-lookup"><span data-stu-id="3502d-119">String</span></span>|<span data-ttu-id="3502d-120">与此 NIC 关联的最后一个本地 (链接本地或站点本地) IPv6 地址。</span><span class="sxs-lookup"><span data-stu-id="3502d-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="3502d-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="3502d-121">macAddress</span></span>|<span data-ttu-id="3502d-122">字符串</span><span class="sxs-lookup"><span data-stu-id="3502d-122">String</span></span>|<span data-ttu-id="3502d-123">此主机上的 NIC 的 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="3502d-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3502d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3502d-124">JSON representation</span></span>

<span data-ttu-id="3502d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3502d-125">The following is a JSON representation of the resource.</span></span>

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
