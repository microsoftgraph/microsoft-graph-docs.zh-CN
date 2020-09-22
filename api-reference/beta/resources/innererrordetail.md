---
title: innerErrorDetail 资源类型
description: 包含在 errorDetail 对象中的内部错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 07220eaead4035dafcb7cd7032916ae4a5db0d75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021901"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="57237-103">innerErrorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="57237-103">innerErrorDetail resource type</span></span>

<span data-ttu-id="57237-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57237-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57237-105">包含在 [errorDetail](errordetail.md) 对象中的内部错误。</span><span class="sxs-lookup"><span data-stu-id="57237-105">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="57237-106">属性</span><span class="sxs-lookup"><span data-stu-id="57237-106">Properties</span></span>

| <span data-ttu-id="57237-107">属性</span><span class="sxs-lookup"><span data-stu-id="57237-107">Property</span></span> | <span data-ttu-id="57237-108">类型</span><span class="sxs-lookup"><span data-stu-id="57237-108">Type</span></span>   | <span data-ttu-id="57237-109">描述</span><span class="sxs-lookup"><span data-stu-id="57237-109">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="57237-110">message</span><span class="sxs-lookup"><span data-stu-id="57237-110">message</span></span>  | <span data-ttu-id="57237-111">String</span><span class="sxs-lookup"><span data-stu-id="57237-111">String</span></span> | <span data-ttu-id="57237-112">人类可读错误消息。</span><span class="sxs-lookup"><span data-stu-id="57237-112">The human-readable error message.</span></span> <span data-ttu-id="57237-113">只读。</span><span class="sxs-lookup"><span data-stu-id="57237-113">Read-only.</span></span> |
| <span data-ttu-id="57237-114">source</span><span class="sxs-lookup"><span data-stu-id="57237-114">source</span></span>   | <span data-ttu-id="57237-115">String</span><span class="sxs-lookup"><span data-stu-id="57237-115">String</span></span> | <span data-ttu-id="57237-116">错误的来源。</span><span class="sxs-lookup"><span data-stu-id="57237-116">The source of the error.</span></span> <span data-ttu-id="57237-117">只读。</span><span class="sxs-lookup"><span data-stu-id="57237-117">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="57237-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57237-118">JSON representation</span></span>

<span data-ttu-id="57237-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57237-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


