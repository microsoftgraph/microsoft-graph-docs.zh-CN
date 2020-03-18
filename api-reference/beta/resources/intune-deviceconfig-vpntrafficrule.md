---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad75e1c4f226952ce75942b006d3a993fcd4274b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787297"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="52ad1-103">vpnTrafficRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="52ad1-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="52ad1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="52ad1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52ad1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52ad1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52ad1-106">VPN 流量规则定义。</span><span class="sxs-lookup"><span data-stu-id="52ad1-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="52ad1-107">属性</span><span class="sxs-lookup"><span data-stu-id="52ad1-107">Properties</span></span>
|<span data-ttu-id="52ad1-108">属性</span><span class="sxs-lookup"><span data-stu-id="52ad1-108">Property</span></span>|<span data-ttu-id="52ad1-109">类型</span><span class="sxs-lookup"><span data-stu-id="52ad1-109">Type</span></span>|<span data-ttu-id="52ad1-110">说明</span><span class="sxs-lookup"><span data-stu-id="52ad1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52ad1-111">name</span><span class="sxs-lookup"><span data-stu-id="52ad1-111">name</span></span>|<span data-ttu-id="52ad1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="52ad1-112">String</span></span>|<span data-ttu-id="52ad1-113">别名.</span><span class="sxs-lookup"><span data-stu-id="52ad1-113">Name.</span></span>|
|<span data-ttu-id="52ad1-114">协议</span><span class="sxs-lookup"><span data-stu-id="52ad1-114">protocols</span></span>|<span data-ttu-id="52ad1-115">Int32</span><span class="sxs-lookup"><span data-stu-id="52ad1-115">Int32</span></span>|<span data-ttu-id="52ad1-116">协议（0-255）。</span><span class="sxs-lookup"><span data-stu-id="52ad1-116">Protocols (0-255).</span></span> <span data-ttu-id="52ad1-117">有效值为0至255</span><span class="sxs-lookup"><span data-stu-id="52ad1-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="52ad1-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="52ad1-118">localPortRanges</span></span>|<span data-ttu-id="52ad1-119">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="52ad1-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="52ad1-120">仅当 protocol 为 TCP 或 UDP （6或17）时，才能设置本地端口范围。</span><span class="sxs-lookup"><span data-stu-id="52ad1-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="52ad1-121">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="52ad1-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="52ad1-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="52ad1-122">remotePortRanges</span></span>|<span data-ttu-id="52ad1-123">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="52ad1-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="52ad1-124">仅当 protocol 为 TCP 或 UDP （6或17）时，才能设置远程端口范围。</span><span class="sxs-lookup"><span data-stu-id="52ad1-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="52ad1-125">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="52ad1-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="52ad1-126">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="52ad1-126">localAddressRanges</span></span>|<span data-ttu-id="52ad1-127">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="52ad1-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="52ad1-128">本地地址范围。</span><span class="sxs-lookup"><span data-stu-id="52ad1-128">Local address range.</span></span> <span data-ttu-id="52ad1-129">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="52ad1-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="52ad1-130">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="52ad1-130">remoteAddressRanges</span></span>|<span data-ttu-id="52ad1-131">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="52ad1-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="52ad1-132">远程地址范围。</span><span class="sxs-lookup"><span data-stu-id="52ad1-132">Remote address range.</span></span> <span data-ttu-id="52ad1-133">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="52ad1-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="52ad1-134">appId</span><span class="sxs-lookup"><span data-stu-id="52ad1-134">appId</span></span>|<span data-ttu-id="52ad1-135">String</span><span class="sxs-lookup"><span data-stu-id="52ad1-135">String</span></span>|<span data-ttu-id="52ad1-136">应用程序标识符（如果应用程序触发此流量规则）。</span><span class="sxs-lookup"><span data-stu-id="52ad1-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="52ad1-137">appType</span><span class="sxs-lookup"><span data-stu-id="52ad1-137">appType</span></span>|[<span data-ttu-id="52ad1-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="52ad1-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="52ad1-139">应用程序类型（如果应用程序触发此流量规则）。</span><span class="sxs-lookup"><span data-stu-id="52ad1-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="52ad1-140">可取值为：`none`、`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="52ad1-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="52ad1-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="52ad1-141">routingPolicyType</span></span>|[<span data-ttu-id="52ad1-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="52ad1-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="52ad1-143">当应用程序触发时，指示是否要沿此路由启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="52ad1-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="52ad1-144">可取值为：`none`、`splitTunnel`、`forceTunnel`。</span><span class="sxs-lookup"><span data-stu-id="52ad1-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="52ad1-145">声称</span><span class="sxs-lookup"><span data-stu-id="52ad1-145">claims</span></span>|<span data-ttu-id="52ad1-146">String</span><span class="sxs-lookup"><span data-stu-id="52ad1-146">String</span></span>|<span data-ttu-id="52ad1-147">与此流量规则关联的声明。</span><span class="sxs-lookup"><span data-stu-id="52ad1-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52ad1-148">关系</span><span class="sxs-lookup"><span data-stu-id="52ad1-148">Relationships</span></span>
<span data-ttu-id="52ad1-149">无</span><span class="sxs-lookup"><span data-stu-id="52ad1-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52ad1-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52ad1-150">JSON Representation</span></span>
<span data-ttu-id="52ad1-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52ad1-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```



