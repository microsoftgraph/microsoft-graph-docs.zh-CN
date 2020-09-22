---
title: errorDetail 资源类型
description: 介绍了失败请求以异步方式创建 Microsoft Search 连接架构的错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6f37f3ca432dcd9c755556b37f4f0ea330907426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013725"
---
# <a name="errordetail-resource-type"></a><span data-ttu-id="a7ad2-103">errorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7ad2-103">errorDetail resource type</span></span>

<span data-ttu-id="a7ad2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7ad2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7ad2-105">介绍了失败请求以异步方式创建 Microsoft Search 连接 [架构](schema.md) 的错误。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-105">Describes an error for a failed request to create a Microsoft Search connection [schema](schema.md) asynchronously.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="a7ad2-106">属性</span><span class="sxs-lookup"><span data-stu-id="a7ad2-106">Properties</span></span>

| <span data-ttu-id="a7ad2-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7ad2-107">Property</span></span>  | <span data-ttu-id="a7ad2-108">类型</span><span class="sxs-lookup"><span data-stu-id="a7ad2-108">Type</span></span>                                               | <span data-ttu-id="a7ad2-109">说明</span><span class="sxs-lookup"><span data-stu-id="a7ad2-109">Description</span></span> |
|:----------|:---------------------------------------------------|:------------|
| <span data-ttu-id="a7ad2-110">详细信息</span><span class="sxs-lookup"><span data-stu-id="a7ad2-110">details</span></span>   | <span data-ttu-id="a7ad2-111">[innerErrorDetail](innererrordetail.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7ad2-111">[innerErrorDetail](innererrordetail.md) collection</span></span> | <span data-ttu-id="a7ad2-112">内部错误的集合（如果有）。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-112">A collection of inner errors, if any.</span></span> <span data-ttu-id="a7ad2-113">只读的，可空。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-113">Read-only, nullable.</span></span> |
| <span data-ttu-id="a7ad2-114">errorCode</span><span class="sxs-lookup"><span data-stu-id="a7ad2-114">errorCode</span></span> | <span data-ttu-id="a7ad2-115">String</span><span class="sxs-lookup"><span data-stu-id="a7ad2-115">String</span></span>                                             | <span data-ttu-id="a7ad2-116">与错误相关联的错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-116">The error code associated with the error, if any.</span></span> <span data-ttu-id="a7ad2-117">只读的，可空。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-117">Read-only, nullable.</span></span> |
| <span data-ttu-id="a7ad2-118">message</span><span class="sxs-lookup"><span data-stu-id="a7ad2-118">message</span></span>   | <span data-ttu-id="a7ad2-119">String</span><span class="sxs-lookup"><span data-stu-id="a7ad2-119">String</span></span>                                             | <span data-ttu-id="a7ad2-120">人类可读错误消息。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-120">The human-readable error message.</span></span> <span data-ttu-id="a7ad2-121">只读。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-121">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a7ad2-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7ad2-122">JSON representation</span></span>

<span data-ttu-id="a7ad2-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7ad2-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "details",
    "errorCode"
  ],
  "@odata.type": "microsoft.graph.errorDetail",
  "baseType": null
}-->

```json
{
  "details": [{"@odata.type": "microsoft.graph.innerErrorDetail"}],
  "errorCode": "String",
  "message": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "errorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


