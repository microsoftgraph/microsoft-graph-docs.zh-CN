---
title: printerCreateOperation 资源类型
description: 代表长时间运行的打印机注册操作。 派生自 printOperation。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 31d872ba84df3fcdd4f246cbd32b3668d21e57d5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516950"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="af2ee-104">printerCreateOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="af2ee-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="af2ee-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af2ee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="af2ee-106">代表长时间运行的打印机注册操作。</span><span class="sxs-lookup"><span data-stu-id="af2ee-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="af2ee-107">派生自 [printOperation](printoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="af2ee-107">Derived from [printOperation](printoperation.md).</span></span>

<span data-ttu-id="af2ee-108">继承自 [printOperation](printoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="af2ee-108">Inherits from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="af2ee-109">Methods</span><span class="sxs-lookup"><span data-stu-id="af2ee-109">Methods</span></span>
|<span data-ttu-id="af2ee-110">方法</span><span class="sxs-lookup"><span data-stu-id="af2ee-110">Method</span></span>|<span data-ttu-id="af2ee-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="af2ee-111">Return type</span></span>|<span data-ttu-id="af2ee-112">Description</span><span class="sxs-lookup"><span data-stu-id="af2ee-112">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="af2ee-113">获取操作</span><span class="sxs-lookup"><span data-stu-id="af2ee-113">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="af2ee-114">printOperation</span><span class="sxs-lookup"><span data-stu-id="af2ee-114">printOperation</span></span>](printoperation.md) | <span data-ttu-id="af2ee-115">在当前用户或应用的租户中检索长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="af2ee-115">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="af2ee-116">属性</span><span class="sxs-lookup"><span data-stu-id="af2ee-116">Properties</span></span>
|<span data-ttu-id="af2ee-117">属性</span><span class="sxs-lookup"><span data-stu-id="af2ee-117">Property</span></span>|<span data-ttu-id="af2ee-118">类型</span><span class="sxs-lookup"><span data-stu-id="af2ee-118">Type</span></span>|<span data-ttu-id="af2ee-119">说明</span><span class="sxs-lookup"><span data-stu-id="af2ee-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2ee-120">id</span><span class="sxs-lookup"><span data-stu-id="af2ee-120">id</span></span>|<span data-ttu-id="af2ee-121">String</span><span class="sxs-lookup"><span data-stu-id="af2ee-121">String</span></span>|<span data-ttu-id="af2ee-122">操作标识符。</span><span class="sxs-lookup"><span data-stu-id="af2ee-122">The operation's identifier.</span></span> <span data-ttu-id="af2ee-123">只读。</span><span class="sxs-lookup"><span data-stu-id="af2ee-123">Read-only.</span></span>|
|<span data-ttu-id="af2ee-124">状态</span><span class="sxs-lookup"><span data-stu-id="af2ee-124">status</span></span>|[<span data-ttu-id="af2ee-125">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="af2ee-125">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="af2ee-126">注册操作的状态。</span><span class="sxs-lookup"><span data-stu-id="af2ee-126">The status of the registration operation.</span></span> <span data-ttu-id="af2ee-127">包含操作的进度以及操作是否成功完成。</span><span class="sxs-lookup"><span data-stu-id="af2ee-127">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="af2ee-128">只读。</span><span class="sxs-lookup"><span data-stu-id="af2ee-128">Read-only.</span></span>|
|<span data-ttu-id="af2ee-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af2ee-129">createdDateTime</span></span>|<span data-ttu-id="af2ee-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2ee-130">DateTimeOffset</span></span>|<span data-ttu-id="af2ee-131">创建操作时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="af2ee-131">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="af2ee-132">只读。</span><span class="sxs-lookup"><span data-stu-id="af2ee-132">Read-only.</span></span>|
|<span data-ttu-id="af2ee-133">证书</span><span class="sxs-lookup"><span data-stu-id="af2ee-133">certificate</span></span>|<span data-ttu-id="af2ee-134">String</span><span class="sxs-lookup"><span data-stu-id="af2ee-134">String</span></span>|<span data-ttu-id="af2ee-135">注册过程中创建的已签名证书。</span><span class="sxs-lookup"><span data-stu-id="af2ee-135">The signed certificate created during the registration process.</span></span> <span data-ttu-id="af2ee-136">只读。</span><span class="sxs-lookup"><span data-stu-id="af2ee-136">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af2ee-137">关系</span><span class="sxs-lookup"><span data-stu-id="af2ee-137">Relationships</span></span>
|<span data-ttu-id="af2ee-138">关系</span><span class="sxs-lookup"><span data-stu-id="af2ee-138">Relationship</span></span>|<span data-ttu-id="af2ee-139">类型</span><span class="sxs-lookup"><span data-stu-id="af2ee-139">Type</span></span>|<span data-ttu-id="af2ee-140">Description</span><span class="sxs-lookup"><span data-stu-id="af2ee-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2ee-141">打印机</span><span class="sxs-lookup"><span data-stu-id="af2ee-141">printer</span></span>|[<span data-ttu-id="af2ee-142">打印机</span><span class="sxs-lookup"><span data-stu-id="af2ee-142">printer</span></span>](printer.md)|<span data-ttu-id="af2ee-143">创建的打印机实体。</span><span class="sxs-lookup"><span data-stu-id="af2ee-143">The created printer entity.</span></span> <span data-ttu-id="af2ee-144">只读。</span><span class="sxs-lookup"><span data-stu-id="af2ee-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af2ee-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af2ee-145">JSON representation</span></span>
<span data-ttu-id="af2ee-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af2ee-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "baseType": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCreateOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)",
  "certificate": "String"
}
```

