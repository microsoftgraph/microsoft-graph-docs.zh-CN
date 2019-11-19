---
title: connectionOperation 资源类型
description: 描述用于创建 Microsoft Search 连接架构的异步请求的状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9ced1c9bd00e3e865c3663ed6ade936747b9dded
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704141"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="8a574-103">connectionOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a574-103">connectionOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a574-104">描述用于创建 Microsoft Search 连接[架构](schema.md)的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="8a574-104">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="8a574-105">方法</span><span class="sxs-lookup"><span data-stu-id="8a574-105">Methods</span></span>

| <span data-ttu-id="8a574-106">方法</span><span class="sxs-lookup"><span data-stu-id="8a574-106">Method</span></span>       | <span data-ttu-id="8a574-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a574-107">Return Type</span></span> | <span data-ttu-id="8a574-108">说明</span><span class="sxs-lookup"><span data-stu-id="8a574-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a574-109">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="8a574-109">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="8a574-110">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="8a574-110">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="8a574-111">读取 connectionOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8a574-111">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a574-112">属性</span><span class="sxs-lookup"><span data-stu-id="8a574-112">Properties</span></span>

| <span data-ttu-id="8a574-113">属性</span><span class="sxs-lookup"><span data-stu-id="8a574-113">Property</span></span> | <span data-ttu-id="8a574-114">类型</span><span class="sxs-lookup"><span data-stu-id="8a574-114">Type</span></span>                          | <span data-ttu-id="8a574-115">说明</span><span class="sxs-lookup"><span data-stu-id="8a574-115">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="8a574-116">error</span><span class="sxs-lookup"><span data-stu-id="8a574-116">error</span></span>    | [<span data-ttu-id="8a574-117">errorDetail</span><span class="sxs-lookup"><span data-stu-id="8a574-117">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="8a574-118">如果`status`为`failed`，则提供有关导致失败的错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8a574-118">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="8a574-119">id</span><span class="sxs-lookup"><span data-stu-id="8a574-119">id</span></span>       | <span data-ttu-id="8a574-120">String</span><span class="sxs-lookup"><span data-stu-id="8a574-120">String</span></span>                        | <span data-ttu-id="8a574-121">ConnectionOperation 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a574-121">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="8a574-122">只读。</span><span class="sxs-lookup"><span data-stu-id="8a574-122">Read-only.</span></span> |
| <span data-ttu-id="8a574-123">状态</span><span class="sxs-lookup"><span data-stu-id="8a574-123">status</span></span>   | <span data-ttu-id="8a574-124">string</span><span class="sxs-lookup"><span data-stu-id="8a574-124">string</span></span>                        | <span data-ttu-id="8a574-125">指示异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8a574-125">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="8a574-126">可取值为：`unspecified`、`inprogress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="8a574-126">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a574-127">关系</span><span class="sxs-lookup"><span data-stu-id="8a574-127">Relationships</span></span>

<span data-ttu-id="8a574-128">无</span><span class="sxs-lookup"><span data-stu-id="8a574-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a574-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a574-129">JSON representation</span></span>

<span data-ttu-id="8a574-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a574-130">The following is a JSON representation of the resource.</span></span>

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
