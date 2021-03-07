---
title: printServiceEndpoint 资源类型
description: 表示打印服务实例的 URI 和标识信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0dd339d433be593e6982b6c38818635830a2d471
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516988"
---
# <a name="printserviceendpoint-resource-type"></a><span data-ttu-id="71f09-103">printServiceEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="71f09-103">printServiceEndpoint resource type</span></span>

<span data-ttu-id="71f09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="71f09-105">表示打印服务实例的 URI 和标识信息。</span><span class="sxs-lookup"><span data-stu-id="71f09-105">Represents URI and identifying information for a print service instance.</span></span>

## <a name="methods"></a><span data-ttu-id="71f09-106">Methods</span><span class="sxs-lookup"><span data-stu-id="71f09-106">Methods</span></span>
|<span data-ttu-id="71f09-107">方法</span><span class="sxs-lookup"><span data-stu-id="71f09-107">Method</span></span>|<span data-ttu-id="71f09-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="71f09-108">Return type</span></span>|<span data-ttu-id="71f09-109">Description</span><span class="sxs-lookup"><span data-stu-id="71f09-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="71f09-110">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="71f09-110">Get endpoint</span></span>](../api/printserviceendpoint-get.md) | [<span data-ttu-id="71f09-111">printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="71f09-111">printServiceEndpoint</span></span>](printserviceendpoint.md) | <span data-ttu-id="71f09-112">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71f09-112">Read the properties and relationships of endpoint object.</span></span> |

## <a name="properties"></a><span data-ttu-id="71f09-113">属性</span><span class="sxs-lookup"><span data-stu-id="71f09-113">Properties</span></span>
|<span data-ttu-id="71f09-114">属性</span><span class="sxs-lookup"><span data-stu-id="71f09-114">Property</span></span>|<span data-ttu-id="71f09-115">类型</span><span class="sxs-lookup"><span data-stu-id="71f09-115">Type</span></span>|<span data-ttu-id="71f09-116">说明</span><span class="sxs-lookup"><span data-stu-id="71f09-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f09-117">displayName</span><span class="sxs-lookup"><span data-stu-id="71f09-117">displayName</span></span>|<span data-ttu-id="71f09-118">String</span><span class="sxs-lookup"><span data-stu-id="71f09-118">String</span></span>|<span data-ttu-id="71f09-119">终结点的可读显示名称。</span><span class="sxs-lookup"><span data-stu-id="71f09-119">A human-readable display name for the endpoint.</span></span>|
|<span data-ttu-id="71f09-120">id</span><span class="sxs-lookup"><span data-stu-id="71f09-120">id</span></span>|<span data-ttu-id="71f09-121">String</span><span class="sxs-lookup"><span data-stu-id="71f09-121">String</span></span>|<span data-ttu-id="71f09-122">标识终结点提供的服务的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="71f09-122">A unique name that identifies the service that the endpoint provides.</span></span> <span data-ttu-id="71f09-123">可能的值包括 `discovery` ： (发现服务) 、 (通知服务 `notification`) 、 (IPP 服务) 和 `ipp` (`registration` 注册服务) 。</span><span class="sxs-lookup"><span data-stu-id="71f09-123">Possible values are: `discovery` (Discovery Service), `notification` (Notification Service), `ipp` (IPP Service), and `registration` (Registration Service).</span></span> <span data-ttu-id="71f09-124">只读。</span><span class="sxs-lookup"><span data-stu-id="71f09-124">Read-only.</span></span>|
|<span data-ttu-id="71f09-125">uri</span><span class="sxs-lookup"><span data-stu-id="71f09-125">uri</span></span>|<span data-ttu-id="71f09-126">String</span><span class="sxs-lookup"><span data-stu-id="71f09-126">String</span></span>|<span data-ttu-id="71f09-127">可用于访问服务的 URI。</span><span class="sxs-lookup"><span data-stu-id="71f09-127">The URI that can be used to access the service.</span></span>|


## <a name="relationships"></a><span data-ttu-id="71f09-128">关系</span><span class="sxs-lookup"><span data-stu-id="71f09-128">Relationships</span></span>
<span data-ttu-id="71f09-129">无。</span><span class="sxs-lookup"><span data-stu-id="71f09-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71f09-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71f09-130">JSON representation</span></span>
<span data-ttu-id="71f09-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f09-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```

