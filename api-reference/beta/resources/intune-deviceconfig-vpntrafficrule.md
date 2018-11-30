---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
ms.openlocfilehash: 564528cf0c0ae39785a2cc43dc800d8dbdf7d285
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043304"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="2791f-103">vpnTrafficRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="2791f-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="2791f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2791f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2791f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2791f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2791f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2791f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2791f-107">VPN 流量规则定义。</span><span class="sxs-lookup"><span data-stu-id="2791f-107">VPN Traffic Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="2791f-108">属性</span><span class="sxs-lookup"><span data-stu-id="2791f-108">Properties</span></span>
|<span data-ttu-id="2791f-109">属性</span><span class="sxs-lookup"><span data-stu-id="2791f-109">Property</span></span>|<span data-ttu-id="2791f-110">类型</span><span class="sxs-lookup"><span data-stu-id="2791f-110">Type</span></span>|<span data-ttu-id="2791f-111">说明</span><span class="sxs-lookup"><span data-stu-id="2791f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2791f-112">name</span><span class="sxs-lookup"><span data-stu-id="2791f-112">name</span></span>|<span data-ttu-id="2791f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="2791f-113">String</span></span>|<span data-ttu-id="2791f-114">名称。</span><span class="sxs-lookup"><span data-stu-id="2791f-114">Name.</span></span>|
|<span data-ttu-id="2791f-115">协议</span><span class="sxs-lookup"><span data-stu-id="2791f-115">protocols</span></span>|<span data-ttu-id="2791f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2791f-116">Int32</span></span>|<span data-ttu-id="2791f-117">协议 (0-255)。</span><span class="sxs-lookup"><span data-stu-id="2791f-117">Protocols (0-255).</span></span> <span data-ttu-id="2791f-118">0 到 255 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="2791f-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="2791f-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="2791f-119">localPortRanges</span></span>|<span data-ttu-id="2791f-120">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="2791f-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="2791f-121">仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置本地端口范围。</span><span class="sxs-lookup"><span data-stu-id="2791f-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="2791f-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2791f-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2791f-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="2791f-123">remotePortRanges</span></span>|<span data-ttu-id="2791f-124">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="2791f-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="2791f-125">仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置远程端口范围。</span><span class="sxs-lookup"><span data-stu-id="2791f-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="2791f-126">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2791f-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2791f-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="2791f-127">localAddressRanges</span></span>|<span data-ttu-id="2791f-128">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="2791f-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="2791f-129">本地地址范围。</span><span class="sxs-lookup"><span data-stu-id="2791f-129">Local address range.</span></span> <span data-ttu-id="2791f-130">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2791f-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2791f-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="2791f-131">remoteAddressRanges</span></span>|<span data-ttu-id="2791f-132">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="2791f-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="2791f-133">远程地址范围。</span><span class="sxs-lookup"><span data-stu-id="2791f-133">Remote address range.</span></span> <span data-ttu-id="2791f-134">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2791f-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2791f-135">appId</span><span class="sxs-lookup"><span data-stu-id="2791f-135">appId</span></span>|<span data-ttu-id="2791f-136">String</span><span class="sxs-lookup"><span data-stu-id="2791f-136">String</span></span>|<span data-ttu-id="2791f-137">应用程序标识符，如果此通信规则触发应用程序。</span><span class="sxs-lookup"><span data-stu-id="2791f-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="2791f-138">appType</span><span class="sxs-lookup"><span data-stu-id="2791f-138">appType</span></span>|[<span data-ttu-id="2791f-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="2791f-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="2791f-140">应用程序类型，如果此通信规则触发应用程序。</span><span class="sxs-lookup"><span data-stu-id="2791f-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="2791f-141">可取值为：`none`、`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="2791f-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="2791f-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="2791f-142">routingPolicyType</span></span>|[<span data-ttu-id="2791f-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="2791f-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="2791f-144">当应用程序触发，该值指示是否启用拆分隧道此路由。</span><span class="sxs-lookup"><span data-stu-id="2791f-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="2791f-145">可取值为：`none`、`splitTunnel`、`forceTunnel`。</span><span class="sxs-lookup"><span data-stu-id="2791f-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="2791f-146">声明</span><span class="sxs-lookup"><span data-stu-id="2791f-146">claims</span></span>|<span data-ttu-id="2791f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="2791f-147">String</span></span>|<span data-ttu-id="2791f-148">与此通信规则关联的声明。</span><span class="sxs-lookup"><span data-stu-id="2791f-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2791f-149">Relationships</span><span class="sxs-lookup"><span data-stu-id="2791f-149">Relationships</span></span>
<span data-ttu-id="2791f-150">无</span><span class="sxs-lookup"><span data-stu-id="2791f-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2791f-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2791f-151">JSON Representation</span></span>
<span data-ttu-id="2791f-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2791f-152">Here is a JSON representation of the resource.</span></span>
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





