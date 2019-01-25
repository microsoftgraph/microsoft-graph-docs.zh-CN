---
title: hostSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526695"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="169b2-104">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="169b2-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="169b2-105">包含状态信息 （包括设备、 计算机等） 的主机。</span><span class="sxs-lookup"><span data-stu-id="169b2-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="169b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="169b2-106">Properties</span></span>

| <span data-ttu-id="169b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="169b2-107">Property</span></span>   | <span data-ttu-id="169b2-108">类型</span><span class="sxs-lookup"><span data-stu-id="169b2-108">Type</span></span>|<span data-ttu-id="169b2-109">说明</span><span class="sxs-lookup"><span data-stu-id="169b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="169b2-110">fqdn</span><span class="sxs-lookup"><span data-stu-id="169b2-110">fqdn</span></span>|<span data-ttu-id="169b2-111">String</span><span class="sxs-lookup"><span data-stu-id="169b2-111">String</span></span>|<span data-ttu-id="169b2-112">主机 FQDN （完全限定域名） (例如，machine.company.com)。</span><span class="sxs-lookup"><span data-stu-id="169b2-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="169b2-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="169b2-113">isAzureAadJoined</span></span>|<span data-ttu-id="169b2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="169b2-114">Boolean</span></span>|<span data-ttu-id="169b2-115">如果主机是加入到 Azure Active Directory 域服务的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="169b2-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="169b2-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="169b2-116">isAzureAadRegistered</span></span>|<span data-ttu-id="169b2-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="169b2-117">Boolean</span></span>|<span data-ttu-id="169b2-118">如果主机注册 Azure Active Directory 设备注册 （BYOD 设备-，即不完全由企业管理），则为 true。</span><span class="sxs-lookup"><span data-stu-id="169b2-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="169b2-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="169b2-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="169b2-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="169b2-120">Boolean</span></span>|<span data-ttu-id="169b2-121">如果主机是加入本地 Active Directory 域的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="169b2-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="169b2-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="169b2-122">netBiosName</span></span>|<span data-ttu-id="169b2-123">String</span><span class="sxs-lookup"><span data-stu-id="169b2-123">String</span></span>|<span data-ttu-id="169b2-124">不带的 DNS 域名的本地主机名称。</span><span class="sxs-lookup"><span data-stu-id="169b2-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="169b2-125">I-5.</span><span class="sxs-lookup"><span data-stu-id="169b2-125">os</span></span>|<span data-ttu-id="169b2-126">String</span><span class="sxs-lookup"><span data-stu-id="169b2-126">String</span></span>|<span data-ttu-id="169b2-127">主机操作系统。</span><span class="sxs-lookup"><span data-stu-id="169b2-127">Host Operating System.</span></span> <span data-ttu-id="169b2-128">（例如，Windows10 MacOS、 RHEL，等）。</span><span class="sxs-lookup"><span data-stu-id="169b2-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="169b2-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="169b2-129">privateIpAddress</span></span>|<span data-ttu-id="169b2-130">String</span><span class="sxs-lookup"><span data-stu-id="169b2-130">String</span></span>|<span data-ttu-id="169b2-131">专用 （不可穿） 的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。</span><span class="sxs-lookup"><span data-stu-id="169b2-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="169b2-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="169b2-132">publicIpAddress</span></span>|<span data-ttu-id="169b2-133">String</span><span class="sxs-lookup"><span data-stu-id="169b2-133">String</span></span>|<span data-ttu-id="169b2-134">公共可路由的 IPv4 或 IPv6 地址 （请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)） 在通知的时间。</span><span class="sxs-lookup"><span data-stu-id="169b2-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="169b2-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="169b2-135">riskScore</span></span>|<span data-ttu-id="169b2-136">String</span><span class="sxs-lookup"><span data-stu-id="169b2-136">String</span></span>|<span data-ttu-id="169b2-137">带有提供程序生成/计算风险的主机的分数。</span><span class="sxs-lookup"><span data-stu-id="169b2-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="169b2-138">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="169b2-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="169b2-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="169b2-139">JSON representation</span></span>

<span data-ttu-id="169b2-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="169b2-140">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
