---
title: cloudAppSecurityState 资源类型
description: 包含状态信息的云应用程序 （destinationServiceName、 destinationServiceIp）。
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045900"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="c58a0-103">cloudAppSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c58a0-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="c58a0-104">包含状态信息的云应用程序 （destinationServiceName、 destinationServiceIp）。</span><span class="sxs-lookup"><span data-stu-id="c58a0-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="c58a0-105">属性</span><span class="sxs-lookup"><span data-stu-id="c58a0-105">Properties</span></span>

| <span data-ttu-id="c58a0-106">属性</span><span class="sxs-lookup"><span data-stu-id="c58a0-106">Property</span></span>     | <span data-ttu-id="c58a0-107">类型</span><span class="sxs-lookup"><span data-stu-id="c58a0-107">Type</span></span>        | <span data-ttu-id="c58a0-108">说明</span><span class="sxs-lookup"><span data-stu-id="c58a0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c58a0-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="c58a0-109">destinationServiceIp</span></span>|<span data-ttu-id="c58a0-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c58a0-110">String</span></span>|<span data-ttu-id="c58a0-111">连接到云应用程序/服务的目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c58a0-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="c58a0-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="c58a0-112">destinationServiceName</span></span>|<span data-ttu-id="c58a0-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c58a0-113">String</span></span>|<span data-ttu-id="c58a0-114">云应用程序/服务名称 （例如"销售"、"收存箱"等）。</span><span class="sxs-lookup"><span data-stu-id="c58a0-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="c58a0-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="c58a0-115">riskScore</span></span>|<span data-ttu-id="c58a0-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c58a0-116">String</span></span>|<span data-ttu-id="c58a0-117">带有提供程序生成/计算风险分数的云应用程序/服务。</span><span class="sxs-lookup"><span data-stu-id="c58a0-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="c58a0-118">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="c58a0-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c58a0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c58a0-119">JSON representation</span></span>

<span data-ttu-id="c58a0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c58a0-120">The following is a JSON representation of the resource.</span></span>

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