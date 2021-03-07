---
title: printService 资源类型
description: 表示打印服务实例的 Azure AD 租户特定说明。 打印基础结构的每个组件都有服务 (例如发现、通知、注册和 IPP) 具有一个或多个终结点。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 986749028a75f98157ff73138396a4ad56672fc8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516989"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="f5b73-104">printService 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5b73-104">printService resource type</span></span>

<span data-ttu-id="f5b73-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b73-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f5b73-106">表示打印服务实例的 Azure AD 租户特定说明。</span><span class="sxs-lookup"><span data-stu-id="f5b73-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="f5b73-107">打印基础结构的每个组件都有服务 (发现、通知、注册和 IPP) 具有一个或多个终结点。</span><span class="sxs-lookup"><span data-stu-id="f5b73-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="f5b73-108">Methods</span><span class="sxs-lookup"><span data-stu-id="f5b73-108">Methods</span></span>
|<span data-ttu-id="f5b73-109">方法</span><span class="sxs-lookup"><span data-stu-id="f5b73-109">Method</span></span>|<span data-ttu-id="f5b73-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5b73-110">Return type</span></span>|<span data-ttu-id="f5b73-111">Description</span><span class="sxs-lookup"><span data-stu-id="f5b73-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="f5b73-112">列出服务</span><span class="sxs-lookup"><span data-stu-id="f5b73-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="f5b73-113">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5b73-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="f5b73-114">获取通用打印服务的列表。</span><span class="sxs-lookup"><span data-stu-id="f5b73-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="f5b73-115">获取服务</span><span class="sxs-lookup"><span data-stu-id="f5b73-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="f5b73-116">printService</span><span class="sxs-lookup"><span data-stu-id="f5b73-116">printService</span></span>](printservice.md) | <span data-ttu-id="f5b73-117">读取服务对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f5b73-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="f5b73-118">List endpoints</span><span class="sxs-lookup"><span data-stu-id="f5b73-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="f5b73-119">[printServiceEndpoint](printserviceendpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5b73-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="f5b73-120">获取服务提供的终结点列表。</span><span class="sxs-lookup"><span data-stu-id="f5b73-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="f5b73-121">属性</span><span class="sxs-lookup"><span data-stu-id="f5b73-121">Properties</span></span>
|<span data-ttu-id="f5b73-122">属性</span><span class="sxs-lookup"><span data-stu-id="f5b73-122">Property</span></span>|<span data-ttu-id="f5b73-123">类型</span><span class="sxs-lookup"><span data-stu-id="f5b73-123">Type</span></span>|<span data-ttu-id="f5b73-124">说明</span><span class="sxs-lookup"><span data-stu-id="f5b73-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5b73-125">id</span><span class="sxs-lookup"><span data-stu-id="f5b73-125">id</span></span>|<span data-ttu-id="f5b73-126">String</span><span class="sxs-lookup"><span data-stu-id="f5b73-126">String</span></span>|<span data-ttu-id="f5b73-127">服务的标识符。</span><span class="sxs-lookup"><span data-stu-id="f5b73-127">The service's identifier.</span></span> <span data-ttu-id="f5b73-128">只读。</span><span class="sxs-lookup"><span data-stu-id="f5b73-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5b73-129">关系</span><span class="sxs-lookup"><span data-stu-id="f5b73-129">Relationships</span></span>
|<span data-ttu-id="f5b73-130">关系</span><span class="sxs-lookup"><span data-stu-id="f5b73-130">Relationship</span></span>|<span data-ttu-id="f5b73-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5b73-131">Type</span></span>|<span data-ttu-id="f5b73-132">Description</span><span class="sxs-lookup"><span data-stu-id="f5b73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5b73-133">endpoints</span><span class="sxs-lookup"><span data-stu-id="f5b73-133">endpoints</span></span>|<span data-ttu-id="f5b73-134">[printServiceEndpoint](printserviceendpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5b73-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="f5b73-135">可用于访问服务的终结点。</span><span class="sxs-lookup"><span data-stu-id="f5b73-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="f5b73-136">只读。</span><span class="sxs-lookup"><span data-stu-id="f5b73-136">Read-only.</span></span> <span data-ttu-id="f5b73-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f5b73-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5b73-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5b73-138">JSON representation</span></span>
<span data-ttu-id="f5b73-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5b73-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

