---
title: printService 资源类型
description: 表示对打印服务实例的特定于 Azure AD 租户的说明。 打印基础结构的每个组件都有服务 (例如，发现、通知、注册和 IPP) 并具有一个或多个终结点。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 00ba50369f2396250df632c13ed3945e8c9d40d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052537"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="db3c4-104">printService 资源类型</span><span class="sxs-lookup"><span data-stu-id="db3c4-104">printService resource type</span></span>

<span data-ttu-id="db3c4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db3c4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db3c4-106">表示对打印服务实例的特定于 Azure AD 租户的说明。</span><span class="sxs-lookup"><span data-stu-id="db3c4-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="db3c4-107">打印基础结构的每个组件都存在的服务 (发现、通知、注册和 IPP) 并具有一个或多个终结点。</span><span class="sxs-lookup"><span data-stu-id="db3c4-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="db3c4-108">方法</span><span class="sxs-lookup"><span data-stu-id="db3c4-108">Methods</span></span>

| <span data-ttu-id="db3c4-109">方法</span><span class="sxs-lookup"><span data-stu-id="db3c4-109">Method</span></span>       | <span data-ttu-id="db3c4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="db3c4-110">Return Type</span></span> | <span data-ttu-id="db3c4-111">说明</span><span class="sxs-lookup"><span data-stu-id="db3c4-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="db3c4-112">列出服务</span><span class="sxs-lookup"><span data-stu-id="db3c4-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="db3c4-113">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db3c4-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="db3c4-114">获取通用打印服务的列表。</span><span class="sxs-lookup"><span data-stu-id="db3c4-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="db3c4-115">获取服务</span><span class="sxs-lookup"><span data-stu-id="db3c4-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="db3c4-116">printService</span><span class="sxs-lookup"><span data-stu-id="db3c4-116">printService</span></span>](printservice.md) | <span data-ttu-id="db3c4-117">读取服务对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db3c4-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="db3c4-118">List endpoints</span><span class="sxs-lookup"><span data-stu-id="db3c4-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="db3c4-119">[printServiceEndpoint](printserviceendpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db3c4-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="db3c4-120">获取服务提供的终结点列表。</span><span class="sxs-lookup"><span data-stu-id="db3c4-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="db3c4-121">属性</span><span class="sxs-lookup"><span data-stu-id="db3c4-121">Properties</span></span>
| <span data-ttu-id="db3c4-122">属性</span><span class="sxs-lookup"><span data-stu-id="db3c4-122">Property</span></span>     | <span data-ttu-id="db3c4-123">类型</span><span class="sxs-lookup"><span data-stu-id="db3c4-123">Type</span></span>        | <span data-ttu-id="db3c4-124">说明</span><span class="sxs-lookup"><span data-stu-id="db3c4-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="db3c4-125">id</span><span class="sxs-lookup"><span data-stu-id="db3c4-125">id</span></span>|<span data-ttu-id="db3c4-126">String</span><span class="sxs-lookup"><span data-stu-id="db3c4-126">String</span></span>|<span data-ttu-id="db3c4-127">服务的标识符。</span><span class="sxs-lookup"><span data-stu-id="db3c4-127">The service's identifier.</span></span> <span data-ttu-id="db3c4-128">只读。</span><span class="sxs-lookup"><span data-stu-id="db3c4-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db3c4-129">关系</span><span class="sxs-lookup"><span data-stu-id="db3c4-129">Relationships</span></span>
| <span data-ttu-id="db3c4-130">关系</span><span class="sxs-lookup"><span data-stu-id="db3c4-130">Relationship</span></span> | <span data-ttu-id="db3c4-131">类型</span><span class="sxs-lookup"><span data-stu-id="db3c4-131">Type</span></span>        | <span data-ttu-id="db3c4-132">说明</span><span class="sxs-lookup"><span data-stu-id="db3c4-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="db3c4-133">endpoints</span><span class="sxs-lookup"><span data-stu-id="db3c4-133">endpoints</span></span>|<span data-ttu-id="db3c4-134">[printServiceEndpoint](printserviceendpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db3c4-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="db3c4-135">可用于访问服务的终结点。</span><span class="sxs-lookup"><span data-stu-id="db3c4-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="db3c4-136">只读。</span><span class="sxs-lookup"><span data-stu-id="db3c4-136">Read-only.</span></span> <span data-ttu-id="db3c4-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="db3c4-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db3c4-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db3c4-138">JSON representation</span></span>

<span data-ttu-id="db3c4-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db3c4-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printService",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "endpoints": [ {"@odata.type": "microsoft.graph.printServiceEndpoint"} ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

