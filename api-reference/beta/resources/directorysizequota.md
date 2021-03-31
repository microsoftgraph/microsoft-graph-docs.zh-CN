---
title: directorySizeQuota 资源类型
description: 表示公司使用的目录配额和总目录配额。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 54e2280fdb416e5ccfd0853ee77a2ef3f90ddf37
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469372"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="8236e-103">directorySizeQuota 资源类型</span><span class="sxs-lookup"><span data-stu-id="8236e-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8236e-104">表示公司使用的目录配额和总目录配额。</span><span class="sxs-lookup"><span data-stu-id="8236e-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="8236e-105">属性</span><span class="sxs-lookup"><span data-stu-id="8236e-105">Properties</span></span>
| <span data-ttu-id="8236e-106">属性</span><span class="sxs-lookup"><span data-stu-id="8236e-106">Property</span></span>   | <span data-ttu-id="8236e-107">类型</span><span class="sxs-lookup"><span data-stu-id="8236e-107">Type</span></span>|<span data-ttu-id="8236e-108">说明</span><span class="sxs-lookup"><span data-stu-id="8236e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8236e-109">使用的内容</span><span class="sxs-lookup"><span data-stu-id="8236e-109">used</span></span>|<span data-ttu-id="8236e-110">Int32</span><span class="sxs-lookup"><span data-stu-id="8236e-110">Int32</span></span>| <span data-ttu-id="8236e-111">已使用的目录配额量。</span><span class="sxs-lookup"><span data-stu-id="8236e-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="8236e-112">total</span><span class="sxs-lookup"><span data-stu-id="8236e-112">total</span></span>|<span data-ttu-id="8236e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8236e-113">Int32</span></span>| <span data-ttu-id="8236e-114">目录配额的总量。</span><span class="sxs-lookup"><span data-stu-id="8236e-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8236e-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8236e-115">JSON representation</span></span>

<span data-ttu-id="8236e-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8236e-116">The following is a JSON representation of the resource.</span></span>

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
