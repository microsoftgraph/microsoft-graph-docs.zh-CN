---
title: printerShare 资源类型
description: 表示可供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a44cac259e9be653ca0e7b21c81b6c72224268b1
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895608"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="66285-103">printerShare 资源类型</span><span class="sxs-lookup"><span data-stu-id="66285-103">printerShare resource type</span></span>

<span data-ttu-id="66285-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66285-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66285-105">表示可供用户和打印应用程序发现的打印机。</span><span class="sxs-lookup"><span data-stu-id="66285-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="66285-106">方法</span><span class="sxs-lookup"><span data-stu-id="66285-106">Methods</span></span>

| <span data-ttu-id="66285-107">方法</span><span class="sxs-lookup"><span data-stu-id="66285-107">Method</span></span>       | <span data-ttu-id="66285-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="66285-108">Return Type</span></span> | <span data-ttu-id="66285-109">说明</span><span class="sxs-lookup"><span data-stu-id="66285-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66285-110">列出 printerShares</span><span class="sxs-lookup"><span data-stu-id="66285-110">List printerShares</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="66285-111">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="66285-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="66285-112">获取租户中的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="66285-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="66285-113">获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="66285-113">Get printerShare</span></span>](../api/printershare-get.md) | [<span data-ttu-id="66285-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="66285-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="66285-115">读取 printerShare 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66285-115">Read properties and relationships of a printerShare object.</span></span> |
| [<span data-ttu-id="66285-116">更新</span><span class="sxs-lookup"><span data-stu-id="66285-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="66285-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="66285-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="66285-118">更新 printerShare 对象。</span><span class="sxs-lookup"><span data-stu-id="66285-118">Update a printerShare object.</span></span> |
| [<span data-ttu-id="66285-119">删除</span><span class="sxs-lookup"><span data-stu-id="66285-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="66285-120">无</span><span class="sxs-lookup"><span data-stu-id="66285-120">None</span></span> | <span data-ttu-id="66285-121">取消打印机的共享。</span><span class="sxs-lookup"><span data-stu-id="66285-121">Unshare a printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="66285-122">属性</span><span class="sxs-lookup"><span data-stu-id="66285-122">Properties</span></span>
| <span data-ttu-id="66285-123">属性</span><span class="sxs-lookup"><span data-stu-id="66285-123">Property</span></span>     | <span data-ttu-id="66285-124">类型</span><span class="sxs-lookup"><span data-stu-id="66285-124">Type</span></span>        | <span data-ttu-id="66285-125">说明</span><span class="sxs-lookup"><span data-stu-id="66285-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66285-126">id</span><span class="sxs-lookup"><span data-stu-id="66285-126">id</span></span>|<span data-ttu-id="66285-127">String</span><span class="sxs-lookup"><span data-stu-id="66285-127">String</span></span>| <span data-ttu-id="66285-128">PrinterShare 的标识符。</span><span class="sxs-lookup"><span data-stu-id="66285-128">The printerShare's identifier.</span></span> <span data-ttu-id="66285-129">只读。</span><span class="sxs-lookup"><span data-stu-id="66285-129">Read-only.</span></span>|
|<span data-ttu-id="66285-130">name</span><span class="sxs-lookup"><span data-stu-id="66285-130">name</span></span>|<span data-ttu-id="66285-131">String</span><span class="sxs-lookup"><span data-stu-id="66285-131">String</span></span>|<span data-ttu-id="66285-132">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="66285-132">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="66285-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66285-133">createdDateTime</span></span>|<span data-ttu-id="66285-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66285-134">DateTimeOffset</span></span>|<span data-ttu-id="66285-135">创建打印机共享时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="66285-135">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="66285-136">只读。</span><span class="sxs-lookup"><span data-stu-id="66285-136">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66285-137">关系</span><span class="sxs-lookup"><span data-stu-id="66285-137">Relationships</span></span>
| <span data-ttu-id="66285-138">关系</span><span class="sxs-lookup"><span data-stu-id="66285-138">Relationship</span></span> | <span data-ttu-id="66285-139">类型</span><span class="sxs-lookup"><span data-stu-id="66285-139">Type</span></span>        | <span data-ttu-id="66285-140">说明</span><span class="sxs-lookup"><span data-stu-id="66285-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66285-141">印刷</span><span class="sxs-lookup"><span data-stu-id="66285-141">printer</span></span>|[<span data-ttu-id="66285-142">印刷</span><span class="sxs-lookup"><span data-stu-id="66285-142">printer</span></span>](printer.md)|<span data-ttu-id="66285-143">与此打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="66285-143">The printer that this printer share is related to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66285-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66285-144">JSON representation</span></span>

<span data-ttu-id="66285-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66285-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->