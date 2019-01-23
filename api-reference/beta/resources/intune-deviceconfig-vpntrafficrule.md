---
title: vpnTrafficRule 资源类型
description: VPN 流量规则定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415283"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="8932f-103">vpnTrafficRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="8932f-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="8932f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8932f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8932f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8932f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8932f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8932f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8932f-107">VPN 流量规则定义。</span><span class="sxs-lookup"><span data-stu-id="8932f-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8932f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8932f-108">Properties</span></span>
|<span data-ttu-id="8932f-109">属性</span><span class="sxs-lookup"><span data-stu-id="8932f-109">Property</span></span>|<span data-ttu-id="8932f-110">类型</span><span class="sxs-lookup"><span data-stu-id="8932f-110">Type</span></span>|<span data-ttu-id="8932f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8932f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8932f-112">name</span><span class="sxs-lookup"><span data-stu-id="8932f-112">name</span></span>|<span data-ttu-id="8932f-113">String</span><span class="sxs-lookup"><span data-stu-id="8932f-113">String</span></span>|<span data-ttu-id="8932f-114">名称。</span><span class="sxs-lookup"><span data-stu-id="8932f-114">Name.</span></span>|
|<span data-ttu-id="8932f-115">协议</span><span class="sxs-lookup"><span data-stu-id="8932f-115">protocols</span></span>|<span data-ttu-id="8932f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8932f-116">Int32</span></span>|<span data-ttu-id="8932f-117">协议 (0-255)。</span><span class="sxs-lookup"><span data-stu-id="8932f-117">Protocols (0-255).</span></span> <span data-ttu-id="8932f-118">0 到 255 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="8932f-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="8932f-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="8932f-119">localPortRanges</span></span>|<span data-ttu-id="8932f-120">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="8932f-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="8932f-121">仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置本地端口范围。</span><span class="sxs-lookup"><span data-stu-id="8932f-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="8932f-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8932f-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8932f-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="8932f-123">remotePortRanges</span></span>|<span data-ttu-id="8932f-124">[numberRange](../resources/intune-deviceconfig-numberrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="8932f-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="8932f-125">仅当协议是 TCP 或 UDP （6 或 17） 时，可以设置远程端口范围。</span><span class="sxs-lookup"><span data-stu-id="8932f-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="8932f-126">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8932f-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8932f-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="8932f-127">localAddressRanges</span></span>|<span data-ttu-id="8932f-128">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="8932f-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="8932f-129">本地地址范围。</span><span class="sxs-lookup"><span data-stu-id="8932f-129">Local address range.</span></span> <span data-ttu-id="8932f-130">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8932f-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8932f-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="8932f-131">remoteAddressRanges</span></span>|<span data-ttu-id="8932f-132">[iPv4Range](../resources/intune-shared-ipv4range.md)集合</span><span class="sxs-lookup"><span data-stu-id="8932f-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="8932f-133">远程地址范围。</span><span class="sxs-lookup"><span data-stu-id="8932f-133">Remote address range.</span></span> <span data-ttu-id="8932f-134">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8932f-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8932f-135">appId</span><span class="sxs-lookup"><span data-stu-id="8932f-135">appId</span></span>|<span data-ttu-id="8932f-136">String</span><span class="sxs-lookup"><span data-stu-id="8932f-136">String</span></span>|<span data-ttu-id="8932f-137">应用程序标识符，如果此通信规则触发应用程序。</span><span class="sxs-lookup"><span data-stu-id="8932f-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="8932f-138">appType</span><span class="sxs-lookup"><span data-stu-id="8932f-138">appType</span></span>|[<span data-ttu-id="8932f-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="8932f-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="8932f-140">应用程序类型，如果此通信规则触发应用程序。</span><span class="sxs-lookup"><span data-stu-id="8932f-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="8932f-141">可取值为：`none`、`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="8932f-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="8932f-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="8932f-142">routingPolicyType</span></span>|[<span data-ttu-id="8932f-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="8932f-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="8932f-144">当应用程序触发，该值指示是否启用拆分隧道此路由。</span><span class="sxs-lookup"><span data-stu-id="8932f-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="8932f-145">可取值为：`none`、`splitTunnel`、`forceTunnel`。</span><span class="sxs-lookup"><span data-stu-id="8932f-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="8932f-146">声明</span><span class="sxs-lookup"><span data-stu-id="8932f-146">claims</span></span>|<span data-ttu-id="8932f-147">String</span><span class="sxs-lookup"><span data-stu-id="8932f-147">String</span></span>|<span data-ttu-id="8932f-148">与此通信规则关联的声明。</span><span class="sxs-lookup"><span data-stu-id="8932f-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8932f-149">关系</span><span class="sxs-lookup"><span data-stu-id="8932f-149">Relationships</span></span>
<span data-ttu-id="8932f-150">无</span><span class="sxs-lookup"><span data-stu-id="8932f-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8932f-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8932f-151">JSON Representation</span></span>
<span data-ttu-id="8932f-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8932f-152">Here is a JSON representation of the resource.</span></span>
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




