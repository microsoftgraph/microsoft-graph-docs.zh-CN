---
title: connectionOperation 资源类型
description: 描述用于创建 Microsoft Search 连接架构的异步请求的状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21d962bbbfee64c51f11cf1ac3f5e7de2c0497e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507483"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="e4328-103">connectionOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4328-103">connectionOperation resource type</span></span>

<span data-ttu-id="e4328-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e4328-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4328-105">描述用于创建 Microsoft Search 连接[架构](schema.md)的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="e4328-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="e4328-106">方法</span><span class="sxs-lookup"><span data-stu-id="e4328-106">Methods</span></span>

| <span data-ttu-id="e4328-107">方法</span><span class="sxs-lookup"><span data-stu-id="e4328-107">Method</span></span>       | <span data-ttu-id="e4328-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4328-108">Return Type</span></span> | <span data-ttu-id="e4328-109">说明</span><span class="sxs-lookup"><span data-stu-id="e4328-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e4328-110">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e4328-110">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="e4328-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e4328-111">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="e4328-112">读取 connectionOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4328-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4328-113">属性</span><span class="sxs-lookup"><span data-stu-id="e4328-113">Properties</span></span>

| <span data-ttu-id="e4328-114">属性</span><span class="sxs-lookup"><span data-stu-id="e4328-114">Property</span></span> | <span data-ttu-id="e4328-115">类型</span><span class="sxs-lookup"><span data-stu-id="e4328-115">Type</span></span>                          | <span data-ttu-id="e4328-116">说明</span><span class="sxs-lookup"><span data-stu-id="e4328-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="e4328-117">error</span><span class="sxs-lookup"><span data-stu-id="e4328-117">error</span></span>    | [<span data-ttu-id="e4328-118">errorDetail</span><span class="sxs-lookup"><span data-stu-id="e4328-118">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="e4328-119">如果`status`为`failed`，则提供有关导致失败的错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e4328-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="e4328-120">id</span><span class="sxs-lookup"><span data-stu-id="e4328-120">id</span></span>       | <span data-ttu-id="e4328-121">String</span><span class="sxs-lookup"><span data-stu-id="e4328-121">String</span></span>                        | <span data-ttu-id="e4328-122">ConnectionOperation 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e4328-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="e4328-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e4328-123">Read-only.</span></span> |
| <span data-ttu-id="e4328-124">状态</span><span class="sxs-lookup"><span data-stu-id="e4328-124">status</span></span>   | <span data-ttu-id="e4328-125">string</span><span class="sxs-lookup"><span data-stu-id="e4328-125">string</span></span>                        | <span data-ttu-id="e4328-126">指示异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e4328-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="e4328-127">可取值为：`unspecified`、`inprogress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="e4328-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e4328-128">关系</span><span class="sxs-lookup"><span data-stu-id="e4328-128">Relationships</span></span>

<span data-ttu-id="e4328-129">无</span><span class="sxs-lookup"><span data-stu-id="e4328-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4328-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4328-130">JSON representation</span></span>

<span data-ttu-id="e4328-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4328-131">The following is a JSON representation of the resource.</span></span>

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
