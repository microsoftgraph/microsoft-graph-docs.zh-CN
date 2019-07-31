---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f9f654b1a68ff393315889d7b2d9286636fcf35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005833"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="ee221-104">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee221-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee221-105">包含有关主机的状态信息 (包括设备、计算机等)。</span><span class="sxs-lookup"><span data-stu-id="ee221-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="ee221-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee221-106">Properties</span></span>

| <span data-ttu-id="ee221-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee221-107">Property</span></span>   | <span data-ttu-id="ee221-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee221-108">Type</span></span>|<span data-ttu-id="ee221-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee221-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee221-110">域名</span><span class="sxs-lookup"><span data-stu-id="ee221-110">fqdn</span></span>|<span data-ttu-id="ee221-111">String</span><span class="sxs-lookup"><span data-stu-id="ee221-111">String</span></span>|<span data-ttu-id="ee221-112">主机 FQDN (完全限定的域名) (例如, machine.company.com)。</span><span class="sxs-lookup"><span data-stu-id="ee221-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="ee221-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="ee221-113">isAzureAadJoined</span></span>|<span data-ttu-id="ee221-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee221-114">Boolean</span></span>|<span data-ttu-id="ee221-115">如此如果主机已加入域到 Azure Active Directory 域服务。</span><span class="sxs-lookup"><span data-stu-id="ee221-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="ee221-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="ee221-116">isAzureAadRegistered</span></span>|<span data-ttu-id="ee221-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee221-117">Boolean</span></span>|<span data-ttu-id="ee221-118">如果主机注册到 Azure Active Directory 设备注册 (BYOD 设备, 而不是由企业完全管理), 则该属性值为 True。</span><span class="sxs-lookup"><span data-stu-id="ee221-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="ee221-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="ee221-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="ee221-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee221-120">Boolean</span></span>|<span data-ttu-id="ee221-121">如此如果主机已加入域到本地 Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="ee221-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="ee221-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="ee221-122">netBiosName</span></span>|<span data-ttu-id="ee221-123">String</span><span class="sxs-lookup"><span data-stu-id="ee221-123">String</span></span>|<span data-ttu-id="ee221-124">本地主机名, 不包含 DNS 域名。</span><span class="sxs-lookup"><span data-stu-id="ee221-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="ee221-125">os</span><span class="sxs-lookup"><span data-stu-id="ee221-125">os</span></span>|<span data-ttu-id="ee221-126">String</span><span class="sxs-lookup"><span data-stu-id="ee221-126">String</span></span>|<span data-ttu-id="ee221-127">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="ee221-127">Host Operating System.</span></span> <span data-ttu-id="ee221-128">(例如, Windows10、MacOS、RHEL 等)。</span><span class="sxs-lookup"><span data-stu-id="ee221-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="ee221-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="ee221-129">privateIpAddress</span></span>|<span data-ttu-id="ee221-130">String</span><span class="sxs-lookup"><span data-stu-id="ee221-130">String</span></span>|<span data-ttu-id="ee221-131">在出现警报时专用 (不可路由) IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。</span><span class="sxs-lookup"><span data-stu-id="ee221-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="ee221-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="ee221-132">publicIpAddress</span></span>|<span data-ttu-id="ee221-133">String</span><span class="sxs-lookup"><span data-stu-id="ee221-133">String</span></span>|<span data-ttu-id="ee221-134">在警报时可公开路由的 IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。</span><span class="sxs-lookup"><span data-stu-id="ee221-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="ee221-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="ee221-135">riskScore</span></span>|<span data-ttu-id="ee221-136">String</span><span class="sxs-lookup"><span data-stu-id="ee221-136">String</span></span>|<span data-ttu-id="ee221-137">主机的提供程序生成/计算的风险分数。</span><span class="sxs-lookup"><span data-stu-id="ee221-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="ee221-138">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="ee221-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee221-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee221-139">JSON representation</span></span>

<span data-ttu-id="ee221-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee221-140">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
