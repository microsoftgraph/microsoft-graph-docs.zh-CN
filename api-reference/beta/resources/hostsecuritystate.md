---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec4b6ba22aceaaaeb3c612f61eb522bfe14243c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496864"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="ab928-104">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab928-104">hostSecurityState resource type</span></span>

<span data-ttu-id="ab928-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ab928-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab928-106">包含有关主机的状态信息（包括设备、计算机等）。</span><span class="sxs-lookup"><span data-stu-id="ab928-106">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="ab928-107">属性</span><span class="sxs-lookup"><span data-stu-id="ab928-107">Properties</span></span>

| <span data-ttu-id="ab928-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab928-108">Property</span></span>   | <span data-ttu-id="ab928-109">类型</span><span class="sxs-lookup"><span data-stu-id="ab928-109">Type</span></span>|<span data-ttu-id="ab928-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab928-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab928-111">域名</span><span class="sxs-lookup"><span data-stu-id="ab928-111">fqdn</span></span>|<span data-ttu-id="ab928-112">String</span><span class="sxs-lookup"><span data-stu-id="ab928-112">String</span></span>|<span data-ttu-id="ab928-113">主机 FQDN （完全限定的域名）（例如，machine.company.com）。</span><span class="sxs-lookup"><span data-stu-id="ab928-113">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="ab928-114">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="ab928-114">isAzureAadJoined</span></span>|<span data-ttu-id="ab928-115">布尔</span><span class="sxs-lookup"><span data-stu-id="ab928-115">Boolean</span></span>|<span data-ttu-id="ab928-116">如此如果主机已加入域到 Azure Active Directory 域服务。</span><span class="sxs-lookup"><span data-stu-id="ab928-116">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="ab928-117">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="ab928-117">isAzureAadRegistered</span></span>|<span data-ttu-id="ab928-118">布尔</span><span class="sxs-lookup"><span data-stu-id="ab928-118">Boolean</span></span>|<span data-ttu-id="ab928-119">如果主机注册到 Azure Active Directory 设备注册（BYOD 设备，而不是由企业完全管理），则该属性值为 True。</span><span class="sxs-lookup"><span data-stu-id="ab928-119">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="ab928-120">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="ab928-120">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="ab928-121">布尔</span><span class="sxs-lookup"><span data-stu-id="ab928-121">Boolean</span></span>|<span data-ttu-id="ab928-122">如此如果主机已加入域到本地 Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="ab928-122">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="ab928-123">netBiosName</span><span class="sxs-lookup"><span data-stu-id="ab928-123">netBiosName</span></span>|<span data-ttu-id="ab928-124">String</span><span class="sxs-lookup"><span data-stu-id="ab928-124">String</span></span>|<span data-ttu-id="ab928-125">本地主机名，不包含 DNS 域名。</span><span class="sxs-lookup"><span data-stu-id="ab928-125">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="ab928-126">os</span><span class="sxs-lookup"><span data-stu-id="ab928-126">os</span></span>|<span data-ttu-id="ab928-127">String</span><span class="sxs-lookup"><span data-stu-id="ab928-127">String</span></span>|<span data-ttu-id="ab928-128">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="ab928-128">Host Operating System.</span></span> <span data-ttu-id="ab928-129">（例如，Windows10、MacOS、RHEL 等）。</span><span class="sxs-lookup"><span data-stu-id="ab928-129">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="ab928-130">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="ab928-130">privateIpAddress</span></span>|<span data-ttu-id="ab928-131">String</span><span class="sxs-lookup"><span data-stu-id="ab928-131">String</span></span>|<span data-ttu-id="ab928-132">在出现警报时专用（不可路由） IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。</span><span class="sxs-lookup"><span data-stu-id="ab928-132">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="ab928-133">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="ab928-133">publicIpAddress</span></span>|<span data-ttu-id="ab928-134">String</span><span class="sxs-lookup"><span data-stu-id="ab928-134">String</span></span>|<span data-ttu-id="ab928-135">在警报时可公开路由的 IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。</span><span class="sxs-lookup"><span data-stu-id="ab928-135">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="ab928-136">riskScore</span><span class="sxs-lookup"><span data-stu-id="ab928-136">riskScore</span></span>|<span data-ttu-id="ab928-137">String</span><span class="sxs-lookup"><span data-stu-id="ab928-137">String</span></span>|<span data-ttu-id="ab928-138">主机的提供程序生成/计算的风险分数。</span><span class="sxs-lookup"><span data-stu-id="ab928-138">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="ab928-139">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="ab928-139">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab928-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab928-140">JSON representation</span></span>

<span data-ttu-id="ab928-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab928-141">The following is a JSON representation of the resource.</span></span>

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
