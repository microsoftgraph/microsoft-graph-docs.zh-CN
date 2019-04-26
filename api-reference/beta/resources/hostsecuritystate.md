---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 670a052fa3d63da0b78ba620dbc6530a8ab122dc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340272"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="4350c-104">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="4350c-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4350c-105">包含有关主机的状态信息 (包括设备、计算机等)。</span><span class="sxs-lookup"><span data-stu-id="4350c-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="4350c-106">属性</span><span class="sxs-lookup"><span data-stu-id="4350c-106">Properties</span></span>

| <span data-ttu-id="4350c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4350c-107">Property</span></span>   | <span data-ttu-id="4350c-108">类型</span><span class="sxs-lookup"><span data-stu-id="4350c-108">Type</span></span>|<span data-ttu-id="4350c-109">说明</span><span class="sxs-lookup"><span data-stu-id="4350c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4350c-110">域名</span><span class="sxs-lookup"><span data-stu-id="4350c-110">fqdn</span></span>|<span data-ttu-id="4350c-111">String</span><span class="sxs-lookup"><span data-stu-id="4350c-111">String</span></span>|<span data-ttu-id="4350c-112">主机 FQDN (完全限定的域名) (例如, machine.company.com)。</span><span class="sxs-lookup"><span data-stu-id="4350c-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="4350c-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="4350c-113">isAzureAadJoined</span></span>|<span data-ttu-id="4350c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4350c-114">Boolean</span></span>|<span data-ttu-id="4350c-115">如此如果主机已加入域到 Azure Active Directory 域服务。</span><span class="sxs-lookup"><span data-stu-id="4350c-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="4350c-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="4350c-116">isAzureAadRegistered</span></span>|<span data-ttu-id="4350c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4350c-117">Boolean</span></span>|<span data-ttu-id="4350c-118">如果主机注册到 Azure Active Directory 设备注册 (BYOD 设备, 而不是由企业完全管理), 则该属性值为 True。</span><span class="sxs-lookup"><span data-stu-id="4350c-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="4350c-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="4350c-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="4350c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4350c-120">Boolean</span></span>|<span data-ttu-id="4350c-121">如此如果主机已加入域到本地 Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="4350c-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="4350c-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="4350c-122">netBiosName</span></span>|<span data-ttu-id="4350c-123">String</span><span class="sxs-lookup"><span data-stu-id="4350c-123">String</span></span>|<span data-ttu-id="4350c-124">本地主机名, 不包含 DNS 域名。</span><span class="sxs-lookup"><span data-stu-id="4350c-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="4350c-125">os</span><span class="sxs-lookup"><span data-stu-id="4350c-125">os</span></span>|<span data-ttu-id="4350c-126">String</span><span class="sxs-lookup"><span data-stu-id="4350c-126">String</span></span>|<span data-ttu-id="4350c-127">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="4350c-127">Host Operating System.</span></span> <span data-ttu-id="4350c-128">(例如, Windows10、MacOS、RHEL 等)。</span><span class="sxs-lookup"><span data-stu-id="4350c-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="4350c-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="4350c-129">privateIpAddress</span></span>|<span data-ttu-id="4350c-130">String</span><span class="sxs-lookup"><span data-stu-id="4350c-130">String</span></span>|<span data-ttu-id="4350c-131">在出现警报时专用 (不可路由) IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。</span><span class="sxs-lookup"><span data-stu-id="4350c-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="4350c-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="4350c-132">publicIpAddress</span></span>|<span data-ttu-id="4350c-133">String</span><span class="sxs-lookup"><span data-stu-id="4350c-133">String</span></span>|<span data-ttu-id="4350c-134">在警报时可公开路由的 IPv4 或 IPv6 地址 (请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918))。</span><span class="sxs-lookup"><span data-stu-id="4350c-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="4350c-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="4350c-135">riskScore</span></span>|<span data-ttu-id="4350c-136">String</span><span class="sxs-lookup"><span data-stu-id="4350c-136">String</span></span>|<span data-ttu-id="4350c-137">主机的提供程序生成/计算的风险分数。</span><span class="sxs-lookup"><span data-stu-id="4350c-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="4350c-138">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="4350c-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4350c-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4350c-139">JSON representation</span></span>

<span data-ttu-id="4350c-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4350c-140">The following is a JSON representation of the resource.</span></span>

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
