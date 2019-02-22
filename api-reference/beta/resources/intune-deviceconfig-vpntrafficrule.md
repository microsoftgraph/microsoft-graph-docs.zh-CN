---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd004341928260187518966e2356f59faff57898
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139940"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="db604-103">vpnTrafficRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="db604-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="db604-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db604-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db604-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db604-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db604-106">VPN 流量规则定义。</span><span class="sxs-lookup"><span data-stu-id="db604-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="db604-107">属性</span><span class="sxs-lookup"><span data-stu-id="db604-107">Properties</span></span>
|<span data-ttu-id="db604-108">属性</span><span class="sxs-lookup"><span data-stu-id="db604-108">Property</span></span>|<span data-ttu-id="db604-109">类型</span><span class="sxs-lookup"><span data-stu-id="db604-109">Type</span></span>|<span data-ttu-id="db604-110">说明</span><span class="sxs-lookup"><span data-stu-id="db604-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db604-111">name</span><span class="sxs-lookup"><span data-stu-id="db604-111">name</span></span>|<span data-ttu-id="db604-112">字符串</span><span class="sxs-lookup"><span data-stu-id="db604-112">String</span></span>|<span data-ttu-id="db604-113">别名.</span><span class="sxs-lookup"><span data-stu-id="db604-113">Name.</span></span>|
|<span data-ttu-id="db604-114">协议</span><span class="sxs-lookup"><span data-stu-id="db604-114">protocols</span></span>|<span data-ttu-id="db604-115">Int32</span><span class="sxs-lookup"><span data-stu-id="db604-115">Int32</span></span>|<span data-ttu-id="db604-116">协议 (0-255)。</span><span class="sxs-lookup"><span data-stu-id="db604-116">Protocols (0-255).</span></span> <span data-ttu-id="db604-117">有效值为0至255</span><span class="sxs-lookup"><span data-stu-id="db604-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="db604-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="db604-118">localPortRanges</span></span>|<span data-ttu-id="db604-119">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="db604-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="db604-120">仅当 protocol 为 TCP 或 UDP (6 或 17) 时, 才能设置本地端口范围。</span><span class="sxs-lookup"><span data-stu-id="db604-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="db604-121">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="db604-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="db604-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="db604-122">remotePortRanges</span></span>|<span data-ttu-id="db604-123">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="db604-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="db604-124">仅当 protocol 为 TCP 或 UDP (6 或 17) 时, 才能设置远程端口范围。</span><span class="sxs-lookup"><span data-stu-id="db604-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="db604-125">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="db604-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="db604-126">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="db604-126">localAddressRanges</span></span>|<span data-ttu-id="db604-127">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="db604-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="db604-128">本地地址范围。</span><span class="sxs-lookup"><span data-stu-id="db604-128">Local address range.</span></span> <span data-ttu-id="db604-129">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="db604-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="db604-130">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="db604-130">remoteAddressRanges</span></span>|<span data-ttu-id="db604-131">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="db604-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="db604-132">远程地址范围。</span><span class="sxs-lookup"><span data-stu-id="db604-132">Remote address range.</span></span> <span data-ttu-id="db604-133">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="db604-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="db604-134">appId</span><span class="sxs-lookup"><span data-stu-id="db604-134">appId</span></span>|<span data-ttu-id="db604-135">String</span><span class="sxs-lookup"><span data-stu-id="db604-135">String</span></span>|<span data-ttu-id="db604-136">应用程序标识符 (如果应用程序触发此流量规则)。</span><span class="sxs-lookup"><span data-stu-id="db604-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="db604-137">appType</span><span class="sxs-lookup"><span data-stu-id="db604-137">appType</span></span>|[<span data-ttu-id="db604-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="db604-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="db604-139">应用程序类型 (如果应用程序触发此流量规则)。</span><span class="sxs-lookup"><span data-stu-id="db604-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="db604-140">可取值为：`none`、`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="db604-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="db604-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="db604-141">routingPolicyType</span></span>|[<span data-ttu-id="db604-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="db604-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="db604-143">当应用程序触发时, 指示是否要沿此路由启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="db604-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="db604-144">可取值为：`none`、`splitTunnel`、`forceTunnel`。</span><span class="sxs-lookup"><span data-stu-id="db604-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="db604-145">声明</span><span class="sxs-lookup"><span data-stu-id="db604-145">claims</span></span>|<span data-ttu-id="db604-146">字符串</span><span class="sxs-lookup"><span data-stu-id="db604-146">String</span></span>|<span data-ttu-id="db604-147">与此流量规则关联的声明。</span><span class="sxs-lookup"><span data-stu-id="db604-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db604-148">关系</span><span class="sxs-lookup"><span data-stu-id="db604-148">Relationships</span></span>
<span data-ttu-id="db604-149">无</span><span class="sxs-lookup"><span data-stu-id="db604-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db604-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db604-150">JSON Representation</span></span>
<span data-ttu-id="db604-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db604-151">Here is a JSON representation of the resource.</span></span>
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




