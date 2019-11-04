---
title: connectionOperation 资源类型
description: 描述用于创建 Microsoft Search 连接架构的异步请求的状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 657d71dc6b1671b2af6011778c0b14bb299e3cf9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938882"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="58b7c-103">connectionOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="58b7c-103">connectionOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58b7c-104">描述用于创建 Microsoft Search 连接[架构](schema.md)的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="58b7c-104">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="58b7c-105">方法</span><span class="sxs-lookup"><span data-stu-id="58b7c-105">Methods</span></span>

| <span data-ttu-id="58b7c-106">方法</span><span class="sxs-lookup"><span data-stu-id="58b7c-106">Method</span></span>       | <span data-ttu-id="58b7c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="58b7c-107">Return Type</span></span> | <span data-ttu-id="58b7c-108">说明</span><span class="sxs-lookup"><span data-stu-id="58b7c-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="58b7c-109">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="58b7c-109">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="58b7c-110">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="58b7c-110">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="58b7c-111">读取 connectionOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58b7c-111">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="58b7c-112">属性</span><span class="sxs-lookup"><span data-stu-id="58b7c-112">Properties</span></span>

| <span data-ttu-id="58b7c-113">属性</span><span class="sxs-lookup"><span data-stu-id="58b7c-113">Property</span></span> | <span data-ttu-id="58b7c-114">类型</span><span class="sxs-lookup"><span data-stu-id="58b7c-114">Type</span></span>                          | <span data-ttu-id="58b7c-115">描述</span><span class="sxs-lookup"><span data-stu-id="58b7c-115">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="58b7c-116">error</span><span class="sxs-lookup"><span data-stu-id="58b7c-116">error</span></span>    | [<span data-ttu-id="58b7c-117">errorDetail</span><span class="sxs-lookup"><span data-stu-id="58b7c-117">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="58b7c-118">如果`status`为`failed`，则提供有关导致失败的错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="58b7c-118">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="58b7c-119">id</span><span class="sxs-lookup"><span data-stu-id="58b7c-119">id</span></span>       | <span data-ttu-id="58b7c-120">String</span><span class="sxs-lookup"><span data-stu-id="58b7c-120">String</span></span>                        | <span data-ttu-id="58b7c-121">ConnectionOperation 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58b7c-121">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="58b7c-122">只读。</span><span class="sxs-lookup"><span data-stu-id="58b7c-122">Read-only.</span></span> |
| <span data-ttu-id="58b7c-123">状态</span><span class="sxs-lookup"><span data-stu-id="58b7c-123">status</span></span>   | <span data-ttu-id="58b7c-124">string</span><span class="sxs-lookup"><span data-stu-id="58b7c-124">string</span></span>                        | <span data-ttu-id="58b7c-125">指示异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="58b7c-125">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="58b7c-126">可取值为：`unspecified`、`inprogress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="58b7c-126">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="58b7c-127">关系</span><span class="sxs-lookup"><span data-stu-id="58b7c-127">Relationships</span></span>

<span data-ttu-id="58b7c-128">无</span><span class="sxs-lookup"><span data-stu-id="58b7c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58b7c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58b7c-129">JSON representation</span></span>

<span data-ttu-id="58b7c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58b7c-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.errorDetail"},
  "id": "String (identifier)",
  "status": "string"
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
