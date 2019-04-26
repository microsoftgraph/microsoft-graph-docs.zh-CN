---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c22ead3b037ff18dbd9c1dedbf68b11f2b55a3bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555008"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="0f199-103">vpnTrafficRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f199-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="0f199-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f199-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f199-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f199-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f199-106">VPN 流量规则定义。</span><span class="sxs-lookup"><span data-stu-id="0f199-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0f199-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f199-107">Properties</span></span>
|<span data-ttu-id="0f199-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f199-108">Property</span></span>|<span data-ttu-id="0f199-109">类型</span><span class="sxs-lookup"><span data-stu-id="0f199-109">Type</span></span>|<span data-ttu-id="0f199-110">说明</span><span class="sxs-lookup"><span data-stu-id="0f199-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f199-111">name</span><span class="sxs-lookup"><span data-stu-id="0f199-111">name</span></span>|<span data-ttu-id="0f199-112">String</span><span class="sxs-lookup"><span data-stu-id="0f199-112">String</span></span>|<span data-ttu-id="0f199-113">别名.</span><span class="sxs-lookup"><span data-stu-id="0f199-113">Name.</span></span>|
|<span data-ttu-id="0f199-114">协议</span><span class="sxs-lookup"><span data-stu-id="0f199-114">protocols</span></span>|<span data-ttu-id="0f199-115">Int32</span><span class="sxs-lookup"><span data-stu-id="0f199-115">Int32</span></span>|<span data-ttu-id="0f199-116">协议 (0-255)。</span><span class="sxs-lookup"><span data-stu-id="0f199-116">Protocols (0-255).</span></span> <span data-ttu-id="0f199-117">有效值为0至255</span><span class="sxs-lookup"><span data-stu-id="0f199-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="0f199-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="0f199-118">localPortRanges</span></span>|<span data-ttu-id="0f199-119">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f199-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="0f199-120">仅当 protocol 为 TCP 或 UDP (6 或 17) 时, 才能设置本地端口范围。</span><span class="sxs-lookup"><span data-stu-id="0f199-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="0f199-121">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0f199-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0f199-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="0f199-122">remotePortRanges</span></span>|<span data-ttu-id="0f199-123">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f199-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="0f199-124">仅当 protocol 为 TCP 或 UDP (6 或 17) 时, 才能设置远程端口范围。</span><span class="sxs-lookup"><span data-stu-id="0f199-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="0f199-125">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0f199-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0f199-126">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="0f199-126">localAddressRanges</span></span>|<span data-ttu-id="0f199-127">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f199-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="0f199-128">本地地址范围。</span><span class="sxs-lookup"><span data-stu-id="0f199-128">Local address range.</span></span> <span data-ttu-id="0f199-129">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0f199-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0f199-130">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="0f199-130">remoteAddressRanges</span></span>|<span data-ttu-id="0f199-131">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f199-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="0f199-132">远程地址范围。</span><span class="sxs-lookup"><span data-stu-id="0f199-132">Remote address range.</span></span> <span data-ttu-id="0f199-133">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0f199-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0f199-134">appId</span><span class="sxs-lookup"><span data-stu-id="0f199-134">appId</span></span>|<span data-ttu-id="0f199-135">String</span><span class="sxs-lookup"><span data-stu-id="0f199-135">String</span></span>|<span data-ttu-id="0f199-136">应用程序标识符 (如果应用程序触发此流量规则)。</span><span class="sxs-lookup"><span data-stu-id="0f199-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="0f199-137">appType</span><span class="sxs-lookup"><span data-stu-id="0f199-137">appType</span></span>|[<span data-ttu-id="0f199-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="0f199-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="0f199-139">应用程序类型 (如果应用程序触发此流量规则)。</span><span class="sxs-lookup"><span data-stu-id="0f199-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="0f199-140">可取值为：`none`、`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="0f199-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="0f199-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="0f199-141">routingPolicyType</span></span>|[<span data-ttu-id="0f199-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="0f199-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="0f199-143">当应用程序触发时, 指示是否要沿此路由启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="0f199-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="0f199-144">可取值为：`none`、`splitTunnel`、`forceTunnel`。</span><span class="sxs-lookup"><span data-stu-id="0f199-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="0f199-145">声称</span><span class="sxs-lookup"><span data-stu-id="0f199-145">claims</span></span>|<span data-ttu-id="0f199-146">String</span><span class="sxs-lookup"><span data-stu-id="0f199-146">String</span></span>|<span data-ttu-id="0f199-147">与此流量规则关联的声明。</span><span class="sxs-lookup"><span data-stu-id="0f199-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f199-148">关系</span><span class="sxs-lookup"><span data-stu-id="0f199-148">Relationships</span></span>
<span data-ttu-id="0f199-149">无</span><span class="sxs-lookup"><span data-stu-id="0f199-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f199-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f199-150">JSON Representation</span></span>
<span data-ttu-id="0f199-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f199-151">Here is a JSON representation of the resource.</span></span>
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





