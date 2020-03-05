---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9eecec1ca70b897f88003b884ea3e5e3a024a7b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529280"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="51605-103">vpnTrafficRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="51605-103">vpnTrafficRule resource type</span></span>

<span data-ttu-id="51605-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="51605-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51605-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51605-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51605-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51605-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51605-107">VPN 流量规则定义。</span><span class="sxs-lookup"><span data-stu-id="51605-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="51605-108">属性</span><span class="sxs-lookup"><span data-stu-id="51605-108">Properties</span></span>
|<span data-ttu-id="51605-109">属性</span><span class="sxs-lookup"><span data-stu-id="51605-109">Property</span></span>|<span data-ttu-id="51605-110">类型</span><span class="sxs-lookup"><span data-stu-id="51605-110">Type</span></span>|<span data-ttu-id="51605-111">说明</span><span class="sxs-lookup"><span data-stu-id="51605-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51605-112">name</span><span class="sxs-lookup"><span data-stu-id="51605-112">name</span></span>|<span data-ttu-id="51605-113">字符串</span><span class="sxs-lookup"><span data-stu-id="51605-113">String</span></span>|<span data-ttu-id="51605-114">别名.</span><span class="sxs-lookup"><span data-stu-id="51605-114">Name.</span></span>|
|<span data-ttu-id="51605-115">协议</span><span class="sxs-lookup"><span data-stu-id="51605-115">protocols</span></span>|<span data-ttu-id="51605-116">Int32</span><span class="sxs-lookup"><span data-stu-id="51605-116">Int32</span></span>|<span data-ttu-id="51605-117">协议（0-255）。</span><span class="sxs-lookup"><span data-stu-id="51605-117">Protocols (0-255).</span></span> <span data-ttu-id="51605-118">有效值为0至255</span><span class="sxs-lookup"><span data-stu-id="51605-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="51605-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="51605-119">localPortRanges</span></span>|<span data-ttu-id="51605-120">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="51605-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="51605-121">仅当 protocol 为 TCP 或 UDP （6或17）时，才能设置本地端口范围。</span><span class="sxs-lookup"><span data-stu-id="51605-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="51605-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="51605-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51605-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="51605-123">remotePortRanges</span></span>|<span data-ttu-id="51605-124">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="51605-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="51605-125">仅当 protocol 为 TCP 或 UDP （6或17）时，才能设置远程端口范围。</span><span class="sxs-lookup"><span data-stu-id="51605-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="51605-126">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="51605-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51605-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="51605-127">localAddressRanges</span></span>|<span data-ttu-id="51605-128">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="51605-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="51605-129">本地地址范围。</span><span class="sxs-lookup"><span data-stu-id="51605-129">Local address range.</span></span> <span data-ttu-id="51605-130">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="51605-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51605-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="51605-131">remoteAddressRanges</span></span>|<span data-ttu-id="51605-132">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="51605-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="51605-133">远程地址范围。</span><span class="sxs-lookup"><span data-stu-id="51605-133">Remote address range.</span></span> <span data-ttu-id="51605-134">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="51605-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51605-135">appId</span><span class="sxs-lookup"><span data-stu-id="51605-135">appId</span></span>|<span data-ttu-id="51605-136">String</span><span class="sxs-lookup"><span data-stu-id="51605-136">String</span></span>|<span data-ttu-id="51605-137">应用程序标识符（如果应用程序触发此流量规则）。</span><span class="sxs-lookup"><span data-stu-id="51605-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="51605-138">appType</span><span class="sxs-lookup"><span data-stu-id="51605-138">appType</span></span>|[<span data-ttu-id="51605-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="51605-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="51605-140">应用程序类型（如果应用程序触发此流量规则）。</span><span class="sxs-lookup"><span data-stu-id="51605-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="51605-141">可取值为：`none`、`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="51605-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="51605-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="51605-142">routingPolicyType</span></span>|[<span data-ttu-id="51605-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="51605-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="51605-144">当应用程序触发时，指示是否要沿此路由启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="51605-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="51605-145">可取值为：`none`、`splitTunnel`、`forceTunnel`。</span><span class="sxs-lookup"><span data-stu-id="51605-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="51605-146">声称</span><span class="sxs-lookup"><span data-stu-id="51605-146">claims</span></span>|<span data-ttu-id="51605-147">String</span><span class="sxs-lookup"><span data-stu-id="51605-147">String</span></span>|<span data-ttu-id="51605-148">与此流量规则关联的声明。</span><span class="sxs-lookup"><span data-stu-id="51605-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51605-149">关系</span><span class="sxs-lookup"><span data-stu-id="51605-149">Relationships</span></span>
<span data-ttu-id="51605-150">无</span><span class="sxs-lookup"><span data-stu-id="51605-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51605-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51605-151">JSON Representation</span></span>
<span data-ttu-id="51605-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51605-152">Here is a JSON representation of the resource.</span></span>
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



