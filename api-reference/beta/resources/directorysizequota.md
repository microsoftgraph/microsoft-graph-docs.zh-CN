---
title: directorySizeQuota 资源类型
description: 表示公司使用的目录配额和总目录配额。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 3af82a957e152f0edf4d87e6fdf9a7888d4b64e4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133985"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="190e3-103">directorySizeQuota 资源类型</span><span class="sxs-lookup"><span data-stu-id="190e3-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="190e3-104">表示公司使用的目录配额和总目录配额。</span><span class="sxs-lookup"><span data-stu-id="190e3-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="190e3-105">属性</span><span class="sxs-lookup"><span data-stu-id="190e3-105">Properties</span></span>
| <span data-ttu-id="190e3-106">属性</span><span class="sxs-lookup"><span data-stu-id="190e3-106">Property</span></span>   | <span data-ttu-id="190e3-107">类型</span><span class="sxs-lookup"><span data-stu-id="190e3-107">Type</span></span>|<span data-ttu-id="190e3-108">说明</span><span class="sxs-lookup"><span data-stu-id="190e3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="190e3-109">使用的内容</span><span class="sxs-lookup"><span data-stu-id="190e3-109">used</span></span>|<span data-ttu-id="190e3-110">Int32</span><span class="sxs-lookup"><span data-stu-id="190e3-110">Int32</span></span>| <span data-ttu-id="190e3-111">已使用的目录配额量。</span><span class="sxs-lookup"><span data-stu-id="190e3-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="190e3-112">total</span><span class="sxs-lookup"><span data-stu-id="190e3-112">total</span></span>|<span data-ttu-id="190e3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="190e3-113">Int32</span></span>| <span data-ttu-id="190e3-114">目录配额的总量。</span><span class="sxs-lookup"><span data-stu-id="190e3-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="190e3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="190e3-115">JSON representation</span></span>

<span data-ttu-id="190e3-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="190e3-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
