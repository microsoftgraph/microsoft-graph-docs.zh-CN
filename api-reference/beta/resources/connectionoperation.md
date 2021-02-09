---
title: connectionOperation 资源类型
description: 描述创建 Microsoft 搜索连接架构的异步请求的状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e17b1f55b00fd7b9bdc69eb7a7a34d3453ab332d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158301"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="986e6-103">connectionOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="986e6-103">connectionOperation resource type</span></span>

<span data-ttu-id="986e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="986e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="986e6-105">描述创建 Microsoft 搜索连接架构的异步请求 [的状态](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="986e6-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="986e6-106">方法</span><span class="sxs-lookup"><span data-stu-id="986e6-106">Methods</span></span>

| <span data-ttu-id="986e6-107">方法</span><span class="sxs-lookup"><span data-stu-id="986e6-107">Method</span></span>       | <span data-ttu-id="986e6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="986e6-108">Return Type</span></span> | <span data-ttu-id="986e6-109">说明</span><span class="sxs-lookup"><span data-stu-id="986e6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="986e6-110">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="986e6-110">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="986e6-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="986e6-111">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="986e6-112">读取 connectionOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="986e6-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="986e6-113">属性</span><span class="sxs-lookup"><span data-stu-id="986e6-113">Properties</span></span>

| <span data-ttu-id="986e6-114">属性</span><span class="sxs-lookup"><span data-stu-id="986e6-114">Property</span></span> | <span data-ttu-id="986e6-115">类型</span><span class="sxs-lookup"><span data-stu-id="986e6-115">Type</span></span>                          | <span data-ttu-id="986e6-116">说明</span><span class="sxs-lookup"><span data-stu-id="986e6-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="986e6-117">error</span><span class="sxs-lookup"><span data-stu-id="986e6-117">error</span></span>    | [<span data-ttu-id="986e6-118">errorDetail</span><span class="sxs-lookup"><span data-stu-id="986e6-118">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="986e6-119">如果是 `status` `failed` ，则提供有关导致失败的错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="986e6-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="986e6-120">id</span><span class="sxs-lookup"><span data-stu-id="986e6-120">id</span></span>       | <span data-ttu-id="986e6-121">String</span><span class="sxs-lookup"><span data-stu-id="986e6-121">String</span></span>                        | <span data-ttu-id="986e6-122">connectionOperation 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="986e6-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="986e6-123">只读。</span><span class="sxs-lookup"><span data-stu-id="986e6-123">Read-only.</span></span> |
| <span data-ttu-id="986e6-124">状态</span><span class="sxs-lookup"><span data-stu-id="986e6-124">status</span></span>   | <span data-ttu-id="986e6-125">string</span><span class="sxs-lookup"><span data-stu-id="986e6-125">string</span></span>                        | <span data-ttu-id="986e6-126">指示异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="986e6-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="986e6-127">可取值为：`unspecified`、`inprogress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="986e6-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="986e6-128">关系</span><span class="sxs-lookup"><span data-stu-id="986e6-128">Relationships</span></span>

<span data-ttu-id="986e6-129">无</span><span class="sxs-lookup"><span data-stu-id="986e6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="986e6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="986e6-130">JSON representation</span></span>

<span data-ttu-id="986e6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="986e6-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
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


