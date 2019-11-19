---
title: innerErrorDetail 资源类型
description: 包含在 errorDetail 对象中的内部错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6b3dfb2ec4caf8ae2b8ec9a279a6d001ad3aaae7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703775"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="e9639-103">innerErrorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9639-103">innerErrorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9639-104">包含在[errorDetail](errordetail.md)对象中的内部错误。</span><span class="sxs-lookup"><span data-stu-id="e9639-104">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="e9639-105">属性</span><span class="sxs-lookup"><span data-stu-id="e9639-105">Properties</span></span>

| <span data-ttu-id="e9639-106">属性</span><span class="sxs-lookup"><span data-stu-id="e9639-106">Property</span></span> | <span data-ttu-id="e9639-107">类型</span><span class="sxs-lookup"><span data-stu-id="e9639-107">Type</span></span>   | <span data-ttu-id="e9639-108">描述</span><span class="sxs-lookup"><span data-stu-id="e9639-108">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="e9639-109">message</span><span class="sxs-lookup"><span data-stu-id="e9639-109">message</span></span>  | <span data-ttu-id="e9639-110">String</span><span class="sxs-lookup"><span data-stu-id="e9639-110">String</span></span> | <span data-ttu-id="e9639-111">人类可读错误消息。</span><span class="sxs-lookup"><span data-stu-id="e9639-111">The human-readable error message.</span></span> <span data-ttu-id="e9639-112">只读。</span><span class="sxs-lookup"><span data-stu-id="e9639-112">Read-only.</span></span> |
| <span data-ttu-id="e9639-113">source</span><span class="sxs-lookup"><span data-stu-id="e9639-113">source</span></span>   | <span data-ttu-id="e9639-114">String</span><span class="sxs-lookup"><span data-stu-id="e9639-114">String</span></span> | <span data-ttu-id="e9639-115">错误的来源。</span><span class="sxs-lookup"><span data-stu-id="e9639-115">The source of the error.</span></span> <span data-ttu-id="e9639-116">只读。</span><span class="sxs-lookup"><span data-stu-id="e9639-116">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="e9639-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9639-117">JSON representation</span></span>

<span data-ttu-id="e9639-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9639-118">The following is a JSON representation of the resource.</span></span>

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
