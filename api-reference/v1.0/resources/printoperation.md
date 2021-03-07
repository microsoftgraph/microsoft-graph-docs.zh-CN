---
title: printOperation 资源类型
description: 代表长时间运行的通用打印操作。 操作类型（如 printerCreateOperation）的基类。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a397a0166ad62a503027499e9e0f5fd4f127b1e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517290"
---
# <a name="printoperation-resource-type"></a><span data-ttu-id="8c0fe-104">printOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c0fe-104">printOperation resource type</span></span>

<span data-ttu-id="8c0fe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c0fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8c0fe-106">代表长时间运行的通用打印操作。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-106">Represents a long-running Universal Print operation.</span></span> <span data-ttu-id="8c0fe-107">操作类型（如 [printerCreateOperation）的基类](printercreateoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-107">Base class for operation types such as [printerCreateOperation](printercreateoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8c0fe-108">Methods</span><span class="sxs-lookup"><span data-stu-id="8c0fe-108">Methods</span></span>
|<span data-ttu-id="8c0fe-109">方法</span><span class="sxs-lookup"><span data-stu-id="8c0fe-109">Method</span></span>|<span data-ttu-id="8c0fe-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c0fe-110">Return type</span></span>|<span data-ttu-id="8c0fe-111">Description</span><span class="sxs-lookup"><span data-stu-id="8c0fe-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="8c0fe-112">获取操作</span><span class="sxs-lookup"><span data-stu-id="8c0fe-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="8c0fe-113">printOperation</span><span class="sxs-lookup"><span data-stu-id="8c0fe-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="8c0fe-114">在当前用户或应用的租户中检索长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="8c0fe-115">属性</span><span class="sxs-lookup"><span data-stu-id="8c0fe-115">Properties</span></span>
|<span data-ttu-id="8c0fe-116">属性</span><span class="sxs-lookup"><span data-stu-id="8c0fe-116">Property</span></span>|<span data-ttu-id="8c0fe-117">类型</span><span class="sxs-lookup"><span data-stu-id="8c0fe-117">Type</span></span>|<span data-ttu-id="8c0fe-118">说明</span><span class="sxs-lookup"><span data-stu-id="8c0fe-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c0fe-119">id</span><span class="sxs-lookup"><span data-stu-id="8c0fe-119">id</span></span>|<span data-ttu-id="8c0fe-120">String</span><span class="sxs-lookup"><span data-stu-id="8c0fe-120">String</span></span>|<span data-ttu-id="8c0fe-121">操作标识符。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-121">The operation's identifier.</span></span> <span data-ttu-id="8c0fe-122">只读。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-122">Read-only.</span></span>|
|<span data-ttu-id="8c0fe-123">状态</span><span class="sxs-lookup"><span data-stu-id="8c0fe-123">status</span></span>|[<span data-ttu-id="8c0fe-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="8c0fe-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="8c0fe-125">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-125">The status of the operation.</span></span> <span data-ttu-id="8c0fe-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-126">Read-only.</span></span>|
|<span data-ttu-id="8c0fe-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c0fe-127">createdDateTime</span></span>|<span data-ttu-id="8c0fe-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c0fe-128">DateTimeOffset</span></span>|<span data-ttu-id="8c0fe-129">创建操作时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-129">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="8c0fe-130">只读。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c0fe-131">关系</span><span class="sxs-lookup"><span data-stu-id="8c0fe-131">Relationships</span></span>
<span data-ttu-id="8c0fe-132">无。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c0fe-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c0fe-133">JSON representation</span></span>
<span data-ttu-id="8c0fe-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c0fe-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

