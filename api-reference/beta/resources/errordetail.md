---
title: errorDetail 资源类型
description: 介绍了失败请求以异步方式创建 Microsoft Search 连接架构的错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7f77ccacd6e1f5339706549873ea4c75d9144e39
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704183"
---
# <a name="errordetail-resource-type"></a><span data-ttu-id="b4943-103">errorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4943-103">errorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4943-104">介绍了失败请求以异步方式创建 Microsoft Search 连接[架构](schema.md)的错误。</span><span class="sxs-lookup"><span data-stu-id="b4943-104">Describes an error for a failed request to create a Microsoft Search connection [schema](schema.md) asynchronously.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="b4943-105">属性</span><span class="sxs-lookup"><span data-stu-id="b4943-105">Properties</span></span>

| <span data-ttu-id="b4943-106">属性</span><span class="sxs-lookup"><span data-stu-id="b4943-106">Property</span></span>  | <span data-ttu-id="b4943-107">类型</span><span class="sxs-lookup"><span data-stu-id="b4943-107">Type</span></span>                                               | <span data-ttu-id="b4943-108">说明</span><span class="sxs-lookup"><span data-stu-id="b4943-108">Description</span></span> |
|:----------|:---------------------------------------------------|:------------|
| <span data-ttu-id="b4943-109">详细信息</span><span class="sxs-lookup"><span data-stu-id="b4943-109">details</span></span>   | <span data-ttu-id="b4943-110">[innerErrorDetail](innererrordetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="b4943-110">[innerErrorDetail](innererrordetail.md) collection</span></span> | <span data-ttu-id="b4943-111">内部错误的集合（如果有）。</span><span class="sxs-lookup"><span data-stu-id="b4943-111">A collection of inner errors, if any.</span></span> <span data-ttu-id="b4943-112">只读的，可空。</span><span class="sxs-lookup"><span data-stu-id="b4943-112">Read-only, nullable.</span></span> |
| <span data-ttu-id="b4943-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="b4943-113">errorCode</span></span> | <span data-ttu-id="b4943-114">String</span><span class="sxs-lookup"><span data-stu-id="b4943-114">String</span></span>                                             | <span data-ttu-id="b4943-115">与错误相关联的错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="b4943-115">The error code associated with the error, if any.</span></span> <span data-ttu-id="b4943-116">只读的，可空。</span><span class="sxs-lookup"><span data-stu-id="b4943-116">Read-only, nullable.</span></span> |
| <span data-ttu-id="b4943-117">message</span><span class="sxs-lookup"><span data-stu-id="b4943-117">message</span></span>   | <span data-ttu-id="b4943-118">String</span><span class="sxs-lookup"><span data-stu-id="b4943-118">String</span></span>                                             | <span data-ttu-id="b4943-119">人类可读错误消息。</span><span class="sxs-lookup"><span data-stu-id="b4943-119">The human-readable error message.</span></span> <span data-ttu-id="b4943-120">只读。</span><span class="sxs-lookup"><span data-stu-id="b4943-120">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b4943-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4943-121">JSON representation</span></span>

<span data-ttu-id="b4943-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4943-122">The following is a JSON representation of the resource.</span></span>

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
