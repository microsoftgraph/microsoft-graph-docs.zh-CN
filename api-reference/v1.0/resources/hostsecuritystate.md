---
title: hostSecurityState 资源类型
description: 包含有关主机的状态信息 (包括设备、计算机等)。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dabe7d0aa026cb1b514e95fbc953dcb1974f8925
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029272"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="0f950-103">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f950-103">hostSecurityState resource type</span></span>

<span data-ttu-id="0f950-104">包含有关主机的状态信息 (包括设备、计算机等)。</span><span class="sxs-lookup"><span data-stu-id="0f950-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="0f950-105">属性</span><span class="sxs-lookup"><span data-stu-id="0f950-105">Properties</span></span>

| <span data-ttu-id="0f950-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f950-106">Property</span></span>   | <span data-ttu-id="0f950-107">类型</span><span class="sxs-lookup"><span data-stu-id="0f950-107">Type</span></span>|<span data-ttu-id="0f950-108">说明</span><span class="sxs-lookup"><span data-stu-id="0f950-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f950-109">域名</span><span class="sxs-lookup"><span data-stu-id="0f950-109">fqdn</span></span>|<span data-ttu-id="0f950-110">String</span><span class="sxs-lookup"><span data-stu-id="0f950-110">String</span></span>|<span data-ttu-id="0f950-111">主机 FQDN (完全限定的`machine.company.com`域名) (例如)。</span><span class="sxs-lookup"><span data-stu-id="0f950-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="0f950-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="0f950-112">isAzureAadJoined</span></span>|<span data-ttu-id="0f950-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f950-113">Boolean</span></span>|<span data-ttu-id="0f950-114">如此如果主机已加入域到 Azure Active Directory 域服务。</span><span class="sxs-lookup"><span data-stu-id="0f950-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="0f950-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="0f950-115">isAzureAadRegistered</span></span>|<span data-ttu-id="0f950-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f950-116">Boolean</span></span>|<span data-ttu-id="0f950-117">如果主机注册到 Azure Active Directory 设备注册 (BYOD 设备, 而不是由企业完全管理), 则该属性值为 True。</span><span class="sxs-lookup"><span data-stu-id="0f950-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="0f950-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="0f950-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="0f950-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f950-119">Boolean</span></span>|<span data-ttu-id="0f950-120">如此如果主机已加入域到本地 Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="0f950-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="0f950-121">netBiosName</span><span class="sxs-lookup"><span data-stu-id="0f950-121">netBiosName</span></span>|<span data-ttu-id="0f950-122">String</span><span class="sxs-lookup"><span data-stu-id="0f950-122">String</span></span>|<span data-ttu-id="0f950-123">本地主机名, 不包含 DNS 域名。</span><span class="sxs-lookup"><span data-stu-id="0f950-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="0f950-124">os</span><span class="sxs-lookup"><span data-stu-id="0f950-124">os</span></span>|<span data-ttu-id="0f950-125">String</span><span class="sxs-lookup"><span data-stu-id="0f950-125">String</span></span>|<span data-ttu-id="0f950-126">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="0f950-126">Host Operating System.</span></span> <span data-ttu-id="0f950-127">(例如, Windows10、MacOS、RHEL 等)。</span><span class="sxs-lookup"><span data-stu-id="0f950-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="0f950-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="0f950-128">privateIpAddress</span></span>|<span data-ttu-id="0f950-129">String</span><span class="sxs-lookup"><span data-stu-id="0f950-129">String</span></span>|<span data-ttu-id="0f950-130">在出现警报时专用 (不可路由) IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。</span><span class="sxs-lookup"><span data-stu-id="0f950-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="0f950-131">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="0f950-131">publicIpAddress</span></span>|<span data-ttu-id="0f950-132">String</span><span class="sxs-lookup"><span data-stu-id="0f950-132">String</span></span>|<span data-ttu-id="0f950-133">在警报时可公开路由的 IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。</span><span class="sxs-lookup"><span data-stu-id="0f950-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="0f950-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="0f950-134">riskScore</span></span>|<span data-ttu-id="0f950-135">String</span><span class="sxs-lookup"><span data-stu-id="0f950-135">String</span></span>|<span data-ttu-id="0f950-136">主机的提供程序生成/计算的风险分数。</span><span class="sxs-lookup"><span data-stu-id="0f950-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="0f950-137">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="0f950-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f950-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f950-138">JSON representation</span></span>

<span data-ttu-id="0f950-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f950-139">The following is a JSON representation of the resource.</span></span>

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
