---
title: cloudAppSecurityState 资源类型
description: 包含有关云应用程序 (destinationServiceName、destinationServiceIp) 的状态信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e000d5d788a293c9aed7b702da2653f42116c0c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029713"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="25eb8-103">cloudAppSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="25eb8-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="25eb8-104">包含有关云应用程序 (destinationServiceName、destinationServiceIp) 的状态信息。</span><span class="sxs-lookup"><span data-stu-id="25eb8-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="25eb8-105">属性</span><span class="sxs-lookup"><span data-stu-id="25eb8-105">Properties</span></span>

| <span data-ttu-id="25eb8-106">属性</span><span class="sxs-lookup"><span data-stu-id="25eb8-106">Property</span></span>     | <span data-ttu-id="25eb8-107">类型</span><span class="sxs-lookup"><span data-stu-id="25eb8-107">Type</span></span>        | <span data-ttu-id="25eb8-108">说明</span><span class="sxs-lookup"><span data-stu-id="25eb8-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25eb8-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="25eb8-109">destinationServiceIp</span></span>|<span data-ttu-id="25eb8-110">String</span><span class="sxs-lookup"><span data-stu-id="25eb8-110">String</span></span>|<span data-ttu-id="25eb8-111">指向云应用程序/服务的连接的目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="25eb8-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="25eb8-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="25eb8-112">destinationServiceName</span></span>|<span data-ttu-id="25eb8-113">String</span><span class="sxs-lookup"><span data-stu-id="25eb8-113">String</span></span>|<span data-ttu-id="25eb8-114">云应用程序/服务名称 (例如, "Salesforce"、"DropBox" 等)。</span><span class="sxs-lookup"><span data-stu-id="25eb8-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="25eb8-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="25eb8-115">riskScore</span></span>|<span data-ttu-id="25eb8-116">String</span><span class="sxs-lookup"><span data-stu-id="25eb8-116">String</span></span>|<span data-ttu-id="25eb8-117">提供程序生成/计算的风险分数 (云应用程序/服务)。</span><span class="sxs-lookup"><span data-stu-id="25eb8-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="25eb8-118">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="25eb8-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25eb8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25eb8-119">JSON representation</span></span>

<span data-ttu-id="25eb8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25eb8-120">The following is a JSON representation of the resource.</span></span>

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
