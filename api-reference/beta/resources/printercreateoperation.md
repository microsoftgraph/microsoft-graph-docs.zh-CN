---
title: printerCreateOperation 资源类型
description: 表示长时间运行的打印机注册操作。 派生自 printOperation。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 54f458e14cbda209d9c2d85f08df4c106db6ab00
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007188"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="42599-104">printerCreateOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="42599-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="42599-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42599-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42599-106">表示长时间运行的打印机注册操作。</span><span class="sxs-lookup"><span data-stu-id="42599-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="42599-107">派生自[printOperation](printoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="42599-107">Derived from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="42599-108">方法</span><span class="sxs-lookup"><span data-stu-id="42599-108">Methods</span></span>

| <span data-ttu-id="42599-109">方法</span><span class="sxs-lookup"><span data-stu-id="42599-109">Method</span></span>       | <span data-ttu-id="42599-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="42599-110">Return Type</span></span> | <span data-ttu-id="42599-111">说明</span><span class="sxs-lookup"><span data-stu-id="42599-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="42599-112">Get 操作</span><span class="sxs-lookup"><span data-stu-id="42599-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="42599-113">printOperation</span><span class="sxs-lookup"><span data-stu-id="42599-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="42599-114">在当前用户或应用程序的租户内检索长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="42599-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="42599-115">属性</span><span class="sxs-lookup"><span data-stu-id="42599-115">Properties</span></span>
| <span data-ttu-id="42599-116">属性</span><span class="sxs-lookup"><span data-stu-id="42599-116">Property</span></span>     | <span data-ttu-id="42599-117">类型</span><span class="sxs-lookup"><span data-stu-id="42599-117">Type</span></span>        | <span data-ttu-id="42599-118">说明</span><span class="sxs-lookup"><span data-stu-id="42599-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42599-119">id</span><span class="sxs-lookup"><span data-stu-id="42599-119">id</span></span>|<span data-ttu-id="42599-120">String</span><span class="sxs-lookup"><span data-stu-id="42599-120">String</span></span>|<span data-ttu-id="42599-121">操作的标识符。</span><span class="sxs-lookup"><span data-stu-id="42599-121">The operation's identifier.</span></span> <span data-ttu-id="42599-122">只读。</span><span class="sxs-lookup"><span data-stu-id="42599-122">Read-only.</span></span>|
|<span data-ttu-id="42599-123">status</span><span class="sxs-lookup"><span data-stu-id="42599-123">status</span></span>|[<span data-ttu-id="42599-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="42599-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="42599-125">注册操作的状态。</span><span class="sxs-lookup"><span data-stu-id="42599-125">The status of the registration operation.</span></span> <span data-ttu-id="42599-126">包含操作的进度以及它是否成功完成。</span><span class="sxs-lookup"><span data-stu-id="42599-126">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="42599-127">只读。</span><span class="sxs-lookup"><span data-stu-id="42599-127">Read-only.</span></span>|
|<span data-ttu-id="42599-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42599-128">createdDateTime</span></span>|<span data-ttu-id="42599-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42599-129">DateTimeOffset</span></span>|<span data-ttu-id="42599-130">创建操作时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="42599-130">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="42599-131">只读。</span><span class="sxs-lookup"><span data-stu-id="42599-131">Read-only.</span></span>|
|<span data-ttu-id="42599-132">证书</span><span class="sxs-lookup"><span data-stu-id="42599-132">certificate</span></span>|<span data-ttu-id="42599-133">String</span><span class="sxs-lookup"><span data-stu-id="42599-133">String</span></span>|<span data-ttu-id="42599-134">注册过程中创建的签名证书。</span><span class="sxs-lookup"><span data-stu-id="42599-134">The signed certificate created during the registration process.</span></span> <span data-ttu-id="42599-135">只读。</span><span class="sxs-lookup"><span data-stu-id="42599-135">Read-only.</span></span>|
|<span data-ttu-id="42599-136">印刷</span><span class="sxs-lookup"><span data-stu-id="42599-136">printer</span></span>|[<span data-ttu-id="42599-137">印刷</span><span class="sxs-lookup"><span data-stu-id="42599-137">printer</span></span>](printer.md)|<span data-ttu-id="42599-138">创建的打印机实体。</span><span class="sxs-lookup"><span data-stu-id="42599-138">The created printer entity.</span></span> <span data-ttu-id="42599-139">只读。</span><span class="sxs-lookup"><span data-stu-id="42599-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42599-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42599-140">JSON representation</span></span>

<span data-ttu-id="42599-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42599-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->