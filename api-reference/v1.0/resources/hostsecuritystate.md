---
title: hostSecurityState 资源类型
description: 包含状态信息 （包括设备、 计算机等） 的主机。
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816336"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="b1d0d-103">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1d0d-103">hostSecurityState resource type</span></span>

<span data-ttu-id="b1d0d-104">包含状态信息 （包括设备、 计算机等） 的主机。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="b1d0d-105">属性</span><span class="sxs-lookup"><span data-stu-id="b1d0d-105">Properties</span></span>

| <span data-ttu-id="b1d0d-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1d0d-106">Property</span></span>   | <span data-ttu-id="b1d0d-107">类型</span><span class="sxs-lookup"><span data-stu-id="b1d0d-107">Type</span></span>|<span data-ttu-id="b1d0d-108">Description</span><span class="sxs-lookup"><span data-stu-id="b1d0d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1d0d-109">fqdn</span><span class="sxs-lookup"><span data-stu-id="b1d0d-109">fqdn</span></span>|<span data-ttu-id="b1d0d-110">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d0d-110">String</span></span>|<span data-ttu-id="b1d0d-111">承载 FQDN （完全限定域名） (例如， `machine.company.com`)。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="b1d0d-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="b1d0d-112">isAzureAadJoined</span></span>|<span data-ttu-id="b1d0d-113">布尔</span><span class="sxs-lookup"><span data-stu-id="b1d0d-113">Boolean</span></span>|<span data-ttu-id="b1d0d-114">如果主机是加入到 Azure Active Directory 域服务的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="b1d0d-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="b1d0d-115">isAzureAadRegistered</span></span>|<span data-ttu-id="b1d0d-116">布尔</span><span class="sxs-lookup"><span data-stu-id="b1d0d-116">Boolean</span></span>|<span data-ttu-id="b1d0d-117">如果主机注册 Azure Active Directory 设备注册 （BYOD 设备-，即不完全由企业管理），则为 true。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="b1d0d-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="b1d0d-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="b1d0d-119">布尔</span><span class="sxs-lookup"><span data-stu-id="b1d0d-119">Boolean</span></span>|<span data-ttu-id="b1d0d-120">如果主机是加入本地 Active Directory 域的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="b1d0d-121">netBiosName</span><span class="sxs-lookup"><span data-stu-id="b1d0d-121">netBiosName</span></span>|<span data-ttu-id="b1d0d-122">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d0d-122">String</span></span>|<span data-ttu-id="b1d0d-123">不带的 DNS 域名的本地主机名称。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="b1d0d-124">操作系统</span><span class="sxs-lookup"><span data-stu-id="b1d0d-124">os</span></span>|<span data-ttu-id="b1d0d-125">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d0d-125">String</span></span>|<span data-ttu-id="b1d0d-126">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-126">Host Operating System.</span></span> <span data-ttu-id="b1d0d-127">（例如，Windows10 MacOS、 RHEL，等）。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="b1d0d-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="b1d0d-128">privateIpAddress</span></span>|<span data-ttu-id="b1d0d-129">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d0d-129">String</span></span>|<span data-ttu-id="b1d0d-130">专用 （不可穿） 的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="b1d0d-131">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="b1d0d-131">publicIpAddress</span></span>|<span data-ttu-id="b1d0d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d0d-132">String</span></span>|<span data-ttu-id="b1d0d-133">公共可路由的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="b1d0d-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="b1d0d-134">riskScore</span></span>|<span data-ttu-id="b1d0d-135">字符串</span><span class="sxs-lookup"><span data-stu-id="b1d0d-135">String</span></span>|<span data-ttu-id="b1d0d-136">带有提供程序生成/计算风险的主机的分数。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="b1d0d-137">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1d0d-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1d0d-138">JSON representation</span></span>

<span data-ttu-id="b1d0d-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1d0d-139">The following is a JSON representation of the resource.</span></span>

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
