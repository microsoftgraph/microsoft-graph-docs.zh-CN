---
title: cloudAppSecurityState 资源类型
description: 包含状态信息的云应用程序 （destinationServiceName、 destinationServiceIp）。
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876802"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="dd4b2-103">cloudAppSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd4b2-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="dd4b2-104">包含状态信息的云应用程序 （destinationServiceName、 destinationServiceIp）。</span><span class="sxs-lookup"><span data-stu-id="dd4b2-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="dd4b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd4b2-105">Properties</span></span>

| <span data-ttu-id="dd4b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd4b2-106">Property</span></span>     | <span data-ttu-id="dd4b2-107">类型</span><span class="sxs-lookup"><span data-stu-id="dd4b2-107">Type</span></span>        | <span data-ttu-id="dd4b2-108">Description</span><span class="sxs-lookup"><span data-stu-id="dd4b2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd4b2-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="dd4b2-109">destinationServiceIp</span></span>|<span data-ttu-id="dd4b2-110">字符串</span><span class="sxs-lookup"><span data-stu-id="dd4b2-110">String</span></span>|<span data-ttu-id="dd4b2-111">连接到云应用程序/服务的目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="dd4b2-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="dd4b2-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="dd4b2-112">destinationServiceName</span></span>|<span data-ttu-id="dd4b2-113">字符串</span><span class="sxs-lookup"><span data-stu-id="dd4b2-113">String</span></span>|<span data-ttu-id="dd4b2-114">云应用程序/服务名称 （例如"销售"、"收存箱"等）。</span><span class="sxs-lookup"><span data-stu-id="dd4b2-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="dd4b2-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="dd4b2-115">riskScore</span></span>|<span data-ttu-id="dd4b2-116">字符串</span><span class="sxs-lookup"><span data-stu-id="dd4b2-116">String</span></span>|<span data-ttu-id="dd4b2-117">带有提供程序生成/计算风险分数的云应用程序/服务。</span><span class="sxs-lookup"><span data-stu-id="dd4b2-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="dd4b2-118">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="dd4b2-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd4b2-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd4b2-119">JSON representation</span></span>

<span data-ttu-id="dd4b2-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd4b2-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
