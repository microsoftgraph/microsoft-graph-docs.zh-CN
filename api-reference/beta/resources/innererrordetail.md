---
title: innerErrorDetail 资源类型
description: 包含在 errorDetail 对象中的内部错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c1dd87e6af015423441b75ada256456e748e3805
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495926"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="50545-103">innerErrorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="50545-103">innerErrorDetail resource type</span></span>

<span data-ttu-id="50545-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="50545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50545-105">包含在[errorDetail](errordetail.md)对象中的内部错误。</span><span class="sxs-lookup"><span data-stu-id="50545-105">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="50545-106">属性</span><span class="sxs-lookup"><span data-stu-id="50545-106">Properties</span></span>

| <span data-ttu-id="50545-107">属性</span><span class="sxs-lookup"><span data-stu-id="50545-107">Property</span></span> | <span data-ttu-id="50545-108">类型</span><span class="sxs-lookup"><span data-stu-id="50545-108">Type</span></span>   | <span data-ttu-id="50545-109">描述</span><span class="sxs-lookup"><span data-stu-id="50545-109">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="50545-110">message</span><span class="sxs-lookup"><span data-stu-id="50545-110">message</span></span>  | <span data-ttu-id="50545-111">String</span><span class="sxs-lookup"><span data-stu-id="50545-111">String</span></span> | <span data-ttu-id="50545-112">人类可读错误消息。</span><span class="sxs-lookup"><span data-stu-id="50545-112">The human-readable error message.</span></span> <span data-ttu-id="50545-113">只读。</span><span class="sxs-lookup"><span data-stu-id="50545-113">Read-only.</span></span> |
| <span data-ttu-id="50545-114">source</span><span class="sxs-lookup"><span data-stu-id="50545-114">source</span></span>   | <span data-ttu-id="50545-115">String</span><span class="sxs-lookup"><span data-stu-id="50545-115">String</span></span> | <span data-ttu-id="50545-116">错误的来源。</span><span class="sxs-lookup"><span data-stu-id="50545-116">The source of the error.</span></span> <span data-ttu-id="50545-117">只读。</span><span class="sxs-lookup"><span data-stu-id="50545-117">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="50545-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50545-118">JSON representation</span></span>

<span data-ttu-id="50545-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50545-119">The following is a JSON representation of the resource.</span></span>

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
