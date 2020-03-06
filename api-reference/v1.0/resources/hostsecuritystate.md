---
title: hostSecurityState 资源类型
description: 包含有关主机的状态信息（包括设备、计算机等）。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8993e9ac301bc1cc0ae4da4ec66cc131a3e06c18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531348"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="95753-103">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="95753-103">hostSecurityState resource type</span></span>

<span data-ttu-id="95753-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95753-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95753-105">包含有关主机的状态信息（包括设备、计算机等）。</span><span class="sxs-lookup"><span data-stu-id="95753-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="95753-106">属性</span><span class="sxs-lookup"><span data-stu-id="95753-106">Properties</span></span>

| <span data-ttu-id="95753-107">属性</span><span class="sxs-lookup"><span data-stu-id="95753-107">Property</span></span>   | <span data-ttu-id="95753-108">类型</span><span class="sxs-lookup"><span data-stu-id="95753-108">Type</span></span>|<span data-ttu-id="95753-109">说明</span><span class="sxs-lookup"><span data-stu-id="95753-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95753-110">域名</span><span class="sxs-lookup"><span data-stu-id="95753-110">fqdn</span></span>|<span data-ttu-id="95753-111">字符串</span><span class="sxs-lookup"><span data-stu-id="95753-111">String</span></span>|<span data-ttu-id="95753-112">主机 FQDN （完全限定的`machine.company.com`域名）（例如）。</span><span class="sxs-lookup"><span data-stu-id="95753-112">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="95753-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="95753-113">isAzureAadJoined</span></span>|<span data-ttu-id="95753-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="95753-114">Boolean</span></span>|<span data-ttu-id="95753-115">如此如果主机已加入域到 Azure Active Directory 域服务。</span><span class="sxs-lookup"><span data-stu-id="95753-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="95753-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="95753-116">isAzureAadRegistered</span></span>|<span data-ttu-id="95753-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="95753-117">Boolean</span></span>|<span data-ttu-id="95753-118">如果主机注册到 Azure Active Directory 设备注册（BYOD 设备，而不是由企业完全管理），则该属性值为 True。</span><span class="sxs-lookup"><span data-stu-id="95753-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="95753-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="95753-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="95753-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="95753-120">Boolean</span></span>|<span data-ttu-id="95753-121">如此如果主机已加入域到本地 Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="95753-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="95753-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="95753-122">netBiosName</span></span>|<span data-ttu-id="95753-123">字符串</span><span class="sxs-lookup"><span data-stu-id="95753-123">String</span></span>|<span data-ttu-id="95753-124">本地主机名，不包含 DNS 域名。</span><span class="sxs-lookup"><span data-stu-id="95753-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="95753-125">os</span><span class="sxs-lookup"><span data-stu-id="95753-125">os</span></span>|<span data-ttu-id="95753-126">字符串</span><span class="sxs-lookup"><span data-stu-id="95753-126">String</span></span>|<span data-ttu-id="95753-127">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="95753-127">Host Operating System.</span></span> <span data-ttu-id="95753-128">（例如，Windows10、MacOS、RHEL 等）。</span><span class="sxs-lookup"><span data-stu-id="95753-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="95753-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="95753-129">privateIpAddress</span></span>|<span data-ttu-id="95753-130">字符串</span><span class="sxs-lookup"><span data-stu-id="95753-130">String</span></span>|<span data-ttu-id="95753-131">在出现警报时专用（不可路由） IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。</span><span class="sxs-lookup"><span data-stu-id="95753-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="95753-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="95753-132">publicIpAddress</span></span>|<span data-ttu-id="95753-133">字符串</span><span class="sxs-lookup"><span data-stu-id="95753-133">String</span></span>|<span data-ttu-id="95753-134">在警报时可公开路由的 IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。</span><span class="sxs-lookup"><span data-stu-id="95753-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="95753-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="95753-135">riskScore</span></span>|<span data-ttu-id="95753-136">字符串</span><span class="sxs-lookup"><span data-stu-id="95753-136">String</span></span>|<span data-ttu-id="95753-137">主机的提供程序生成/计算的风险分数。</span><span class="sxs-lookup"><span data-stu-id="95753-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="95753-138">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="95753-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95753-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95753-139">JSON representation</span></span>

<span data-ttu-id="95753-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95753-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
