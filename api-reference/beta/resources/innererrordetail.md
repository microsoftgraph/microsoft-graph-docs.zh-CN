---
title: innerErrorDetail 资源类型
description: 包含在 errorDetail 对象中的内部错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a5b85f17b87343766a4edb00c6d620c185ecaf5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939654"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="99dd6-103">innerErrorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="99dd6-103">innerErrorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99dd6-104">包含在[errorDetail](errordetail.md)对象中的内部错误。</span><span class="sxs-lookup"><span data-stu-id="99dd6-104">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="99dd6-105">属性</span><span class="sxs-lookup"><span data-stu-id="99dd6-105">Properties</span></span>

| <span data-ttu-id="99dd6-106">属性</span><span class="sxs-lookup"><span data-stu-id="99dd6-106">Property</span></span> | <span data-ttu-id="99dd6-107">类型</span><span class="sxs-lookup"><span data-stu-id="99dd6-107">Type</span></span>   | <span data-ttu-id="99dd6-108">描述</span><span class="sxs-lookup"><span data-stu-id="99dd6-108">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="99dd6-109">message</span><span class="sxs-lookup"><span data-stu-id="99dd6-109">message</span></span>  | <span data-ttu-id="99dd6-110">String</span><span class="sxs-lookup"><span data-stu-id="99dd6-110">String</span></span> | <span data-ttu-id="99dd6-111">人类可读错误消息。</span><span class="sxs-lookup"><span data-stu-id="99dd6-111">The human-readable error message.</span></span> <span data-ttu-id="99dd6-112">只读。</span><span class="sxs-lookup"><span data-stu-id="99dd6-112">Read-only.</span></span> |
| <span data-ttu-id="99dd6-113">source</span><span class="sxs-lookup"><span data-stu-id="99dd6-113">source</span></span>   | <span data-ttu-id="99dd6-114">字符串</span><span class="sxs-lookup"><span data-stu-id="99dd6-114">String</span></span> | <span data-ttu-id="99dd6-115">错误的来源。</span><span class="sxs-lookup"><span data-stu-id="99dd6-115">The source of the error.</span></span> <span data-ttu-id="99dd6-116">只读。</span><span class="sxs-lookup"><span data-stu-id="99dd6-116">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="99dd6-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99dd6-117">JSON representation</span></span>

<span data-ttu-id="99dd6-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99dd6-118">The following is a JSON representation of the resource.</span></span>

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
