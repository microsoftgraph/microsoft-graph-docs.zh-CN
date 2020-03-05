---
title: cloudAppSecurityState 资源类型
description: 包含有关云应用程序（destinationServiceName、destinationServiceIp）的状态信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e2df4dd25f4209996b4e5cf4f2083790385e84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507640"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="cfe4f-103">cloudAppSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfe4f-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="cfe4f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cfe4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfe4f-105">包含有关云应用程序（destinationServiceName、destinationServiceIp）的状态信息。</span><span class="sxs-lookup"><span data-stu-id="cfe4f-105">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="cfe4f-106">属性</span><span class="sxs-lookup"><span data-stu-id="cfe4f-106">Properties</span></span>

| <span data-ttu-id="cfe4f-107">属性</span><span class="sxs-lookup"><span data-stu-id="cfe4f-107">Property</span></span>     | <span data-ttu-id="cfe4f-108">类型</span><span class="sxs-lookup"><span data-stu-id="cfe4f-108">Type</span></span>        | <span data-ttu-id="cfe4f-109">说明</span><span class="sxs-lookup"><span data-stu-id="cfe4f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cfe4f-110">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="cfe4f-110">destinationServiceIp</span></span>|<span data-ttu-id="cfe4f-111">String</span><span class="sxs-lookup"><span data-stu-id="cfe4f-111">String</span></span>|<span data-ttu-id="cfe4f-112">指向云应用程序/服务的连接的目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="cfe4f-112">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="cfe4f-113">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="cfe4f-113">destinationServiceName</span></span>|<span data-ttu-id="cfe4f-114">String</span><span class="sxs-lookup"><span data-stu-id="cfe4f-114">String</span></span>|<span data-ttu-id="cfe4f-115">云应用程序/服务名称（例如，"Salesforce"、"DropBox" 等）。</span><span class="sxs-lookup"><span data-stu-id="cfe4f-115">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="cfe4f-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="cfe4f-116">riskScore</span></span>|<span data-ttu-id="cfe4f-117">String</span><span class="sxs-lookup"><span data-stu-id="cfe4f-117">String</span></span>|<span data-ttu-id="cfe4f-118">提供程序生成/计算的风险分数（云应用程序/服务）。</span><span class="sxs-lookup"><span data-stu-id="cfe4f-118">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="cfe4f-119">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="cfe4f-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfe4f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfe4f-120">JSON representation</span></span>

<span data-ttu-id="cfe4f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfe4f-121">The following is a JSON representation of the resource.</span></span>

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
