---
title: genericError 资源类型
description: 通用错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: bb43271706ddfd46324ee871405a28bdfa868448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132779"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="1db60-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="1db60-103">genericError resource type</span></span>

<span data-ttu-id="1db60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1db60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1db60-105">通用错误。</span><span class="sxs-lookup"><span data-stu-id="1db60-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="1db60-106">属性</span><span class="sxs-lookup"><span data-stu-id="1db60-106">Properties</span></span>

| <span data-ttu-id="1db60-107">属性</span><span class="sxs-lookup"><span data-stu-id="1db60-107">Property</span></span> | <span data-ttu-id="1db60-108">类型</span><span class="sxs-lookup"><span data-stu-id="1db60-108">Type</span></span> | <span data-ttu-id="1db60-109">描述</span><span class="sxs-lookup"><span data-stu-id="1db60-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1db60-110">message</span><span class="sxs-lookup"><span data-stu-id="1db60-110">message</span></span> | <span data-ttu-id="1db60-111">String</span><span class="sxs-lookup"><span data-stu-id="1db60-111">String</span></span> | <span data-ttu-id="1db60-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="1db60-112">The error message.</span></span> |
| <span data-ttu-id="1db60-113">code</span><span class="sxs-lookup"><span data-stu-id="1db60-113">code</span></span> | <span data-ttu-id="1db60-114">String</span><span class="sxs-lookup"><span data-stu-id="1db60-114">String</span></span> | <span data-ttu-id="1db60-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="1db60-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1db60-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1db60-116">JSON representation</span></span>

<span data-ttu-id="1db60-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1db60-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```

