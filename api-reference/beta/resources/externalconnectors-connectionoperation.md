---
title: connectionOperation 资源类型
description: 描述创建连接架构的异步请求Microsoft 搜索状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1b9e3bf811807213970694ebe4e7748bf59e32ef
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467644"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="9d20d-103">connectionOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d20d-103">connectionOperation resource type</span></span>

<span data-ttu-id="9d20d-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="9d20d-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d20d-105">描述创建连接架构的异步Microsoft 搜索[状态](externalconnectors-schema.md)。</span><span class="sxs-lookup"><span data-stu-id="9d20d-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](externalconnectors-schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9d20d-106">方法</span><span class="sxs-lookup"><span data-stu-id="9d20d-106">Methods</span></span>

| <span data-ttu-id="9d20d-107">方法</span><span class="sxs-lookup"><span data-stu-id="9d20d-107">Method</span></span>       | <span data-ttu-id="9d20d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d20d-108">Return Type</span></span> | <span data-ttu-id="9d20d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d20d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9d20d-110">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="9d20d-110">Get connectionOperation</span></span>](../api/externalconnectors-connectionoperation-get.md) | [<span data-ttu-id="9d20d-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="9d20d-111">connectionOperation</span></span>](externalconnectors-connectionoperation.md) | <span data-ttu-id="9d20d-112">读取 connectionOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d20d-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d20d-113">属性</span><span class="sxs-lookup"><span data-stu-id="9d20d-113">Properties</span></span>

| <span data-ttu-id="9d20d-114">属性</span><span class="sxs-lookup"><span data-stu-id="9d20d-114">Property</span></span> | <span data-ttu-id="9d20d-115">类型</span><span class="sxs-lookup"><span data-stu-id="9d20d-115">Type</span></span>                          | <span data-ttu-id="9d20d-116">说明</span><span class="sxs-lookup"><span data-stu-id="9d20d-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="9d20d-117">error</span><span class="sxs-lookup"><span data-stu-id="9d20d-117">error</span></span>    | [<span data-ttu-id="9d20d-118">publicError</span><span class="sxs-lookup"><span data-stu-id="9d20d-118">publicError</span></span>](publicerror.md) | <span data-ttu-id="9d20d-119">如果 `status` 为 `failed` ，则提供有关导致失败的错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9d20d-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="9d20d-120">id</span><span class="sxs-lookup"><span data-stu-id="9d20d-120">id</span></span>       | <span data-ttu-id="9d20d-121">String</span><span class="sxs-lookup"><span data-stu-id="9d20d-121">String</span></span>                        | <span data-ttu-id="9d20d-122">connectionOperation 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9d20d-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="9d20d-123">只读。</span><span class="sxs-lookup"><span data-stu-id="9d20d-123">Read-only.</span></span> |
| <span data-ttu-id="9d20d-124">状态</span><span class="sxs-lookup"><span data-stu-id="9d20d-124">status</span></span>   | <span data-ttu-id="9d20d-125">String</span><span class="sxs-lookup"><span data-stu-id="9d20d-125">String</span></span>                        | <span data-ttu-id="9d20d-126">指示异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9d20d-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="9d20d-127">可取值为：`unspecified`、`inprogress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="9d20d-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d20d-128">关系</span><span class="sxs-lookup"><span data-stu-id="9d20d-128">Relationships</span></span>

<span data-ttu-id="9d20d-129">无</span><span class="sxs-lookup"><span data-stu-id="9d20d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d20d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d20d-130">JSON representation</span></span>

<span data-ttu-id="9d20d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d20d-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
