---
title: printServiceEndpoint 资源类型
description: 表示打印服务实例的 URI 和标识信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8b9289807778c1a44940d8e8eb0d9163ed12f006
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985858"
---
# <a name="printserviceendpoint-resource-type"></a><span data-ttu-id="49d42-103">printServiceEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="49d42-103">printServiceEndpoint resource type</span></span>

<span data-ttu-id="49d42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49d42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49d42-105">表示打印服务实例的 URI 和标识信息。</span><span class="sxs-lookup"><span data-stu-id="49d42-105">Represents URI and identifying information for a print service instance.</span></span>

## <a name="methods"></a><span data-ttu-id="49d42-106">方法</span><span class="sxs-lookup"><span data-stu-id="49d42-106">Methods</span></span>

| <span data-ttu-id="49d42-107">方法</span><span class="sxs-lookup"><span data-stu-id="49d42-107">Method</span></span>       | <span data-ttu-id="49d42-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="49d42-108">Return Type</span></span> | <span data-ttu-id="49d42-109">说明</span><span class="sxs-lookup"><span data-stu-id="49d42-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="49d42-110">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="49d42-110">Get endpoint</span></span>](../api/printserviceendpoint-get.md) | [<span data-ttu-id="49d42-111">printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="49d42-111">printServiceEndpoint</span></span>](printserviceendpoint.md) | <span data-ttu-id="49d42-112">读取终结点对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49d42-112">Read the properties and relationships of endpoint object.</span></span> |

## <a name="properties"></a><span data-ttu-id="49d42-113">属性</span><span class="sxs-lookup"><span data-stu-id="49d42-113">Properties</span></span>
| <span data-ttu-id="49d42-114">属性</span><span class="sxs-lookup"><span data-stu-id="49d42-114">Property</span></span>     | <span data-ttu-id="49d42-115">类型</span><span class="sxs-lookup"><span data-stu-id="49d42-115">Type</span></span>        | <span data-ttu-id="49d42-116">说明</span><span class="sxs-lookup"><span data-stu-id="49d42-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="49d42-117">displayName</span><span class="sxs-lookup"><span data-stu-id="49d42-117">displayName</span></span>|<span data-ttu-id="49d42-118">String</span><span class="sxs-lookup"><span data-stu-id="49d42-118">String</span></span>|<span data-ttu-id="49d42-119">终结点的人可读显示名称。</span><span class="sxs-lookup"><span data-stu-id="49d42-119">A human-readable display name for the endpoint.</span></span>|
|<span data-ttu-id="49d42-120">name</span><span class="sxs-lookup"><span data-stu-id="49d42-120">name</span></span>|<span data-ttu-id="49d42-121">String</span><span class="sxs-lookup"><span data-stu-id="49d42-121">String</span></span>|<span data-ttu-id="49d42-122">标识终结点提供的服务的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="49d42-122">A unique name that identifies the service that the endpoint provides.</span></span> <span data-ttu-id="49d42-123">可能的值包括： `discovery` (发现服务) 、 `notification` (通知服务) 、 `ipp` (IPP 服务) 和 `registration` (注册服务) 。</span><span class="sxs-lookup"><span data-stu-id="49d42-123">Possible values are: `discovery` (Discovery Service), `notification` (Notification Service), `ipp` (IPP Service), and `registration` (Registration Service).</span></span> <span data-ttu-id="49d42-124">只读。</span><span class="sxs-lookup"><span data-stu-id="49d42-124">Read-only.</span></span>|
|<span data-ttu-id="49d42-125">url</span><span class="sxs-lookup"><span data-stu-id="49d42-125">uri</span></span>|<span data-ttu-id="49d42-126">String</span><span class="sxs-lookup"><span data-stu-id="49d42-126">String</span></span>|<span data-ttu-id="49d42-127">可用于访问服务的 URI。</span><span class="sxs-lookup"><span data-stu-id="49d42-127">The URI that can be used to access the service.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49d42-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49d42-128">JSON representation</span></span>

<span data-ttu-id="49d42-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49d42-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}-->

```json
{
  "displayName": "String",
  "name": "String (identifier)",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printServiceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

