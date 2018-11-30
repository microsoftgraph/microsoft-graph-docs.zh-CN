---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: ae64d4e0f13e39cb344fd54f5e600cfbfe0dc4f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044895"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="c9165-104">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9165-104">hostSecurityState resource type</span></span>

 > <span data-ttu-id="c9165-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9165-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9165-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9165-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9165-107">包含状态信息 （包括设备、 计算机等） 的主机。</span><span class="sxs-lookup"><span data-stu-id="c9165-107">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="c9165-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9165-108">Properties</span></span>

| <span data-ttu-id="c9165-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9165-109">Property</span></span>   | <span data-ttu-id="c9165-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9165-110">Type</span></span>|<span data-ttu-id="c9165-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9165-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9165-112">fqdn</span><span class="sxs-lookup"><span data-stu-id="c9165-112">fqdn</span></span>|<span data-ttu-id="c9165-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c9165-113">String</span></span>|<span data-ttu-id="c9165-114">主机 FQDN （完全限定域名） (例如，machine.company.com)。</span><span class="sxs-lookup"><span data-stu-id="c9165-114">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="c9165-115">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="c9165-115">isAzureAadJoined</span></span>|<span data-ttu-id="c9165-116">布尔</span><span class="sxs-lookup"><span data-stu-id="c9165-116">Boolean</span></span>|<span data-ttu-id="c9165-117">如果主机是加入到 Azure Active Directory 域服务的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="c9165-117">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="c9165-118">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="c9165-118">isAzureAadRegistered</span></span>|<span data-ttu-id="c9165-119">布尔</span><span class="sxs-lookup"><span data-stu-id="c9165-119">Boolean</span></span>|<span data-ttu-id="c9165-120">如果主机注册 Azure Active Directory 设备注册 （BYOD 设备-，即不完全由企业管理），则为 true。</span><span class="sxs-lookup"><span data-stu-id="c9165-120">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="c9165-121">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="c9165-121">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="c9165-122">布尔</span><span class="sxs-lookup"><span data-stu-id="c9165-122">Boolean</span></span>|<span data-ttu-id="c9165-123">如果主机是加入本地 Active Directory 域的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="c9165-123">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="c9165-124">netBiosName</span><span class="sxs-lookup"><span data-stu-id="c9165-124">netBiosName</span></span>|<span data-ttu-id="c9165-125">字符串</span><span class="sxs-lookup"><span data-stu-id="c9165-125">String</span></span>|<span data-ttu-id="c9165-126">不带的 DNS 域名的本地主机名称。</span><span class="sxs-lookup"><span data-stu-id="c9165-126">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="c9165-127">操作系统</span><span class="sxs-lookup"><span data-stu-id="c9165-127">os</span></span>|<span data-ttu-id="c9165-128">字符串</span><span class="sxs-lookup"><span data-stu-id="c9165-128">String</span></span>|<span data-ttu-id="c9165-129">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="c9165-129">Host Operating System.</span></span> <span data-ttu-id="c9165-130">（例如，Windows10 MacOS、 RHEL，等）。</span><span class="sxs-lookup"><span data-stu-id="c9165-130">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="c9165-131">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="c9165-131">privateIpAddress</span></span>|<span data-ttu-id="c9165-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c9165-132">String</span></span>|<span data-ttu-id="c9165-133">专用 （不可穿） 的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。</span><span class="sxs-lookup"><span data-stu-id="c9165-133">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="c9165-134">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="c9165-134">publicIpAddress</span></span>|<span data-ttu-id="c9165-135">字符串</span><span class="sxs-lookup"><span data-stu-id="c9165-135">String</span></span>|<span data-ttu-id="c9165-136">公共可路由的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。</span><span class="sxs-lookup"><span data-stu-id="c9165-136">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="c9165-137">riskScore</span><span class="sxs-lookup"><span data-stu-id="c9165-137">riskScore</span></span>|<span data-ttu-id="c9165-138">字符串</span><span class="sxs-lookup"><span data-stu-id="c9165-138">String</span></span>|<span data-ttu-id="c9165-139">带有提供程序生成/计算风险的主机的分数。</span><span class="sxs-lookup"><span data-stu-id="c9165-139">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="c9165-140">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="c9165-140">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9165-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9165-141">JSON representation</span></span>

<span data-ttu-id="c9165-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9165-142">The following is a JSON representation of the resource.</span></span>

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
